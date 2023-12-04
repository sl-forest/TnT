<template>

  <div>
    <TheHeader />

    <main>
      <h1>開聞岳</h1>
        <div class="TouristSpot">

          <div class = TouristSpot_img>
            <img src="~/assets/img/KaimonDake.jpg" alt="開聞岳">
          </div>
          
          <div class = TouristSpot_note>
            <dl>
              <dt>移動方法</dt>
              <dd>【電車】JR指宿枕崎線「開聞」駅より徒歩約20分で登山口</dd>
            </dl>

            <dl>
              <dt>詳しく</dt>
              <dd><a href = "https://www.ibusuki.or.jp/tourism/view/kaimondake/" target=”_blank”>開聞岳（いぶすき観光ネット）</a></dd>
            </dl>target="_blank"
            <a href="https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000479.html" class = "btn" target="_blank">開聞岳 周辺のホテル・旅館</a>
          </div>

        </div>
    </main>
    <TheFooter />
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
        margin: auto;
        padding-left: 16px;
      }

      .TouristSpot_note h2 {
        margin: 8px auto;
      }

      .TouristSpot_note dl {
        font-size: 18px;
        margin: 3px 0;
        overflow: hidden;
        display: flex;
        align-items: center;
        background-color: #e0e2e2;
      }

      .TouristSpot_note dt {
        vertical-align: middle;
        flex-shrink: 0;
        text-align: center;
        width: 20%;
      }

      .TouristSpot_note dd {
        width: 13.5cm;
        margin: 0px;
        display: flex;
        background-color: #fff;
        padding-left: 1%;
        flex-grow: 1;
      }

      .TouristSpot_note dd a {
        text-decoration: none;
        color: blue;
      }

      .TouristSpot_note dd a:hover {
        color: rgb(71, 1, 92);
      }

    /* ボタン */
      a.btn {
        display: block;
        text-align: center;
        text-decoration: none;
        width: 320px;
        margin: 18px auto;
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