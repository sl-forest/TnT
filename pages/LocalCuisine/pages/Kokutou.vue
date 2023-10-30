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
      <h1>黒糖</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Kokutou.jpg" alt="黒糖">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>奄美地域</p>
                <h2>食材</h2>
                <p>さとうきび</p>
                <h2>歴史</h2>
                <p>元禄時代（１６８８年）、日本に黒糖（黒砂糖）は伝わった。江戸時代より沖縄、奄美大島、種子島などで生産されており、沖縄で黒糖（黒砂糖）は“ヌチグスイ（命薬）”と呼ばれ薬として飲まれていたこともある。</p>
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

    /*郷土料理説明*/
      .LocalCuisine {
        display: flex;
        padding-bottom: 24px;
      }

      .LocalCuisine h1 {
        margin: 1.6px auto;
      }

      .LocalCuisine_img img {
        height: 10cm;
      }

      .LocalCuisine_img p {
        margin: 0;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 1cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 0 auto;
      }
    }
</style>