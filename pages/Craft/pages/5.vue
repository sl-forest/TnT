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
            <li><a class="item-link" href="http://localhost:3000">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000">伝統芸能</a></li>
            <li><a class="item-link" href="http://localhost:3000">年間行事</a></li>
            <li><a class="item-link" href="http://localhost:3000">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
        <h1>「伝統工芸品」</h1>
        <h2 class = craft_headline>???</h2>
        <div class="craft">
            <div class = craft01_img>
                <img src="" alt="???">
            </div>
            
            <div class = explanation>
                <p>
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class="craft">
            <div class = craft01_img>
                <img src="" alt="???">
            </div>

            <div class = explanation>
                <p>
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class="craft">
            <div class = craft03_img>
                <img src="" alt="???">
            </div>

            <div class = explanation>
                <p>
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class="craft">
            <div class = craft04_img>
                <img src="" alt="???">
            </div>

            <div class = explanation>
                <p>
                </p>
                <p></p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class="craft">
            <div class = craft05_img>
                <img src="" alt="???">
            </div>

            <div class = explanation>
                <p>
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <!-- 検索ボックス -->
        <form id="form1" action="http://localhost:3000/">
        <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
        <input id="sbtn" type="submit" value="検索" />
        </form>
        
        <ul class="Pagination">
          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
            </svg>
            </a>
            </li>

              <li class="Pagination-Item">
                <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
              </li>
              
              <li class="Pagination-Item">
                <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4"><span>4</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link  isActive" href="http://localhost:3000/Craft/pages/5"><span>5</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/5">
                      <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                          <path stroke-linecap="round" stroke-linejoin="round" d="M13 5l7 7-7 7M5 5l7 7-7 7" />
                      </svg>
                      </a>
                  </li>
              </ul>
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

    /*フォーム全体*/
      #form1{
        margin-left: auto; 
        margin-right: auto;
        position: relative;  /*フォームの相対位置*/	
        max-width: 270px;  /*フォームのサイズ*/
        margin-bottom: 15px; /*フォームの下に余白*/	 	
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

      h1 {
        margin-bottom: 0;
      }

      h2.craft_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 工芸品一覧説明 */
      .craft {
        display: flex;
      }

      .craft p {
        margin: 0;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 工芸品画像 */
      .craft01_img img{
        width: 5cm;
        height: auto;
      }

      .craft03_img img{
        width: 5cm;
        height: auto;
      }
      
      /* ページネーション */
      .Pagination {
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .Pagination-Item-Link {
        width: 45px;
        height: 45px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: none;
        flex-wrap: wrap;
        overflow: hidden;
        background: #fff;
        border: solid 2px #111;
        font-size: 14px;
        color: #111;
        font-weight: bold;
        transition: all 0.15s linear;
      }

      .Pagination-Item-Link-Icon {
        width: 20px;
      }

      .Pagination-Item-Link.isActive {
        background: #111;
        color: #fff;
        pointer-events: none;
      }

      .Pagination-Item-Link:not(.isActive):hover {
        background: #111;
        color: #fff;
      }

      .Pagination > * + * {
        margin-left: 8px;
      }

    }

</style>