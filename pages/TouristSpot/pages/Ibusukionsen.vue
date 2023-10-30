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

      <h1>指宿温泉 砂むし会館 砂楽</h1>

        <div class="TouristSpot">

            <div class = TouristSpot_img>
                <img src="~/assets/img/Sunamushi.jpg" alt="指宿温泉 砂むし会館 砂楽">
                <a href = "https://travel.rakuten.co.jp/onsen/kagoshima/OK00906.html" class = "btn">指宿温泉の温泉旅館・ホテル一覧</a>
            </div>
            
            <div class = TouristSpot_note>    
              
              <dl>
                <dt>営業時間</dt>
                <dd>8:30～21:00（受付は20:30まで）
                    <br>
                    ※土日・祝日を除いて12:00～13:00は清掃等のため受付休止
                    <br>
                    ※繁忙期は最終受付時間が早まる場合あり
                    <br>
                    ※7月・12月は点検などで臨時休館あり
                </dd>
              </dl>

              <dl>
                <dt>料金</dt>
                <dd>中学生以上1,100円、小学生以下600円
                    <br>
                    ※浴衣込みの料金
                    <br>
                    ※バスタオル貸出は200円、砂むし記念タオルは200円で販売
                    <br>
                    ※砂むし入浴にはタオル（砂よけ用）が必要
                </dd>
              </dl>

              <dl>
                <dt>住所</dt>
                <dd>鹿児島県指宿市湯の浜5-25-18</dd>
              </dl>

              <dl>
                <dt>移動方法</dt>
                <dd>【電車】JR指宿枕崎線「指宿駅」より徒歩約20分
                    <br>
                    【車】JR指宿枕崎線「指宿駅」より約5分
                </dd>
              </dl>

              <dl>
                <dt>詳しく</dt>
                <dd><a href="http://ibusuki-saraku.jp/">砂むし会館 砂楽 公式ページ</a></dd>
              </dl>

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
        margin-top: 0;
        padding-left: 16px;
      }

      .TouristSpot_note h2 {
        margin: 8px auto;
      }

      .TouristSpot_note dl {
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
        display: flex;
        background-color: #fff;
        padding-left: 1%;
        flex-grow: 1;
      }
   
    /* ボタン */
      a.btn {
        display: block;
        text-align: center;
        vertical-align: middle;
        text-decoration: none;
        width: 320px;
        margin-top: 18px;
        margin-left: 60px;
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