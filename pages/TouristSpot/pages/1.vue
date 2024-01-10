<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>桜島</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/sakurajima02.jpg" alt="桜島">
        </div>
        
        <div class = explanation>
          <p>
            鹿児島のシンボルである「桜島」は、錦江湾にある陸続きの島。<br>
            標高約1,117メートルの御岳（北岳）という活火山が、現在も活発に噴火を続けている。<br>
            散策に適した溶岩遊歩道の途中には、絶景を望める展望所も複数完備。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Sakurajima"><b>スポット情報</b></a>
        </div>
      </div>

      <h2 class = spot_headline>屋久島</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Yakushima.jpg" alt="屋久島">
        </div>

        <div class = explanation>
          <p>
            日本で初めて世界自然遺産に登録された。<br>
            本土最南端・鹿児島県佐多岬の南南西約60キロメートルの海上に位置する島。<br>
            小さな面積ながら、九州最高峰の宮之浦岳（標高約1,936メートル）をはじめ、1,000メートル超の山々が46座もあり、「洋上のアルプス」と呼ばれている。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Yakushima"><b>スポット情報</b></a>
        </div>
      </div>

      <h2 class = spot_headline>奄美大島</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Amami.jpg" alt="奄美大島">
        </div>

        <div class = explanation>
          <p>
            世界自然遺産に登録されている。<br>
            鹿児島県と沖縄県の中間に位置し、日本版「天国に一番近い島」と称されている。<br>
            青く澄んだ海や、ここにしか生息していない動植物など、雄大な自然が魅力。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Amami"><b>スポット情報</b></a>
        </div>
      </div>

      <h2 class = spot_headline>種子島宇宙センター</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/SpaceCenter.jpg" alt="種子島宇宙センター">
        </div>

        <div class = explanation>
          <p>
            1969年に造られた種子島宇宙センターは、総面積約970万平米に及ぶ、日本最大のロケット発射場。<br>
            青い海と白い砂浜に囲まれていることから、「世界一美しいロケット発射場」と呼ばれている。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/SpaceCenter"><b>スポット情報</b></a>
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
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/3"><span>3</span></a>
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
  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  br {display: none;}

  .spot {text-align: center;}

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
  main {max-width: 1024px;}

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