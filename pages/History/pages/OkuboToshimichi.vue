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
              
              <p class="timeline-date">1830年（1歳）</p>
                <div class="timeline-content">
                    <h3>鹿児島城下の高麗町に生まれる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1846年（18歳）</p>
                <div class="timeline-content">
                    <h3>薩摩藩の記録所書役となる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1850年（22歳）</p>
                <div class="timeline-content">
                    <h3>お由羅騒動で免職・謹慎の処分を受ける。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1853年（25歳）</p>
                <div class="timeline-content">
                    <h3>謹慎を解かれる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1866年（38歳）</p>
                <div class="timeline-content">
                    <h3>第二次長州征討の出兵拒否。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1869年（41歳）</p>
                <div class="timeline-content">
                    <h3>明治政府の参議に就任。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1871年（43歳）</p>
                <div class="timeline-content">
                    <h3>岩倉使節団の一員として、欧米12カ国を歴訪。大蔵卿に就任。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1873年（45歳）</p>
                <div class="timeline-content">
                    <h3>帰国。征韓論で西郷らと対立。内務卿に就任。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1877年（48歳）</p>
                <div class="timeline-content">
                    <h3>西南戦争の指揮を執る。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1878年（49歳）</p>
                <div class="timeline-content">
                    <h3>紀尾井坂で襲撃され、死亡。</h3>
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