<template>
  <div>

    <header>
      <!-- ロゴ -->
      <div class="logo">
        <a href="#"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>
      </div>

      <!--  サイトの名前 -->
      <div class="site-name">
        <h1>鹿児島紹介サイト</h1>
      </div>

      <!-- メニュー -->
      <nav>
        <div class="menu">
          <ul class="item">
            <li><a class="item-link" href="http://localhost:3000/Craft">工芸品</a></li>
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
      <search>
      <form id="form1" action="http://localhost:3000/about">
      <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
      <input id="sbtn" type="submit" value="検索" />
      </form>
      </search>
      
    </header>

    <body>
      <div class="top_img">
        <img src="~/assets/img/Top_img1.png" alt="トップ画像">
      </div>

      <div class="Kagoshima_about">
        <center>
          <h1>～鹿児島について～</h1>
          <p>多くの観光名所や豊かな自然があり、その土地に根付いた伝統と人の温もり溢れる地方。</p>
          <p>時代の流れに揉まれ戦乱の歴史をその身に刻みながらも発展してきた鹿児島。</p>
          <p>そんな魅力溢れる鹿児島を体験してみてはいかがでしょうか？</p>
        </center>
      </div>

      <div class= talk>
        <div class = human01><img src ="" alt="ジジイ"></div>
        <p></p>
        <div class = human02><img src ="" alt="息子"></div>
        <p></p>
      </div>
    </body>

    <footer>
      <p>footer</p>
    </footer>
  </div>
</template>

<style>

  header {
    display: flex;  /*ヘッダーの下の要素を並列に*/
    height: 80px; /*ヘッダーの高さ*/
    padding: 0; /*ヘッダーの位置調整*/
    background: #333; /*ヘッダーの背景色*/
  }

  .site-name h1 {
    color: #fff;  /*サイトの名前の色*/
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

  .top_img img {
    width: 100%;
  }

  .Kagoshima_about h1 {
    margin-bottom: 8px;
  }

  .Kagoshima_about p {
    font-size: 25px;
    margin: 0;
  }
</style>
