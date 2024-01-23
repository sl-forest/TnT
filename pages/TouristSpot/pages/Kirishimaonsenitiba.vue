<template>

  <div>
    <TheHeader />

    <main>
      <h1>霧島温泉市場</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/Itiba.jpg" alt="霧島温泉市場">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>8:30～18:00（店舗により異なる）
                <br>
                ※不定休
            </dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>足湯:大人100円、小学生以下50円（タオル貸出付き）
            </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県霧島市牧園町高千穂3878-114</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【バス】鹿児島空港から路線バス霧島いわさきホテル行きで約30分、「丸尾」バス停下車、徒歩約1分
                <br>
                【車】JR肥薩線「霧島温泉」駅より車で約20分、九州自動車道「横川」ICより車で約35分
            </dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://kirishima-marche.com/" target="_blank">霧島温泉市場 公式ページ</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/onsen/kagoshima/OK00896.html" class = "btn" target="_blank">霧島温泉の温泉旅館・ホテル一覧</a>

        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}       /* 要素の外側余白 */

main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;            /* 要素の外側余白 */
  padding: 8px 0;       /* 要素の内側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}


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
  body {margin-top: 18%;}  /* 要素の外側上余白 */

  h1 {text-align: center;} /* 左右の中央揃え */

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
    margin: 0;
    padding: 2%;
    font-size: 15px;
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
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }

  .TouristSpot_note dd a:hover {color: rgb(71, 1, 92);}
}
</style>