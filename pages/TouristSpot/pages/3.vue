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
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Ibusukionsen">指宿温泉 砂むし会館 砂楽はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = spot_headline>霧島温泉市場</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Itiba.jpg" alt="霧島温泉市場">
        </div>
        
        <div class = explanation>
          <p>
            霧島温泉郷の中心に位置する「霧島温泉市場」は、観光案内所・土産店・食事処が集まる施設。<br>
            鹿児島・霧島の特産品を多数取り揃えたお店があり、お土産探しにぴったり。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kirishimaonsenitiba">霧島温泉市場はこちら</a>
          </div>
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
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kirishimajingu">霧島神宮はこちら</a>
          </div>
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
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Kagoshimajingu">鹿児島神宮はこちら</a>
          </div>
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
  margin: 0;                        /* 全余白の指定 */
  padding: 8px 0;                   /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;  /* 上線 */
}

.explanation p {
  margin: 0;           /* 全余白の指定 */
  font-family: serif;  /* フォントの変更 */
  font-weight: bold;   /* 文字の太さ */
  font-size: 15px;     /* 文字の大きさ */
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

  .spot {text-align: center;} /* 中央揃え */

  h2.spot_headline {text-align: center;}  /* 中央揃え */

  .link-space {margin: 16px 0;} /* 要素の外側余白 */

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px; /* 要素の外側上余白 */
  }
  
/* 画像 */
  .spot_img img {width: 400px;} /* 横幅 */
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .spot {
    display: flex;        /* 親要素に対して子要素を横並び */
    margin-bottom: 16px;  /* 要素の外側下余白 */
    column-gap: 1rem;     /* 行や列の間のすき間を定義 */
  }
  
  .explanation {align-self: center;}  /* 中央揃え */

  .link-space {margin-top: 0.5rem;} /* 要素の外側上余白 */

/* 画像 */
  .spot_img img {width: 192px;} /* 横幅 */
}
</style>