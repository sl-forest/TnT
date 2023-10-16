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
            <li><a class="item-link" href="http://localhost:3000/TraditionalCulture/pages/1">伝統芸能</a></li>
            <li><a class="item-link" href="http://localhost:3000">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
      <h1>開聞岳</h1>
        <div class="TouristSpot">
            <div class = TouristSpot_img>
                <img src="~/assets/img/KaimonDake.jpg" alt="開聞岳">
            </div>
            
            <div class = TouristSpot_note>
                
                <h2>移動方法</h2>
                <p>【電車】JR指宿枕崎線「開聞」駅より徒歩約20分で登山口</p>

                <div class = "Hotel">
                    <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000479.html">開聞岳 周辺のホテル・旅館</a>
                </div>
                    
            </div>
        </div>
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
      padding-left: 24px;
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

      .TouristSpot {
        display: flex;
        padding-bottom: 24px;
      }

      .TouristSpot h1 {
        margin: 1.6px auto;
      }

      .TouristSpot_img img {
        height: 10cm;
      }

      .TouristSpot_img p {
        margin: 0;
      }

      .TouristSpot_note {
        margin-top: 1cm;
        margin-left: 16px;
      }

      .TouristSpot_note h2 {
        margin: 8px auto;
      }

      .TouristSpot_note p {
        margin: 0 auto;
      }
}

</style>