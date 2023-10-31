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
      <h1>がね</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Gane.jpg" alt="がね">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>さつまいも、人参、ニラ、小麦粉</p>
                <h2>歴史</h2>
                <p>「がね」は、さつまいもや野菜を太めの千切りにし、衣をつけて揚げる料理。その見た目が“かに（鹿児島弁でがねという）”に似ていることからこの名がついた。</p>
                <p>砂糖を多く入れ甘めな味付けが特徴で地域により具材や衣の材料は違う。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（8～10個分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>さつまいも</li>
                <li>200g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>人参</li>
                <li>50g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>ニラ</li>
                <li>30g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】小麦粉</li>
                <li>100g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】もち米粉</li>
                <li>50g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】砂糖</li>
                <li>40g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】卵</li>
                <li>1個</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】淡口醤油</li>
                <li>大さじ1.5</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】塩</li>
                <li>ふたつまみ</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】水</li>
                <li>80cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>油</li>
                <li>適量</li>
              </ul>
            </li>

          </ul>

              <h3>作り方</h3>

              <ul class = "LocalCuisine_make">
                
                <li>
                  <div class = "num">1</div>
                  <div class = "text">
                    さつまいもは薄く皮を剥き（ところどころ皮を残す）、5mm角×7～8cmの細切りにする。
                    ボウルに水を張り、さつまいもが完全に浸るようにさらしてざるに開ける。
                    人参は薄く皮を剥き、さつまいもより短めの2～3cmに切る。ニラは7～8cmの長さに切る。
                  </div>
                </li>

                <li>
                  <div class = "num">2</div>
                  <div class = "text">
                    ボウルに1と水以外の材料を加えながら衣が具にまとわりつく感じになるまで混ぜる。
                  </div>
                </li>

                <li>
                  <div class = "num">3</div>
                  <div class = "text">
                    鍋に油を3cm以上の深さになるように入れて、170度になるように熱する。（臭みが取れる）
                  </div>
                </li>

                <li>
                  <div class = "num">4</div>
                  <div class = "text">
                    木杓子で具をすくい、横長にカニの姿のようにかたちをととのえる。
                    菜箸で向こう側に押すように鍋に落とし、2、3分でひっくり返し、さつまいもの甘い匂いがしてきて全体がきつね色になったら揚げ上がり。
                    バットにキッチンペーパーを敷き、立てて並べると油の切れが良い。
                  </div>
                </li>

              </ul>

              <div class = "offer">
                <p>レシピ提供元名 : NPO法人霧島食育研究会</p>
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
        margin-top: 0.6cm;
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

    /*提供*/
      .offer {
        margin: 16px 0px 0px 0px;
        text-align: right;
      }

      .offer p {
        margin: 4px 0px 0px 0px;
        font-size: 80%;
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