<template>

  <div>
    <TheHeader />

    <main>
      <h1>維新ふるさと館</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/Furusatokan-min.jpg" alt="維新ふるさと館">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>9:00～16:30（閉館17:00）</dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>大人（高校生以上） 個人:300円   団体:240円
                <br>
                小人（小・中学生） 個人:150円   団体:120円
                <br>
                ※未就学児は無料。
                <br>
                ※団体は20人以上。
            </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市加治屋町23-1</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>JR鹿児島中央駅から徒歩8分
                <br>
                【車】鹿児島空港から車で45分
                <br>
                桜島フェリーターミナルから車で10分
            </dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://ishinfurusatokan.info/" target="_blank">維新ふるさと館 公式ホームページ</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000317.html" class = "btn" target="_blank">維新ふるさと館 周辺のホテル・旅館</a>

        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}
main {margin: 0 auto;}

h1 {
  margin: 0;
  padding: 8px 0;
  font-family: 'New Tegomin', serif;
}

.TouristSpot_note dl {
  margin: 3px 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  background-color: #e0e2e2;
}

.TouristSpot_note dt {
  flex-shrink: 0;
  text-align: center;
}

.TouristSpot_note dd {
  margin: 0;
  display: flex;
  background-color: #fff;
  padding-left: 1%;
  flex-grow: 1;
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

/* マウスオーバー */
a.btn:hover {
  color: #27acd9;
  background: #fff;
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}
  h1 {text-align: center;}
  .TouristSpot_img {text-align: center;}

  .TouristSpot_img img {
    width: 400px;
    height: auto;
  }

  .TouristSpot_note {margin-top: 16px;}
  .TouristSpot_note h2 {margin: 8px auto;}
  .TouristSpot_note dl {font-size: 15px;}
  .TouristSpot_note dt {width: 20%;}

  .TouristSpot_note dd {
    padding: 2%;
    font-size: 16px;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}
  
  .TouristSpot {
    display: flex;
    padding-bottom: 24px;
  }

  .TouristSpot_img img {
    width: auto;
    height: 345px;
  }

  .TouristSpot_note {
    margin: auto;
    padding-left: 16px;
  }

  .TouristSpot_note h2 {margin: 8px auto;}
  .TouristSpot_note dl {font-size: 18px;}
  .TouristSpot_note dt {width: 20%;}
  .TouristSpot_note dd {width: 14cm;}
  /* マウスオーバー */
  .TouristSpot_note dd a:hover {color: rgb(71, 1, 92);}
}
</style>