<template>

  <div>
    <TheHeader />

    <main>
      <h1>「郷土料理」</h1>
      <h2 class = localcuisine_headline>鶏飯</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Keihan.jpg" alt="鶏飯">
          <div class="teikyou">
            <p>
              写真協力：<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>
        
        <div class = explanation>
          <p>
            「鶏飯」は、ほぐした鶏肉、干ししいたけ、錦糸卵、パパイヤの味噌漬け、みかんの皮などを、<br>
            白いごはんの上にのせ、鶏ガラのスープをかけて食べる、奄美地域を代表する郷土料理。<br>
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Keihan">鶏飯はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = localcuisine_headline>ぶり大根</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Buridaikon.jpg" alt="ぶり大根">
        </div>

        <div class = explanation>
          <p>
            鹿児島県の特産品であるブリと大根を使った「ぶり大根」は冬の定番料理として親しまれている。<br>
            ブリの旨味と大根の甘みが一体となった、冬の定番料理。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/BuriDaikon">ぶり大根はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = localcuisine_headline>鶏刺し</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Torisashi.jpeg" alt="鶏刺し">
          <div class="teikyou">
            <p>
              写真協力：<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            もも肉、むね肉、ささみ、砂肝などの部位を魚のお刺身と同じように醤油をつけて食べる料理。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/ChickenSashimi">鳥刺しはこちら</a>
          </div>
        </div>
      </div>

      <h2 class = localcuisine_headline>豚汁</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonjiru.jpg" alt="豚汁">
        </div>
        
        <div class = explanation>
          <p>
            豚肉（主にバラ肉）と好みの野菜（ニンジン、ゴボウ、だいこん）などを煮て、<br>
            味噌仕立てにした汁物で、味噌汁の一種。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Tonjiru">豚汁はこちら</a>
          </div>
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
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/LocalCuisine/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/3"><span>3</span></a>
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
  margin: 0;                       /* 要素の外側余白 */
  padding: 8px 0;                  /* 要素の内側余白 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

/* 提供文字 */
.teikyou {font-weight: bold;}  /* 文字の太さ */

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
  padding: 0;               /* 要素の内側余白 */
  display: flex;            /* 親要素に対して子要素を横並びにする */
  align-items: center;      /* 上下の中央揃え */
  justify-content: center;  /* 横並び要素の左右中央揃え */
  list-style: none;         /* 黒点削除 */
}

.Pagination-Item-Link {
  width: 45px;              /* 横幅 */
  height: 45px;             /* 高さ */
  border-radius: 50%;       /* 角を丸める */  
  display: flex;            /* 親要素に対して子要素を横並びにする */
  justify-content: center;  /* 横並び要素の左右中央揃え */
  align-items: center;      /* 上下の中央揃え */
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
  .localcuisine_img img {width: 320px;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 郷土料理一覧説明 */
  .localcuisine {
    display: flex;        /* 親要素に対して子要素を横並び */
    margin-bottom: 16px;  /* 要素の外側下余白 */
    column-gap: 1rem;     /* 行や列の間のすき間を定義 */
  }
  
  .explanation {align-self: center;}  /* 中央揃え */

  .link-space {margin-top: 0.5rem;} /* 要素の外側上余白 */

/* 画像 */
  .localcuisine_img img {width: 190px;}
}
</style>