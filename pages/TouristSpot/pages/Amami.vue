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

      <h1>奄美大島</h1>

        <div class="TouristSpot">

            <div class = TouristSpot_img>
                <img src="~/assets/img/Amami.jpg" alt="奄美大島">
            </div>
            
            <div class = TouristSpot_note>    
              
              <dl>
                <dt>移動方法</dt>
                <dd>【飛行機】羽田空港、成田空港、伊丹空港、関西空港、福岡空港、鹿児島空港、那覇空港より直行便あり</dd>
                <dd>【船】鹿児島新港より約11時間</dd>
              </dl>

              <a href = "https://search.travel.rakuten.co.jp/ds/hotellist/Japan-Kagoshima-Amami-Amami_Oshima" class = "btn">奄美大島 周辺のホテル・旅館</a>
              <a href = "https://experiences.travel.rakuten.co.jp/destinations/amamioshima-kikaijima-tokunoshima?scid=wi_txp_rakutentravel_travelguide" class = "btn">奄美大島でできること</a>

            </div>

        </div>

        <div>

        </div>

    </main>

  <fotter>

  </fotter>
  
  </div>

</template>

<style>
    /* スマホ向けスタイル */
    @media screen and (max-width: 767px) {
    .TouristSpot_note > dd {
        border: 1px solid #ddd;
        border-top: none;
    }
    .TouristSpot_note > dt,
    .TouristSpot_note > dd {
        text-align: center;
    }
    .TouristSpot_note > dd > ul {
        text-align: left;
    }
}
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
        margin-top: 1.2cm;
        margin-left: 16px;
      }

      .TouristSpot_note h2 {
        margin: 8px auto;
      }

      .TouristSpot_note p {
        margin: 0 auto;
        font-size: 18px;
        margin-top: 8px;
        margin-bottom: 8px;
      }

      .TouristSpot_note dl {
        font-size: 15px;
        margin: 3px 0;
        overflow: hidden;
        display: flex;
        flex-wrap: wrap;
      }

      .TouristSpot_note dt {
        background-color: #e0e2e2;
        width: 20%;
        margin-right: 1%;
        align-items: center;
        justify-content: center;
      }

      .TouristSpot_note dd {
        padding-top: 8px;
        margin: 0px;
        display: flex;
      }

    /* ボタン */
      a.btn {
        display: block;
        text-align: center;
        vertical-align: middle;
        text-decoration: none;
        width: 320px;
        margin-top: 24px;
        padding: 1rem 4rem;
        font-weight: bold;
        border: 2px solid #27acd9;
        background: #27acd9;
        color: #fff;
        border-radius: 100vh;
        transition: 0.5s;
      }
      
      a.btn:hover {
        color: #27acd9;
        background: #fff;
      }
}
</style>