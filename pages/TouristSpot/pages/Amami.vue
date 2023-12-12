<template>

  <div>
    <TheHeader />

    <main>
      <h1>奄美大島</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/Amami.jpg" alt="奄美大島">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>移動方法</dt>
            <dd>【飛行機】羽田空港、成田空港、伊丹空港、関西空港、福岡空港、鹿児島空港、那覇空港より直行便あり
              <br>
              【船】鹿児島新港より約11時間
            </dd>
          </dl>

          <a href = "https://search.travel.rakuten.co.jp/ds/hotellist/Japan-Kagoshima-Amami-Amami_Oshima" class = "btn" target="_blank">奄美大島 周辺のホテル・旅館</a>
          <a href = "https://experiences.travel.rakuten.co.jp/destinations/amamioshima-kikaijima-tokunoshima?scid=wi_txp_rakutentravel_travelguide" class = "btn" target="_blank">奄美大島でできること</a>

        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
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
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {

  main {
    margin: 0 auto;
  }

  h1 {
    margin: 16px 0;
    text-align: center;
  }
  
  .TouristSpot {
    padding-bottom: 16px;
  }

  .TouristSpot h1 {
    margin: 1.6px auto;
  }

  .TouristSpot_img {
    text-align: center;
  }

  .TouristSpot_img img {
    height: 8cm;
  }

  .TouristSpot_img p {
    margin: 0;
  }

  .TouristSpot_note {
    margin-top: 16px;
  }

  .TouristSpot_note h2 {
    margin: 8px auto;
  }

  .TouristSpot_note dl {
    display: table;
    width: 100%;
    font-size: 15px;
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
    margin: 0px;
    padding: 2%;
    font-size: 14px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
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
    width: 14cm;
    margin: 0px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>