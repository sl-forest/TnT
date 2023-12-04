<template>

  <div>
    <TheHeader />

    <main>
      <h1>曾木の滝</h1>
        <div class="TouristSpot">

          <div class = TouristSpot_img>
            <img src="~/assets/img/SogiTaki.jpg" alt="曾木の滝">
          </div>
          
          <div class = TouristSpot_note>    
            
            <dl>
              <dt>営業時間</dt>
              <dd>散策自由
                  <br>
                  ※紅葉の見頃は11月下旬～12月上旬、桜の見頃は3月下旬～4月上旬
              </dd>
            </dl>

            <dl>
              <dt>料金</dt>
              <dd>無料</dd>
            </dl>

            <dl>
              <dt>住所</dt>
              <dd>鹿児島県伊佐市大口宮人628-41</dd>
            </dl>

            <dl>
              <dt>移動方法</dt>
              <dd>【電車・車】九州新幹線「出水」駅より車で約60分
                  <br>
                  【車】九州自動車道「栗野」ICより約30分
              </dd>
            </dl>

            <dl>
              <dt>詳しく</dt>
              <dd><a href="https://soginotaki.kagoshima.jp/soginotaki" target="_blank">曽木の滝 観光ガイド</a></dd>
            </dl>
            <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000307.html" class = "btn" target="_blank">曾木の滝 周辺のホテル・旅館</a>

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
        width: 14.5cm;
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
        margin: 24px auto;
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