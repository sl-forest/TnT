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
        
        <h1>年表</h1>

        <div class="box">
          <ul class="timeline">
            <li>
              <p class="timeline-date">1836年（0歳）</p>
              <div class="timeline-content">
                <h3>篤姫生まれる</h3>
              </div>
            </li>

            <li>
              <p class="timeline-date">1853年（17歳）</p>
              <div class="timeline-content">
                <h3>篤姫が島津斉彬なりあきらの養女となる</h3>
              </div>
            </li>

            <li>
              <p class="timeline-date">1856年（20歳）</p>
              <div class="timeline-content">
                <h3>篤姫が徳川家定の御台所（みだいどころ。正妻）となる</h3>
              </div>
            </li>

            <li>
              <p class="timeline-date">1858年（22歳）</p>
              <div class="timeline-content">
                <h3>徳川家定、島津斉彬、あいついで亡くなる</h3>
              </div>
            </li>

            <li>
              <p class="timeline-date">1867年（31歳）</p>
              <div class="timeline-content">
                <h3>大政奉還。江戸城無血開城</h3>
              </div>
            </li>

            <li>
              <p class="timeline-date">1883年（47歳）</p>
              <div class="timeline-content">
                <h3>篤姫亡くなる</h3>
              </div>
            </li>
          </ul>
        </div>

    </main>
</div>

</template>

<style>
    /* スマホ向けスタイル */
    .timeline {
        list-style: none;
      }
      
      .timeline > li {
        margin-bottom: 60px;
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
      
    /* 年表 */
      .timeline > li {
        overflow: hidden;
        margin: 0;
        position: relative;
      }
      
      .timeline-date {
        width: 135px;
        float: left;
        margin-top: 20px;
      }
      
      .timeline-content {
        width: 75%;
        float: left;
        border-left: 3px #e5e5d1 solid;
        padding-left: 30px;
      }
      
      .timeline-content:before {
        content: '';
        width: 12px;
        height: 12px;
        background: #6fc173;
        position: absolute;
        left: 130px;
        top: 24px;
        border-radius: 100%;
      } 
    }

</style>