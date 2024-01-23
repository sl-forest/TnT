<template>

  <div>
    <TheHeader />

    <main>
      <h1>雄川の滝</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/OgawaTaki.jpg" alt="雄川の滝">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>見学自由
                <br>
                ※天候などにより立ち入り禁止になる場合あり
            </dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>無料</dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県南大隅町根占</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【車】鹿児島空港から約1時間45分</dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://www.kagoshima-kankou.com/guide/51100" target="_blank">雄川の滝（鹿児島県観光サイト）</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/yado/kagoshima/kanoya.html" class = "btn" target="_blank">雄川の滝 周辺のホテル・旅館</a>

        </div>

      </div>
    </main>
    <TheFooter />>
  </div>

</template>

<style>
/* 共通 */
main {margin: 0 auto;}

.TouristSpot_note dd a {
  text-decoration: none;
  color: blue;
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
  h1 {
    margin: 16px 0;
    text-align: center;
  }

  .TouristSpot h1 {margin: 1.6px auto;}

  .TouristSpot_img {text-align: center;}

  .TouristSpot_img img {height: 8cm;}

  .TouristSpot_note {margin-top: 16px;}

  .TouristSpot_note h2 {margin: 8px auto;}

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
    font-size: 16px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .TouristSpot {
    display: flex;
    padding-bottom: 24px;
  }

  .TouristSpot h1 {margin: 1.6px auto;}

  .TouristSpot_img img {height: 10cm;}

  .TouristSpot_note {
    margin: auto;
    padding-left: 16px;
  }

  .TouristSpot_note h2 {margin: 8px auto;}

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

  .TouristSpot_note dd a:hover {color: rgb(71, 1, 92);}
}
</style>