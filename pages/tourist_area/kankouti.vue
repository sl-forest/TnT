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
            <li><a class="item-link" href="#">工芸品</a></li>
            <li><a class="item-link" href="#">歴史</a></li>
            <li><a class="item-link" href="#">郷土料理</a></li>
            <li><a class="item-link" href="#">伝統芸能</a></li>
            <li><a class="item-link" href="#">年間行事</a></li>
            <li><a class="item-link" href="#">観光地</a></li>
            <li><a class="item-link" href="#">世界遺産</a></li>
          </ul>
        </div>
      </nav>
      
      <!-- 検索ボックス -->
      <form id="form1" action="http://localhost:3000/about">
      <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
      <input id="sbtn" type="submit" value="検索" />
      </form>

    </header>

    <main>
        <h1>「おすすめの観光地一覧」</h1>
        <h2 class = tourist_area_headline>桜島</h2>
        <div class=" craft01 ">
            <div class = tourist_area01_img>
                <img src="~/assets/img/sakurajima.jpg" alt="桜島">
            </div>
            
            <div class = explanation01>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = tourist_area_headline>???</h2>
        <div class=" tourist_area02 ">
            <div class = tourist_area01_img>
                <img src="" alt="???">
            </div>

            <div class = explanation02>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = tourist_area_headline>???</h2>
        <div class=" tourist_area03 ">
            <div class = tourist_area03_img>
                <img src="" alt="???">
            </div>

            <div class = explanation03>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = tourist_area_headline>???</h2>
        <div class=" tourist_area04 ">
            <div class = tourist_area04_img>
                <img src="" alt="???">
            </div>

            <div class = explanation04>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = tourist_area_headline>???</h2>
        <div class=" tourist_area05 ">
            <div class = tourist_area_img>
                <img src="" alt="???">
            </div>

            <div class = explanation05>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>
    </main>

    <fotter>

    </fotter>
    
  </div>
</template>

<style>
    /* スマホ向けスタイル */
    main {
    

    }

    /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
      main {
        max-width: 1024px;
        margin: 0 auto;
      }


    }

    header {
    display: flex;  /*ヘッダーの下の要素を並列に*/
    height: 80px; /*ヘッダーの高さ*/
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
    margin-top: 5px;  /*ロゴの位置調整*/
    margin-bottom: 5px; /*ロゴの位置調整*/
    margin-left: 15px;  /*ロゴの位置調整*/
    margin-right: 15px; /*ロゴの位置調整*/
  }

  .logo a img {
    width: 65px;  /*ロゴ画像の幅調整*/
    height: 65px; /*ロゴ画像の高さ調整*/
    padding-top: 1.5px; /*ロゴの位置調整*/
  }
 
  .item ul {
    display: inline-block;
    margin-top: 25px;
}

  ul {
    padding-left: 24px;
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
  position:relative;  /*フォームの相対位置*/	
  max-width:270px;  /*フォームのサイズ*/
  margin-bottom:15px; /*フォームの下に余白*/	 	
  }

/*検索ボックス*/
  #sbox{
  position:absolute;  /*フォームの絶対位置*/	
  left: 0;  /*検索ボタンの位置調整*/
  top: 13.5px; 	/*検索ボタンの位置調整*/
  outline:0;  /*クリック時の青い枠線消す*/	
  height:50px;  /*検索ボックスの高さ*/	
  padding:0 10px; /*テキスト位置調整*/	 
  border-radius:2px 0 0 2px;  /*検索ボックスの角を丸める*/		
  background:#eee;  /*検索ボックスの背景カラー*/		
  }

/*検索ボタン*/
  #sbtn{
  width:70px; /*検索ボタンの横幅*/ 
  height:50px;  /*検索ボタンの縦幅*/ 
  position:absolute;  /*検索ボタンの絶対位置*/  
  left:190px; /*検索ボタンの位置調整*/  
  top: 15.5px;  /*検索ボタンの位置調整*/
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

  body {
    margin: 20px;
    padding: 0;
  }

  h1 {
    margin-bottom: 0;
  }

  h2.tourist_area_headline {
    margin: 0;
    padding-top: 8px;
    border-top: 2px solid #d5d4c3;
  }
  
  .tourist_area01 {
    display: flex;
  }

  .tourist_area01_img {
    width: 5cm;
    margin: 0;
    padding: 0;
  }

  .tourist_area01 img {
    width: 5cm;
    height: auto;
  }

  .tourist_area01 p {
    padding: 0, 0, 0, 20;
    margin: 0;
  }

  .explanation01 {
    padding-top: 24px;
    padding-left: 16px;
  }

</style>