<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>桜島</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/sakurajima.jpg" alt="桜島">
        </div>
        
        <div class = explanation>
          <p>
            鹿児島のシンボルである「桜島」は、錦江湾にある陸続きの島。<br>
            標高約1,117メートルの御岳（北岳）という活火山が、現在も活発に噴火を続けている。<br>
            散策に適した溶岩遊歩道の途中には、絶景を望める展望所も複数完備。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Sakurajima">桜島はこちら</a>
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
            小さな面積ながら、九州最高峰の宮之浦岳（標高約1,936メートル）をはじめ、<br>
            1,000メートル超の山々が46座もあり、「洋上のアルプス」と呼ばれている。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Yakushima">屋久島はこちら</a>
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
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Amami">奄美大島はこちら</a>
        </div>
      </div>

      <h2 class = spot_headline>種子島宇宙センター</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/SpaceCenter.jpg" alt="種子島宇宙センター">
        </div>

        <div class = explanation>
          <p>
            1969年に造られた種子島宇宙センターは、総面積約970万平米に及ぶ、<br>
            日本最大のロケット発射場。<br>
            青い海と白い砂浜に囲まれていることから、「世界一美しいロケット発射場」<br>
            と呼ばれている。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/SpaceCenter">宇宙センターはこちら</a>
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
  .spot_img img {width: 400px;}
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

/* 観光地画像 */
  .spot_img img {width: 192px;}
}
</style>