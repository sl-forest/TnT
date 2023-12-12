<template>

  <div>
    <TheHeader />

    <main>
      <h1>仙厳園</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/Senganen.jpg" alt="仙厳園">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>9:00～17:00
                <br>
                ※年中無休
                <br>
                ※3月第1日曜日は鹿児島マラソンのため休園
            </dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>庭園+尚古集成館+御殿:高校生以上1,500円、小中学生750円
                <br>
                庭園+尚古集成館:高校生以上1,000円、小中学生500円
            </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市吉野町9700-1</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【バス】各種バス「仙巌園前」バス停下車すぐ
                <br>
                【車】九州自動車道「姶良（あいら）」ICより約40分
            </dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://www.senganen.jp/" target="_blank">仙厳園 公式ホームページ</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000332.html" class = "btn" target="_blank">名勝 仙厳園 周辺のホテル・旅館</a>

        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
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
    font-size: 16px;
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
    width: 15cm;
    margin: 0px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>