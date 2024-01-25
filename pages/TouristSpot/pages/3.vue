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
          <p>
            海岸に天然砂むし温泉、屋内には大浴場や休憩所を完備した、<br>
            指宿温泉を代表する日帰り入浴施設。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Ibusukionsen">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>霧島温泉市場</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Itiba.jpg" alt="霧島温泉市場">
        </div>
        
        <div class = explanation>
          <p>
            霧島温泉郷の中心に位置する「霧島温泉市場」は、観光案内所・土産店・食事処が<br>
            集まる施設。<br>
            鹿児島・霧島の特産品を多数取り揃えたお店があり、お土産探しにぴったり。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kirishimaonsenitiba">スポット情報</a>
        </div>
      </div>
      
      <h2 class = spot_headline>霧島神宮</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Jingu.jpg" alt="霧島神宮">
        </div>

        <div class = explanation>
          <p>
            鹿児島県屈指のパワースポットで、6世紀に建立された歴史ある神社。<br>
            御主神は、建国神話の主人公である瓊々杵尊（ににぎのみこと）。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kirishimajingu">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>鹿児島神宮</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/kagoshimajingu.jpg" alt="鹿児島神宮">
        </div>

        <div class = explanation>
          <p>
            天津日高日子穂穂出見尊（山幸彦）と豊玉比売命を主祭神として祀る。<br>
            旧暦1月18日を過ぎた最初の日曜には初午祭がある。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kagoshimajingu">スポット情報</a>
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
body {margin: 0;}       /* 要素の外側余白 */

main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;                          /* 要素の外側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

h2.spot_headline {
  margin: 0;                       /* 全余白の指定 */
  padding: 8px 0;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

.explanation p {
  margin: 0;          /* 全余白の指定 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;      /* インラインブロック要素へ変更 */
  padding: 0.3em 0.6em;       /* 要素の内側余白 */
  text-decoration: none;      /* 下線無効 */
  color: black;             /* 文字の色 */
  border: solid 2px black;  /* 枠線 */
  border-radius: 3px;         /* 要素の境界の外側の角を丸める */
  transition: .4s;            /* 要素の2つの状態間の変化を定義する */
}

/* マウスオーバー */
.btn:hover {
  background: black;  /* 背景 */
  color: white;       /* 文字の色 */
}

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
  body {margin-top: 18%;} /* 要素の外側上余白 */

  br {display: none;}     /* 表示しない */

  h1 {
    padding: 8px 0;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
  }

  .spot {text-align: center;}

  h2.spot_headline {text-align: center;}

  .link-space {margin: 16px 0;}

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px;
  }
  
/* 画像 */
  .spot_img img{height: 7cm;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .spot {
    display: flex;
    margin-bottom: 16px;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

/* 画像 */
  .spot_img img {width: 5cm;}
}
</style>