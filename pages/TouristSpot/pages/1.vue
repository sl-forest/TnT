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
        <h2 class = spot_headline>桜島</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/sakurajima02.jpg" alt="桜島">
            </div>
            
            <div class = explanation>
                <p>鹿児島のシンボルである「桜島」は、錦江湾にある陸続きの島。</p>
                <p>標高約1,117メートルの御岳（北岳）という活火山が、現在も活発に噴火を続けている。</p>
                <p>散策に適した溶岩遊歩道の途中には、絶景を望める展望所も複数完備。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Sakurajima">スポット情報</a>
        </div>

        <h2 class = spot_headline>屋久島</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Yakushima.jpg" alt="屋久島">
            </div>

            <div class = explanation>
                <p>日本で初めて世界自然遺産に登録された。</p>
                <p>本土最南端・鹿児島県佐多岬の南南西約60キロメートルの海上に位置する島。</p>
                <p>小さな面積ながら、九州最高峰の宮之浦岳（標高約1,936メートル）をはじめ、1,000メートル超の山々が46座もあり、「洋上のアルプス」と呼ばれている。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Yakushima">スポット情報</a>
        </div>

        <h2 class = spot_headline>奄美大島</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/Amami.jpg" alt="奄美大島">
            </div>

            <div class = explanation>
                <p>世界自然遺産に登録されている。</p>
                <p>鹿児島県と沖縄県の中間に位置し、日本版「天国に一番近い島」と称されている。</p>
                <p>青く澄んだ海や、ここにしか生息していない動植物など、雄大な自然が魅力。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Amami">スポット情報</a>
        </div>

        <h2 class = spot_headline>種子島宇宙センター</h2>
        <div class="spot">
            <div class = spot_img>
                <img src="~/assets/img/SpaceCenter.jpg" alt="種子島宇宙センター">
            </div>

            <div class = explanation>
                <p>1969年に造られた種子島宇宙センターは、総面積約970万平米に及ぶ、日本最大のロケット発射場。</p>
                <p>青い海と白い砂浜に囲まれていることから、「世界一美しいロケット発射場」と呼ばれている。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/SpaceCenter">スポット情報</a>
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
                <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/1"><span>1</span></a>
              </li>
              
              <li class="Pagination-Item">
                <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/2"><span>2</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/3"><span>3</span></a>
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