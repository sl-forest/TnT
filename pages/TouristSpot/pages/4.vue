<template>

  <div>
    <header>
      <!-- ロゴ -->
      <div class="logo">
        <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>
      </div>

      <!--  サイトの名前 -->
      <div class="site-name">
        <a href="http://localhost:3000"><h1>鹿児島紹介サイト</h1></a>
      </div>

      <!-- メニュー -->
      <nav>
        <div class="menu">
          <ul class="item">
            <li><a class="item-link" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a class="item-link" href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
        <h1>「観光地」</h1>

        <h2 class = spot_headline>仙巌園</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Senganen.jpg" alt="">
            </div>

            <div class = explanation>
                <p>江戸時代初期に薩摩藩主・島津氏によって造られた、別邸跡とその庭園。</p>
                <p>錦江湾や桜島の景観を取り入れた設計で、雄大な景色が楽しめる。</p>
                <p>隣接する尚古集成館は幕末に建てられた金属加工の工場跡で、世界遺産「明治日本の産業革命遺産」のひとつ。</p>
                <p>島津家の歴史や近代化事業を紹介する展示が行われている。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Sengannen">スポット情報</a>
        </div>

        

        <h2 class = spot_headline>天文館</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/TenmonKan.jpg" alt="天文館">
            </div>

            <div class = explanation>
                <p>南九州一の繁華街として人気のスポット。</p>
                <p>江戸時代に、西洋文明を進んで取り入れた島津重豪公が1779年に天文観測や暦の作成などを行う施設「明時館（別名天文館）」を建てたことが名前の由来。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Tenmonkan">スポット情報</a>
        </div>

        <h2 class = spot_headline>知覧特攻平和会館</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Kinenkan.jpg" alt="知覧特攻平和会館">
            </div>
            
            <div class = explanation>
                <p>館内では、平和を祈念し、その記録を後世に正しく伝えるべく、陸軍特別攻撃隊員や各地の戦地で</p>
                <p>戦死した隊員たちの遺品、遺影、関係資料を展示している。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/ChiranPeaceMuseum">スポット情報</a>
        </div>

        <h2 class = spot_headline>維新ふるさと館</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Furusatokan.jpg" alt="維新ふるさと館">
            </div>
            
            <div class = explanation>
                <p>西郷隆盛、大久保利通など明治維新に活躍した偉人の出身地加治屋町にある歴史ミュージアム。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Ishinfurusatokan">スポット情報</a>
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

  <fotter>

  </fotter>
  
  </div>

</template>

<style>
    /* スマホ向けスタイル */

    /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
      main {
        max-width: 1024px;
        margin: 0 auto;
      }
      
      header {
        flex-wrap: wrap; /*折り返し */
        display: flex;  /*ヘッダーの下の要素を並列に*/
        padding: 0; /*ヘッダーの位置調整*/
        background: #333; /*ヘッダーの背景色*/
      }
      
      .site-name h1 {
        color: #fff;  /*サイトの名前の色*/
      }

      .site-name a {
        text-decoration: none;
      }

      .logo {
        margin: 5px 15px;
      }

      .logo a img {
        width: 65px;  /*ロゴ画像の幅調整*/
        height: 65px; /*ロゴ画像の高さ調整*/
        padding-top: 1.5px; /*ロゴの位置調整*/
      }
      
      nav ul {
        padding-left: 3em;
      }

      .item ul {
        display: inline-block;
        margin-top: 25px;
      }

      ul {
        list-style: none;
        padding: 0;
      }
      
      .item li {
        display: inline-block;
        list-style: none;
        margin-right: 16px;
        padding: 10px;
        border-bottom: 2px solid #2ac5b3;
      }

      .item li a {
        color: #fff;  /*メニューの色*/
        text-decoration: none;  /*メニューの下線を消す*/
      }
      
      h1 {
        margin-bottom: 0;
      }

      h2.spot_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 工芸品一覧説明 */
      .spot {
        display: flex;
      }

      .spot p {
        margin: 0;
        font-size: 14px;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 観光地画像 */
      .spot_img img{
        width: 5cm;
        height: auto;
      }
      
      /* ページネーション */
      .Pagination {
        display: flex;
        align-items: center;
        justify-content: center;
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

      .Pagination-Item-Link-Icon {
        width: 20px;
      }

      .Pagination-Item-Link.isActive {
        background: #111;
        color: #fff;
        pointer-events: none;
      }

      .Pagination-Item-Link:not(.isActive):hover {
        background: #111;
        color: #fff;
      }

      .Pagination > * + * {
        margin-left: 8px;
      }

    }

</style>