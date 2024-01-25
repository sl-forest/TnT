<template>

  <div>
    <TheHeader />
    <main>
      <h1>「国指定伝統工芸品」</h1>
      <h2 class = craft_headline>本場大島紬</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/OshimaTsumugi.jpg" alt="本場大島紬">
        </div>
        
        <div class = explanation>
          <p>
            1,300年の歴史を持ち、絹織物の最高傑作といわれている。<br>
            30数工程もある緻密な手作業により、図案から織り上がるまで半年から1年以上もかかる。<br>
            大島紬村では本場大島紬の製造現場見学や、泥染め・織り体験、着付体験などが楽しめる。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/AuthenticOshimaTsumugi">本場大島紬はこちら</a>
        </div>

      </div>

      <h2 class = craft_headline>川辺仏壇</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/kawabebutudan.jpg" alt="川辺仏壇">
        </div>

        <div class = explanation>
          <p>
            川辺仏壇（かわなべぶつだん）は、鹿児島県南九州市川辺町周辺で作られている仏壇。<br>
            川辺仏壇の特徴は、「ガマ戸」と呼ばれる川辺仏壇オリジナルの独特な仏壇がある。<br>
            ”ガマ”とは、鹿児島県の方言で洞窟を表す。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/KawabeButsudan">川辺仏壇はこちら</a>
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
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
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
  margin: 0;                       /* 要素の外側余白 */
  padding: 8px 0;                  /* 要素の内側余白 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

.explanation p {
  margin: 0;          /* 要素の外側余白 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;      /* インラインブロック要素へ変更 */
  padding: 0.4em 0.8em;       /* 要素の内側余白 */
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
  width: 45px;              /* 横幅 */
  height: 45px;             /* 高さ */
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

.Pagination-Item-Link-Icon {width: 20px;} /* 横幅 */

/* マウスオーバー */
.Pagination-Item-Link.isActive {
  background: #111;   /* 背景 */
  color: #fff;        /* 文字の色 */
  pointer-events: none; /* クリックやタッチ操作を無効化 */
}

.Pagination-Item-Link:not(.isActive):hover {
  background: #111; /* 背景 */
  color: #fff;      /* 文字の色 */
}

.Pagination > * + * {margin-left: 8px;} /* 要素の外側左余白 */

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */
  
  br {display: none;}     /* 表示しない */

  h1 {
    padding: 8px 0;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
  }

  .craft {text-align: center;}

  h2.craft_headline {text-align: center;}

  .link-space {margin: 8px 0;}  /* 要素の外側余白 */

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px; /* 要素の外側上余白 */
  }
  
/* 画像 */
  .craft_img img {width: 320px;}  /* 横幅 */
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .craft {
    display: flex;
    margin-bottom: 16px;  /* 要素の外側下余白 */
  }
  
  .explanation {
    margin: auto; /* 要素の外側余白 */
    width: 40em;  /* 横幅 */
  }

  .link-space {align-self: end;}

/* 画像 */
  .craft_img img {width: 180px;}  /* 横幅 */
}
</style>