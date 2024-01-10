<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>指宿温泉 砂むし会館 砂楽</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Sunamushi.jpg" alt="指宿温泉 砂むし会館 砂楽">
        </div>
        
        <div class = explanation>
          <p>海岸に天然砂むし温泉、屋内には大浴場や休憩所を完備した、指宿温泉を代表する日帰り入浴施設。</p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Ibusukionsen"><b>スポット情報</b></a>
        </div>
      </div>

      <h2 class = spot_headline>霧島温泉市場</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Itiba.jpg" alt="霧島温泉市場">
        </div>
        
        <div class = explanation>
          <p>
            霧島温泉郷の中心に位置する「霧島温泉市場」は、観光案内所・土産店・食事処が集まる施設。<br class="pc">
            鹿児島・霧島の特産品を多数取り揃えたお店があり、お土産探しにぴったり。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kirishimaonsenitiba"><b>スポット情報</b></a>
        </div>
      </div>
      
      <h2 class = spot_headline>霧島神宮</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Jingu.jpg" alt="霧島神宮">
        </div>

        <div class = explanation>
          <p>
            鹿児島県屈指のパワースポットで、6世紀に建立された歴史ある神社。<br class="pc">
            御主神は、建国神話の主人公である瓊々杵尊（ににぎのみこと）。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kirishimajingu"><b>スポット情報</b></a>
        </div>
      </div>

      <h2 class = spot_headline>鹿児島神宮</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/kagoshimajingu.jpg" alt="鹿児島神宮">
        </div>

        <div class = explanation>
          <p>
            天津日高日子穂穂出見尊（山幸彦）と豊玉比売命を主祭神として祀る。<br class="pc">
            旧暦1月18日を過ぎた最初の日曜には初午祭がある。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kagoshimajingu"><b>スポット情報</b></a>
        </div>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/1">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
            </svg>
          </a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/4"><span>4</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/4">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M13 5l7 7-7 7M5 5l7 7-7 7" />
            </svg>
          </a>
        </li>
      </ul>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
main {margin: 0 auto;}

h1 {font-family: 'New Tegomin', serif;}

/* ページネーション */
.Pagination {
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
}

.Pagination-Item-Link {
  width: 45px;
  height: 45px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  flex-wrap: wrap;
  overflow: hidden;
  background: #fff;
  border: solid 2px #111;
  font-size: 14px;
  color: #111;
  font-weight: bold;
  transition: all 0.15s linear;
}

.Pagination-Item-Link-Icon {width: 20px;}

.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  .pc {display: none;}

  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  .spot {
    text-align: center;
  }

  h2.spot_headline {
    margin: 0;
    text-align: center;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  .link-space {margin: 8px 0;}

  .explanation p {
    font-size: 15px;
    text-align: left; /* 左寄せ */
    margin-top: 16px;
    margin-bottom: 0;
  }
  
  .explanation-link {
    text-decoration: none;
    color: blue;
  }
  
/* 観光地理画像 */
  .spot_img img{
    width: 8cm;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }

  h1 {margin-bottom: 0;}
  
/* 観光地一覧説明 */
  .spot {display: flex;}

  .spot p {
    margin: 0;
    font-size: 14px;
  }

  h2.spot_headline {
    margin: 0;
    padding-top: 8px;
    border-top: 2px solid #d5d4c3;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

  .link-space a {
    margin: 0;
    font-size: 14px;
  }

  .explanation-link {
    align-self: end;
    text-decoration: none;
    color: blue;
  }

  a:hover.explanation-link {color: rgb(71, 1, 92);}

/* 観光地画像 */
  .spot_img img{
    width: 5cm;
    height: auto;
  }
}
</style>