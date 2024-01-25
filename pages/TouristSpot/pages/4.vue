<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>仙巌園</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Senganen.jpg" alt="仙厳園">
        </div>

        <div class = explanation>
          <p>
            江戸時代初期に薩摩藩主・島津氏によって造られた、別邸跡とその庭園。<br>
            錦江湾や桜島の景観を取り入れた設計で、雄大な景色が楽しめる。<br>
            隣接する尚古集成館は幕末に建てられた金属加工の工場跡で、<br>
            世界遺産「明治日本の産業革命遺産」のひとつ。<br>
            島津家の歴史や近代化事業を紹介する展示が行われている。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Sengannen">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>天文館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/TenmonKan.jpg" alt="天文館">
        </div>

        <div class = explanation>
          <p>
            南九州一の繁華街として人気のスポット。<br>
            江戸時代に、西洋文明を進んで取り入れた島津重豪公が1779年に天文観測や暦の作成<br>
            などを行う施設「明時館（別名天文館）」を建てたことが名前の由来。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Tenmonkan">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>知覧特攻平和会館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Kinenkan.jpg" alt="知覧特攻平和会館">
        </div>
        
        <div class = explanation>
          <p>
            館内では、平和を祈念し、その記録を後世に正しく伝えるべく、陸軍特別攻撃隊員や<br>
            各地の戦地で戦死した隊員たちの遺品、遺影、関係資料を展示している。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/ChiranPeaceMuseum">スポット情報</a>
        </div>
      </div>

      <h2 class = spot_headline>維新ふるさと館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Furusatokan.jpg" alt="維新ふるさと館">
        </div>
        
        <div class = explanation>
          <p>
            西郷隆盛、大久保利通など明治維新に活躍した偉人の出身地加治屋町に<br>
            ある歴史ミュージアム。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Ishinfurusatokan">スポット情報</a>
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
            <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/3"><span>3</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/4"><span>4</span></a>
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
  .spot_img img{height: 6cm;}
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