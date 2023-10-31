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

        <div class = "box">
          <ul class="timeline">
            <li>
                <p class="timeline-date">1827年（1歳）</p>
                <div class="timeline-content">
                  <h3>鹿児島城下・下鍛冶屋しもかじや町に生まれる。(幼名、小吉)</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1844年（18歳）</p>
                <div class="timeline-content">
                  <h3>藩に出仕し、郡方書役助こおりかたかきやくすけとなる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1850年（24歳）</p>
                <div class="timeline-content">
                  <h3>島津斉彬しまづなりあきらに農政に関する意見書を提出する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1854年（28歳）</p>
                <div class="timeline-content">
                  <h3>斉彬のお供として江戸へ向かう。庭方役にわかたやくに昇進する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1859年（33歳）</p>
                <div class="timeline-content">
                  <h3>奄美大島で潜居生活を始める。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1862年（36歳）</p>
                <div class="timeline-content">
                  <h3>鹿児島に帰国するも、再び流刑に。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1864年（38歳）</p>
                <div class="timeline-content">
                  <h3>禁門の変で薩摩軍を指揮する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1866年（40歳）</p>
                <div class="timeline-content">
                  <h3>薩長同盟を結ぶ。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1868年（42歳）</p>
                <div class="timeline-content">
                  <h3>鳥羽伏見の戦い。江戸無血開城。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1871年（45歳）</p>
                <div class="timeline-content">
                  <h3>新政府の参議となる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1873年（47歳）</p>
                <div class="timeline-content">
                  <h3>征韓論騒動が起こり、敗れて鹿児島へ帰国する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1874年（48歳）</p>
                <div class="timeline-content">
                  <h3>私学校を作る。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1877年（51歳）</p>
                <div class="timeline-content">
                  <h3>西南戦争・城山にて自決する。</h3>
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