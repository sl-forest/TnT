<template>

  <div>
    <TheHeader />

    <main>
      <h1>「県指定伝統工芸品」</h1>
      <h2 class = craft_headline>屋久杉</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Yakusugi.jpg" alt="屋久杉">
        </div>

        <div class = explanation>
          <p>
            世界自然遺産に登録されている「屋久島」は1,000メートル以上の高峰が連なっており、<br>
            この大自然の中で育った樹齢1,000年以上のものを「屋久杉」と呼んでいる。<br>
            現在は自然保護のため、倒木や土埋木だけを工芸品として加工している。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/Yakusugi">屋久杉はこちら</a>
        </div>

      </div>

      <h2 class = craft_headline>薩摩切子</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子">
        </div>

        <div class = explanation>
          <p>
            江戸末期に薩摩藩で造られた切子ガラス。鉛を24～25%含むクリスタルガラスを使用。<br>
            無色のガラス（クリアガラス）の表面に色ガラスを1～2mm程度溶着させた <br>
            ”色被せガラス”にカットを施し、磨きあげた製品を「薩摩切子」と言う。
          </p> 
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/SatsumaKiriko">薩摩切子はこちら</a>
        </div>

      </div>

      <h2 class = craft_headline>薩摩つげ櫛</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Tugegushi.jpg" alt="薩摩つげ櫛">
        </div>

        <div class = explanation>
          <p>
            江戸時代から「櫛になりたや薩摩の櫛に、諸国娘の手に渡ろ」とうたわれ、<br>全国に名を馳せていた。
            材質が硬く、色艶が美しいのが特徴。<br>
            なめらかな櫛どおりで、静電気・抜け毛・切れ毛が少ないといわれている。
          </p>
        </div>

        <div class="link-space">
          <a class="btn" href="http://localhost:3000/Craft/pages/SatsumaBoxwoodComb">薩摩つげ櫛はこちら</a>
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
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
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
  margin: 0;            /* 要素の外側余白 */
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
  border-radius: 3px;         /* 角を丸める */
  transition: .4s;            /* 要素の2つの状態間の変化を定義する */
}

/* マウスオーバー */
.btn:hover {
  background: black;  /* 背景 */
  color: white;       /* 文字の色 */
}

/* ページネーション */
.Pagination {
  padding: 0;               /* 要素の内側余白 */
  display: flex;            /* 親要素に対して子要素を横並びにする */
  align-items: center;      /* 中央揃え */
  justify-content: center;  /* 横並び要素の中央揃え */
  list-style: none;         /* 黒点削除 */
}

.Pagination-Item-Link {
  width: 45px;              /* 横幅 */
  height: 45px;             /* 高さ */
  border-radius: 50%;       /* 角を丸める */  
  display: flex;            /* 親要素に対して子要素を横並びにする */
  justify-content: center;  /* 横並び要素の中央揃え */
  align-items: center;      /* 中央揃え */
  text-decoration: none;    /* 下線無効 */
  flex-wrap: wrap;          /* 子要素を折り返す */       
  overflow: hidden;         /* 要素からはみ出た部分を非表示 */
  background: #fff;       /* 背景 */
  border: solid 2px #111; /* 枠線 */
  font-size: 14px;          /* 文字の大きさ */
  color: #111;            /* 文字の色 */
  font-weight: bold;        /* 文字の太さ */
  transition: all 0.15s linear; /* 要素の2つの状態間の変化を定義する */
}

.Pagination-Item-Link-Icon {width: 20px;} /* 横幅 */

/* アクティブボタン */
.Pagination-Item-Link.isActive {
  background: #111;   /* 背景 */
  color: #fff;        /* 文字の色 */
  pointer-events: none; /* クリックやタッチ操作を無効化 */
}

/* マウスオーバー */
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
    padding: 8px 0;       /* 要素の内側余白 */
    text-align: center;   /* 中央揃え */
  }

  .craft {text-align: center;}  /* 中央揃え */

  h2.craft_headline {text-align: center;} /* 中央揃え */

  .link-space {margin: 16px 0;} /* 要素の外側余白 */

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
    display: flex;        /* 親要素に対して子要素を横並びにする */
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