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
        <h1>「伝統工芸品」</h1>
        <h2 class = craft_headline>屋久杉</h2>
        <div class="craft">
            <div class = craft04_img>
                <img src="~/assets/img/Yakusugi.jpg" alt="屋久杉">
            </div>

            <div class = explanation>
                <p>世界自然遺産に登録されている「屋久島」は1,000メートル以上の高峰が連なっており、この大自然の中で育った樹齢1,000年以上のものを「屋久杉」と呼んでいる。</p>
                <p> 木目の美しさ、色、かおりの良さなど、まさに銘木というにふさわしく、家具やインテリア用品などに幅広く活用されている。</p>
                <p>現在は自然保護のため、倒木や土埋木だけを工芸品として加工しています。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>薩摩切子</h2>
        <div class="craft">
            <div class = craft01_img>
                <img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子">
            </div>

            <div class = explanation>
                <p>江戸末期に薩摩藩で造られた切子ガラス。</p>
                <p>鉛を24～25%含むクリスタルガラスを使用し、無色のガラス（クリアガラス）の表面に色ガラスを1～2mm程度溶着させた ”色被せガラス”にカットを施し、磨きあげた製品を「薩摩切子」と言う。</p> 
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>薩摩つげ櫛</h2>
        <div class="craft">
            <div class = craft04_img>
                <img src="~/assets/img/Tugegushi.jpg" alt="薩摩つげ櫛">
            </div>

            <div class = explanation>
                <p>江戸時代から「櫛になりたや薩摩の櫛に、諸国娘の手に渡ろ」とうたわれ、全国に名を馳せていた。</p>
                <p>材質が硬く、色艶が美しいのが特徴。</p>
                <p>なめらかな櫛どおりで、静電気・抜け毛・切れ毛が少ないといわれている。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
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
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3">
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

      h2.craft_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 工芸品一覧説明 */
      .craft {
        display: flex;
      }

      .craft p {
        margin: 0;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 工芸品画像 */
      .craft01_img img{
        width: 5cm;
        height: auto;
      }

      .craft03_img img{
        width: 5cm;
        height: auto;
      }

      .craft04_img img{
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