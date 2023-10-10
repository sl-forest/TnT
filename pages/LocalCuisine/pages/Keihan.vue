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
      <h1>鶏飯（けいはん）</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Keihan.jpeg" alt="鶏飯">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>奄美地域</p>
                <h2>食材</h2>
                <p>米、鶏肉、干ししいたけ、卵、パパイヤの味噌漬け、ねぎ、みかんの皮、のり</p>
                <h2>歴史</h2>
                <p>奄美群島が薩摩藩の支配下に置かれていた時代、鹿児島本土からやってくる役人たちの威圧的な態度を少しでも和らげるためにつくられたのがはじまりだといわれてる。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（4人分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>米</li>
                <li>320g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>水</li>
                <li>480cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>鶏ガラ</li>
                <li>240g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>水</li>
                <li>800cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>しょうが（薄切り）</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>鶏ささみ</li>
                <li>60g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】塩</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】清酒</li>
                <li>小さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】淡口醤油</li>
                <li>大さじ1</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】本みりん</li>
                <li>小さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>干ししいたけ</li>
                <li>8g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>干ししいたけ戻し汁</li>
                <li>80cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【B】 淡口醤油</li>
                <li>小さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【B】 本みりん</li>
                <li>小さじ1</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>卵</li>
                <li>2個</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【C】 砂糖（上白糖）</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【C】 塩</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>さやいんげん</li>
                <li>80g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>塩</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>葉ねぎ</li>
                <li>20g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>パパイヤの味噌漬け</li>
                <li>40g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>みかんの皮</li>
                <li>少々</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>焼きのり</li>
                <li>少々</li>
              </ul>
            </li>

          </ul>

              <h3>作り方</h3>

              <ul class = "LocalCuisine_make">
                
                <li>
                  <div class = "num">1</div>
                  <div class = "text">
                    （下ごしらえ）干ししいたけは洗って水で戻し、戻した汁はだし汁として使う。
                    米は炊く30分前にといで、分量の水に浸しておく。
                    鶏ガラはよく洗って余分なものを取り除く。
                    葉ねぎ、パパイヤの味噌漬け、みかんの皮はみじん切りに、焼きのりは千切りにする。
                  </div>
                </li>

                <li>
                  <div class = "num">2</div>
                  <div class = "text">
                    米は普通に炊く。
                  </div>
                </li>

                <li>
                  <div class = "num">3</div>
                  <div class = "text">
                    	水（800cc）をはった鍋に、鶏ガラ、皮付きのしょうがを入れて火にかける。
                  </div>
                </li>

                <li>
                  <div class = "num">4</div>
                  <div class = "text">
                    アクを取り除きながら弱火で1時間くらい煮たら、鶏ささみを入れてゆでる。
                  </div>
                </li>

                <li>
                  <div class = "num">5</div>
                  <div class = "text">
                    	鶏ささみは取り出して細かく裂き、だし汁はこし、【A】を入れてスープとして使う。
                  </div>
                </li>

                <li>
                  <div class = "num">6</div>
                  <div class = "text">
                    	【B】と干ししいたけの戻し汁を火にかけ、千切りにしたしいたけを煮含める。
                  </div>
                </li>

                <li>
                  <div class = "num">7</div>
                  <div class = "text">
                    さやいんげんは塩ゆでし、細めの千切りにする。
                  </div>
                </li>

                <li>
                  <div class = "num">8</div>
                  <div class = "text">
                    溶いた卵に【C】を混ぜフライパンで薄く焼き、錦糸卵を作る。
                  </div>
                </li>

                <li>
                  <div class = "num">9</div>
                  <div class = "text">
                    	鶏ささみ、しいたけ、錦糸卵、さやいんげん、葉ねぎ、パパイヤ漬け、みかんの皮、のりを皿にきれいに盛り付ける。
                  </div>
                </li>

                <li>
                  <div class = "num">10</div>
                  <div class = "text">
                    ごはんを茶碗に盛り、8をかたち良くのせて5のスープをたっぷりかけていただく。
                  </div>
                </li>
              
              </ul>

              <div class = "offer">
                <p>レシピ提供元名 : 「郷土食の料理集」（公益社団法人　全国学校栄養士協議会）</p>
                <p>※レシピは地域・家庭によって違いがあります。</p>
              </div>

        </div>
    </main>

        <!-- 検索ボックス -->
        <form id="form1" action="http://localhost:3000/">
        <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
        <input id="sbtn" type="submit" value="検索" />
        </form>

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

    /*フォーム全体*/
      #form1{
        margin-top: 16px;
        margin-left: auto; 
        margin-right: auto;
        position: relative;  /*フォームの相対位置*/	
        max-width: 270px;  /*フォームのサイズ*/
        margin-bottom: 16px; /*フォームの下に余白*/	 	
      }

    /*検索ボックス*/
      #sbox{
        left: 0;  /*検索ボタンの位置調整*/
        top: 13.5px; 	/*検索ボタンの位置調整*/
        outline: 0;  /*クリック時の青い枠線消す*/	
        height: 35px;  /*検索ボックスの高さ*/	
        padding: 0 10px; /*テキスト位置調整*/	 
        border-radius: 2px 0 0 2px;  /*検索ボックスの角を丸める*/		
        background:#eee;  /*検索ボックスの背景カラー*/		
      }

    /*検索ボタン*/
      #sbtn{
        width:70px; /*検索ボタンの横幅*/ 
        height:40px;  /*検索ボタンの縦幅*/ 
        border-radius:0 2px 2px 0;  /*検索ボタンの角を丸める*/ 
        background:#7fbfff; /*検索ボタンの背景カラー*/ 
        border:none;  /*検索ボタンの枠線を消す*/ 
        color:#fff; /*検索ボタンのテキストカラー*/ 
        font-weight:bold; /*検索ボタンのテキスト太字*/ 
        font-size:16px; /*検索ボタンのフォントサイズ*/ 
      }

    /*検索ボタンマウスオーバー時*/
      #sbtn:hover{
        color:#666; /*検索ボタンマウスオーバー時のフォントカラー*/ 
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
        margin-top: 2.4cm;
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