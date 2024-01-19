<template>

  <div>
    <TheHeader />

    <main>
      <h1>天文館</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/TenmonKan.jpg" alt="天文館">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業日</dt>
            <dd>通年</dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市東千石町</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【市電「天文館通」下車</dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://www.kagoshima-yokanavi.jp/spot?rta%5B%5D=3&rtd=&q=&lat=&lng=&st=acs&vw=tile" target="_blank">天文館エリアの観光スポット一覧</a></dd>
          </dl>
          <a href = "https://search.travel.rakuten.co.jp/ds/hotellist/Japan-Kagoshima-Kagoshima-Tenmonkan-review?s_kwcid=paidsearch&gclid=EAIaIQobChMIoofh8ICLggMVagp7Bx2LDQVLEAAYAyAAEgIpz_D_BwE&gclsrc=aw.ds" class = "btn" target="_blank">天文館 周辺のホテル・旅館</a>

        </div>

      </div>
    </main>
    <TheFooter />
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

  .TouristSpot_img img {height: 6cm;}

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
  main {max-width: 1024px;}
  
  .TouristSpot {
    display: flex;
    padding-bottom: 24px;
  }

  .TouristSpot h1 {Margin: 1.6px auto;}

  .TouristSpot_img img {height: 8cm;}

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