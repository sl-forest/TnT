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
      <h1>鳥刺し</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Torisashi02.jpeg" alt="鳥刺し">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>鶏肉</p>
                <h2>歴史</h2>
                <p>鹿児島県では、江戸時代から薩摩武士たちが士風高揚のため、盛んに闘鶏をおこなっており、その際に負けた鶏をその場でしめて食べる習慣があった。闘鶏が禁止された後も、各家庭で鶏が飼われ、来客がある時や祝いの席のために鶏をしめて調理し食べていたという。このように鹿児島県においては、古くから鶏肉を使った料理が身近でにあったことから、鶏肉を刺身で食べる「鶏刺し」が根づいたと考えられてる。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>鶏刺し用鶏肉（もも・ささみ・むね肉）</li>
                <li>150g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>玉ねぎ</li>
                <li>30g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>ねぎ</li>
                <li>5g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>しょうが</li>
                <li>お好みで</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>にんにく</li>
                <li>お好みで</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>青じそ</li>
                <li>お好みで</li>
              </ul>
            </li>

          </ul>

              <h3>作り方</h3>

              <ul class = "LocalCuisine_make">
                
                <li>
                  <div class = "num">1</div>
                  <div class = "text">
                    鶏刺し用の新鮮な鶏肉を用意する。
                  </div>
                </li>

                <li>
                  <div class = "num">2</div>
                  <div class = "text">
                    バーナーなどで皮目をあぶり、表面の色が変わったら火を止める。（中は生のまま）
                  </div>
                </li>

                <li>
                  <div class = "num">3</div>
                  <div class = "text">
                    	3mm幅に皮目から切る。肉の繊維の方向を見て繊維を断ち切るようにくらいの刺身に切る。
                  </div>
                </li>

                <li>
                  <div class = "num">4</div>
                  <div class = "text">
                    青じそを敷き部位ごとに盛り付け玉ねぎはスライス、ネギは小口切り。しょうがニンニクはすりおろして一緒に盛り付け、好みで醤油やポン酢で味わう。
                  </div>
                </li>

              </ul>

              <div class = "offer">
                <p>レシピ提供元名 : 株式会社Table of Smile</p>
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
        height: 12cm;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 1.8cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 8px auto;
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
</style>