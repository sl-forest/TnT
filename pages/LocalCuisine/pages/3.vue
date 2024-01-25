<template>

  <div>
    <TheHeader />

    <main>
      <h1>「郷土料理」</h1>
      <h2 class = localcuisine_headline>白熊</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Shirokuma.jpg" alt="白熊">
          <div class="teikyou">
            <p>
              出典：<br>
              農林水産省「うちの郷土料理」
            </p>
          </div>
        </div>
        
        <div class = explanation>
          <p>「白熊」は、削った氷に練乳をかけ、その上にチェリーやレーズン、みかん、パイン、小豆、寒天と、色とりどりのトッピングをのせた氷菓子。</p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/ShiroKuma">白熊はこちら</a>
        </div>
      </div>

      <h2 class = localcuisine_headline>かるかん</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Karukan02.jpg" alt="かるかん">
          <div class="teikyou">
            <p>画像提供元：鹿児島県</p>
          </div>
        </div>

        <div class = explanation>
          <p>「かるかん」は、かるかん粉、山芋、水を使ってつくる鹿児島県の銘菓。</p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Karukan">かるかんはこちら</a>
        </div>
      </div>

      <h2 class = localcuisine_headline>両棒餅（じゃんぼ餅）</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Janbomoti.jpg" alt="じゃんぼ餅">
          <div class="teikyou">
            <p>
              出典：<br>
              農林水産省「うちの郷土料理」
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            「じゃんぼ餅」とは、つきたての餅やもち米粉を使っただんご串を2本さして、とろみのある<br>
            砂糖醤油ダレをかけて食べる、鹿児島県で古くから親しまれている料理である。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/JumboMochi">両棒餅はこちら</a>
        </div>
      </div>

      <h2 class = localcuisine_headline>神酒（みき）</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Miki.jpg" alt="みき">
          <div class="teikyou">
            <p>
              出典：<br>
              農林水産省「うちの郷土料理」
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            米とさつまいも、砂糖を使った乳酸菌発酵飲料で、奄美地域の他に沖縄県でも飲まれている。
            沖縄県では、さつまいもではなく麦を使う。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Miki">神酒はこちら</a>
        </div>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/1"><span>1</span></a>
          </li>
          
          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/2"><span>2</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link isActive" href="http://localhost:3000/LocalCuisine/pages/3"><span>3</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/3">
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

h2.localcuisine_headline {
  margin: 0;                       /* 全余白の指定 */
  padding: 8px 0;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

/* 提供文字 */
.teikyou {font-weight: bold;  /* 文字の太さ */}

.teikyou p {
  margin: 0;        /* 全余白の指定 */
  font-size: 13px;    /* 文字の大きさ */
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

  h1 {
    padding: 8px 0;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
  }

  br {display: none;}     /* 表示しない */

  .localcuisine {text-align: center;}

  h2.localcuisine_headline {text-align: center;}

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px;
  }

  .link-space {margin: 16px 0;}

/* 画像 */
  .localcuisine_img img {height: 7cm;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 郷土料理一覧説明 */
  .localcuisine {
    display: flex;
    margin-bottom: 16px;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

/* 画像 */
  .localcuisine_img img {width: 5cm;}
}
</style>