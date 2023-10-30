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
      <h1>油ゾーメン</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Zomen.jpg" alt="油ゾーメン">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>奄美地域</p>
                <h2>食材</h2>
                <p>豚肉、そうめん、ニラ、いりこ、だし汁</p>
                <h2>歴史</h2>
                <p>薩摩藩統治時代に薩摩から持ち込まれ、乾麺で保存がきくことから奄美地域でよく食べられるようになったのではないかという説があるが、定かではない。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（4人分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>塩豚肉（豚もも肉でも良い）</li>
                <li>120g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>そうめん</li>
                <li>180g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>ニラ</li>
                <li>180g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>いりこ</li>
                <li>12g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>サラダ油</li>
                <li>大さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>だし汁</li>
                <li>2cup</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>醤油</li>
                <li>大さじ1・1/2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>塩、こしょう</li>
                <li>各少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>ごま油</li>
                <li>小さじ2</li>
              </ul>
            </li>

          </ul>

              <h3>作り方</h3>

              <ul class = "LocalCuisine_make">
                
                <li>
                  <div class = "num">1</div>
                  <div class = "text">
                    ［塩豚肉のつくり方］三枚肉のかたまり（300g）の表面全体に塩をすりこむようにしてまぶす。
                    ビニール袋に入れて冷蔵庫で保存する（1週間程度保存できる）。
                  </div>
                </li>

                <li>
                  <div class = "num">2</div>
                  <div class = "text">
                    豚肉は熱湯で三度塩抜きをする。
                  </div>
                </li>

                <li>
                  <div class = "num">3</div>
                  <div class = "text">
                    豚肉は細切りにしておく。
                  </div>
                </li>

                <li>
                  <div class = "num">4</div>
                  <div class = "text">
                    そうめんは少しかためにゆでて、ざるに上げておく。
                  </div>
                </li>

                <li>
                  <div class = "num">5</div>
                  <div class = "text">
                    ニラは2cmの長さに切っておく。
                  </div>
                </li>

                <li>
                  <div class = "num">6</div>
                  <div class = "text">
                    中華鍋に油を引き、豚肉を炒める。
                  </div>
                </li>

                <li>
                  <div class = "num">7</div>
                  <div class = "text">
                    6にいりことそうめんを入れ、混ぜながら炒める。
                  </div>
                </li>

                <li>
                  <div class = "num">8</div>
                  <div class = "text">
                    7にだし汁をまわし入れる。
                  </div>
                </li>

                <li>
                  <div class = "num">9</div>
                  <div class = "text">
                    8に醤油を回し入れる。
                  </div>
                </li>

                <li>
                  <div class = "num">10</div>
                  <div class = "text">
                    9に塩、こしょうをふり、ニラを入れ混ぜ、最後にごま油を入れる。
                  </div>
                </li>
                
              </ul>

              <div class = "offer">
                <p>レシピ提供元名 : 「郷土の味」（鹿児島県食生活改善推進員連絡協議会）</p>
                <p>※レシピは地域・家庭によって違いがあります。</p>
              </div>

        </div>
    </main>

  <fotter>

  </fotter>
  
  </div>

</template>

<style>
    /* スマホ向けスタイル */

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

    /*郷土料理説明*/
      .LocalCuisine {
        display: flex;
        padding-bottom: 24px;
      }

      .LocalCuisine h1 {
        margin: 1.6px auto;
      }

      .LocalCuisine_img img {
        height: 10cm;
      }

      .LocalCuisine_img p {
        margin: 0;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 1cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 0 auto;
      }

      .recipe {
        background: #d2e7f3;
        padding: 24px;
      }

      .recipe h3 {
        margin: 0;
        padding: 0;
        border-bottom: 1px solid #1b1b1b;
      }

      .list {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 6px;
        border-bottom: 1px solid #9e9595;
      }

      .list_last {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 64px;
      }

    /*作り方*/
      .LocalCuisine_make {
        list-style: none;
        margin: 0;
        font-size: 1em;
        padding: 0;
      }

      .LocalCuisine_make li {
        display: table;
        padding: 16px 0;
        border-bottom: 1px solid #9e9595;
      }

      .num {
        display: inline-block;
        font-size: 1.714em;
        width: 40px;
        margin-top: -5px;
        padding-right: 10px;
      }

      .text {
        display: table-cell;
        vertical-align: top;
        width: 100%;
      }
    }
    
    /*提供*/
      .offer {
        margin: 16px 0px 0px 0px;
        text-align: right;
      }

      .offer p {
        margin: 4px 0px 0px 0px;
        font-size: 80%;
      }
</style>