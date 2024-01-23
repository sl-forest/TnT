<template>

  <div>
    <TheHeader />
    <main>
      <h1>「国指定伝統工芸品」</h1>
      <h2 class = craft_headline>薩摩焼</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
        </div>

        <div class = explanation>
          <p>
            薩摩焼は、鹿児島県内で焼かれる陶磁器。<br>
            鉄分が多い土を高温で焼き締めるため、素朴で頑丈な仕上がりが特徴。<br>
           「白もん」と呼ばれる豪華絢爛な色絵錦手の陶器と<br>「黒もん」と呼ばれる大衆向けの雑器に分かれる。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/SatsumaPorcelain">薩摩焼はこちら</a>
        </div>

      </div>

      <h2 class = craft_headline>白薩摩</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/ShiroSatsuma.jpg" alt="白薩摩">
        </div>

        <div class = explanation>
          <p>
            淡い黄色の地に無色の釉薬が掛かった陶器で表面を貫入という細かいヒビが覆っており<br>
            「白もん」と呼ばれている。<br>
            白土を使った「白もん」は珍重され、藩主のみに使用が許されたもので、幕末のパリ万博に<br>
            出品し、多くの人々の注目と賞賛を得た。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/WhiteSatsuma">白薩摩はこちら</a>
        </div>

      </div>

      <h2 class = craft_headline>黒薩摩</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/KuroSatsuma.jpg" alt="黒薩摩">
        </div>

        <div class = explanation>
          <p>
            「黒薩摩」は鉄分の多い鹿児島の土とシラス層や凝塊岩などに雑木灰を調合したうわ薬を<br>
            使い、素朴で剛健な焼物で「黒もん」と呼ばれている。<br>
            「黒もん」は庶民生活道具として鹿児島の人々に愛されている。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/BlackSatsuma">黒薩摩はこちら</a>
        </div>

      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4"><span>4</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4">
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

h2.craft_headline {
  margin: 0px;                       /* 要素の外側余白 */
  padding: 8px 0px;                  /* 要素の内側余白 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

.explanation p {
  margin: 0px;          /* 要素の外側余白 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;
  padding: 0.4em 0.8em;       /* 要素の内側余白 */
  text-decoration: none;
  color: black;             /* 文字の色 */
  border: solid 2px black;
  border-radius: 3px;
  transition: .4s;
}

.btn:hover {
  background: black;  /* 背景 */
  color: white;       /* 文字の色 */
}

/* ページネーション */
.Pagination {
  padding: 0;               /* 要素の内側余白 */
  display: flex;            /* 親要素に対して子要素を横並びにする  */
  align-items: center;      /* 上下の中央揃え */
  justify-content: center;
  list-style: none;
}

.Pagination-Item-Link {
  width: 45px;              /* 横幅 */
  height: 45px;             /* 高さ */
  border-radius: 50%;
  display: flex;            /* 親要素に対して子要素を横並びにする  */
  justify-content: center;
  align-items: center;
  text-decoration: none;
  flex-wrap: wrap;
  overflow: hidden;         /* 要素からはみ出た部分を非表示 */
  background: #fff;       /* 背景 */
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
    padding: 8px 0px;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
  }

  .craft {text-align: center;}  /* 左右の中央揃え */

  h2.craft_headline {text-align: center;} /* 左右の中央揃え */

  .link-space {margin: 16px 0;} /* 要素の外側余白 */

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px; /* 要素の外側上余白 */
  }
  
/* 画像 */
  .craft_img img {width: 8cm;}  /* 横幅 */
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .craft {
    display: flex;        /* 親要素に対して子要素を横並びにする  */
    margin-bottom: 16px;  /* 要素の外側下余白 */
  }
  
  .explanation {
    margin: auto; /* 要素の外側余白 */
    width: 40em;  /* 横幅 */
  }

  .link-space {align-self: end;}

/* 画像 */
  .craft_img img {width: 5cm;}  /* 横幅 */
}
</style>