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
            <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>

      <h1>旧集成館機械工場（尚古集成館）</h1>

        <div class="WorldHeritage">

            <div class = WorldHeritage_img>
                <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
            </div>
            
            <div class = WorldHeritage_note>   

              <dl>
                <dt>営業日</dt>
                <dd>通年</dd>
              </dl>

              <dl>
                <dt>営業時間</dt>
                <dd>8:30～17:30</dd>
              </dl>

              <dl>
                <dt>休日</dt>
                <dd>
                    年中無休
                    <br>
                    ※かごしまマラソン開催日を除く
                </dd>
              </dl>

              <dl>
                <dt>料金</dt>
                <dd>
                  個人 : 大人・高校生以上1000円,小中学生500円
                  <br>
                  団体（20名以上）: 大人・高校生以上900円, 小中学生450円
                  <br>
                  団体（100名以上）: 大人・高校生以上850円, 小中学生400円
                  <br>
                  ※乳幼児無料
                  </dd>
              </dl>

              <dl>
                <dt>住所</dt>
                <dd>鹿児島県鹿児島市吉野町磯</dd>
              </dl>

              <dl>
                <dt>移動方法</dt>
                <dd>
                    【車】鹿児島中央駅から20分
                    <br>
                    【車】鹿児島空港から（姶良IC～国道10号経由】で40分
                    <br>
                    【バス】鹿児島中央駅からカゴシマシティビュー・まち巡りバスで約３０～５０分「仙巖園前」バス停下車すぐ
                </dd>
              </dl>

              <dl>
                <dt>詳しくは</dt>
                <dd><a href="https://www.shuseikan.jp/heritage/heritage02.html">尚古集成館 公式ホームページ</a></dd>
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
      .WorldHeritage_note > dd {
        border: 1px solid #ddd;
        border-top: none;
      }

      .WorldHeritage_note > dt,
      .WorldHeritage_note > dd {
        text-align: center;
      }

      .WorldHeritage_note > dd > ul {
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
      
      .WorldHeritage {
        display: flex;
        padding-bottom: 24px;
      }

      .WorldHeritage h1 {
        margin: 1.6px auto;
      }

      .WorldHeritage_img img {
        height: 9.5cm;
      }

      .WorldHeritage_img p {
        margin: 0;
      }

      .WorldHeritage_note {
        margin-top: 0;
        padding-left: 16px;
      }

      .WorldHeritage_note h2 {
        margin: 8px auto;
      }

      .WorldHeritage_note dl {
        font-size: 15px;
        margin: 3px 0;
        overflow: hidden;
        display: flex;
        align-items: center;
        background-color: #e0e2e2;
      }

      .WorldHeritage_note dt {
        vertical-align: middle;
        flex-shrink: 0;
        text-align: center;
        width: 20%;
      }

      .WorldHeritage_note dd {
        width: 15cm;
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
        margin-left: 65px;
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