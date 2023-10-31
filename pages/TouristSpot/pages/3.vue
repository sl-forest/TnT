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
        <h2 class = spot_headline>指宿温泉 砂むし会館 砂楽</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Sunamushi.jpg" alt="指宿温泉 砂むし会館 砂楽">
            </div>
            
            <div class = explanation>
                <p>海岸に天然砂むし温泉、屋内には大浴場や休憩所を完備した、指宿温泉を代表する日帰り入浴施設。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Ibusukionsen">スポット情報</a>
        </div>

        <h2 class = spot_headline>霧島温泉市場</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Itiba.jpg" alt="霧島温泉市場">
            </div>
            
            <div class = explanation>
                <p>霧島温泉郷の中心に位置する「霧島温泉市場」は、観光案内所・土産店・食事処が集まる施設。</p>
                <p>鹿児島・霧島の特産品を多数取り揃えたお店があり、お土産探しにぴったり。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kirishimaonsenitiba">スポット情報</a>
        </div>
        
        <h2 class = spot_headline>霧島神宮</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Jingu.jpg" alt="霧島神宮">
            </div>

            <div class = explanation>
                <p>鹿児島県屈指のパワースポットで、6世紀に建立された歴史ある神社。</p>
                <p>御主神は、建国神話の主人公である瓊々杵尊（ににぎのみこと）。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kirishimajingu">スポット情報</a>
        </div>

        <h2 class = spot_headline>鹿児島神宮</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/kagoshimajingu.jpg" alt="鹿児島神宮">
            </div>

            <div class = explanation>
                <p>天津日高日子穂穂出見尊（山幸彦）と豊玉比売命を主祭神として祀る。</p>
                <p>旧暦1月18日を過ぎた最初の日曜には初午祭がある。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kagoshimajingu">スポット情報</a>
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