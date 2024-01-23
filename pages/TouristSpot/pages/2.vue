<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>曾木の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/SogiTaki.jpg" alt="曾木の滝">
        </div>
          
        <div class = explanation>
          <p>
            幅約210メートル、高さ約12メートルのスケールを誇り、<br>
            「東洋のナイアガラ」とも呼ばれる滝。<br>
            春は桜やつつじが彩り、夏は水量も多く豪快。<br>
            秋は紅葉がライトアップされ、冬は雪景色を楽しめる。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Soginotaki">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>丸尾の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/MaruoTaki.jpg" alt="丸尾の滝">
        </div>

        <div class = explanation>
          <p>
            高さ約23メートル、幅約16メートルの滝。<br>
            ここを流れる水は温泉の湯であり、霧島地区の温泉水を集めて流れる珍しい「湯の滝」。
          </p>
        </div>
        <div class="link-space">
          <a class ="ntn" href="http://localhost:3000/TouristSpot/pages/Maruonotaki">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>雄川の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/OgawaTaki.jpg" alt="雄川の滝">
        </div>

        <div class = explanation>
          <p>
            落差約46メートル、幅約60メートルの滝。<br>
            大河ドラマ『西郷どん』のオープニング映像で話題となった。<br>
            エメラルドグリーンの美しい滝つぼが特徴で、フォトジェニックな光景が広がる。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Ogawanotaki">スポット情報</a>
        </div>
      </div>
      
      <h2 class = spot_headline>開聞岳</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/KaimonDake.jpg" alt="開聞岳">
        </div>

        <div class = explanation>
          <p>
            薩摩半島の最南端に位置する標高約924メートルの開聞岳は、「日本百名山」<br>
            にも数えられている南薩摩を代表する山。<br>
            別名「薩摩富士」と呼ばれ、指宿のシンボルとして親しまれている。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kaimondake">スポット情報</a>
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
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/2"><span>2</span></a>
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
  display: inline-block;
  padding: 0.3em 0.8em;
  text-decoration: none;
  color: black;
  border: solid 2px black;
  border-radius: 3px;
  transition: .4s;
}

.btn:hover {
  background: black;
  color: white;
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