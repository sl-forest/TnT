<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>仙巌園</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Senganen-min.jpg" alt="仙厳園">
        </div>

        <div class = explanation>
          <p>
            江戸時代初期に薩摩藩主・島津氏によって造られた、別邸跡とその庭園。<br>
            隣接する尚古集成館は幕末に建てられた金属加工の工場跡で、世界遺産「明治日本の産業革命遺産」のひとつ。<br>
            島津家の歴史や近代化事業を紹介する展示が行われている。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Sengannen">仙厳園はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = spot_headline>天文館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/TenmonKan-min.jpg" alt="天文館">
        </div>

        <div class = explanation>
          <p>
            南九州一の繁華街として人気のスポット。<br>
            江戸時代に、西洋文明を進んで取り入れた島津重豪公が1779年に天文観測や暦の作成などを<br>
            行う施設「明時館（別名天文館）」を建てたことが名前の由来。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Tenmonkan">天文館はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = spot_headline>知覧特攻平和会館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Kinenkan-min.jpg" alt="知覧特攻平和会館">
        </div>
        
        <div class = explanation>
          <p>
            館内では、平和を祈念し、その記録を後世に正しく伝えるべく、陸軍特別攻撃隊員や<br>
            各地の戦地で戦死した隊員たちの遺品、遺影、関係資料を展示している。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/ChiranPeaceMuseum">知覧特攻平和会館はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = spot_headline>維新ふるさと館</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/Furusatokan-min.jpg" alt="維新ふるさと館">
        </div>
        
        <div class = explanation>
          <p>
            西郷隆盛、大久保利通など明治維新に活躍した偉人の出身地加治屋町にある歴史ミュージアム。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/TouristSpot/pages/Ishinfurusatokan">維新ふるさと館はこちら</a>
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
body {margin: 0;}
main {margin: 0 auto;}

h1 {
  margin: 0;
  font-family: 'New Tegomin', serif;
}

h2.spot_headline {
  margin: 0;
  padding: 8px 0;
  border-top: 2px solid #d5d4c3;
}

.explanation p {
  margin: 0;
  font-family: serif;
  font-weight: bold;
  font-size: 15px;
}

/* ボタン */
.btn {
  display: inline-block;
  padding: 0.3em 0.6em;
  text-decoration: none;
  color: black;
  border: solid 2px black;
  border-radius: 3px;
  transition: .4s;
}

/* マウスオーバー */
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

/* アクティブボタン */
.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

/* マウスオーバー */
.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}
  br {display: none;}

  h1 {
    padding: 8px 0;
    text-align: center;
  }

  .spot {text-align: center;}
  h2.spot_headline {text-align: center;}
  .link-space {margin: 16px 0;}

  .explanation p {
    text-align: left;
    margin-top: 16px;
  }
  
/* 画像 */
  .spot_img img {
    width: 400px;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}
  h1 {padding-top: 16px;}
  
/* 一覧説明 */
  .spot {
    display: flex;
    margin-bottom: 16px;
    column-gap: 1rem;
  }
  
  .explanation {align-self: center;}
  .link-space {margin-top: 0.5rem;}

/* 画像 */
  .spot_img img {
    width: 192px;
    height: auto;
  }
}
</style>