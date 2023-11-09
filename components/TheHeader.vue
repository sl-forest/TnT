<template>
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
            <li><a class="item-link" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a class="item-link" href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </nav>

      <div class="serch-box">
        <form id="form" action="http://localhost:3000" method="get">
        <input id="sbox" type="search" name="search" placeholder="キーワードを入力">
        <input id="sbtn" type="submit" name="submit" value="検索">
        </form>
      </div>

    </header>
</template>

<style>
  /* スマホ向けスタイル */

  /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
  /* ヘッダー */
  header {
    display: flex;  /*ヘッダーの下の要素を並列に*/
    height: 80px; /*ヘッダーの高さ*/
    padding: 0; /*ヘッダーの位置調整*/
    background: #333; /*ヘッダーの背景色*/
  }

  .site-name h1 {
    color: #fff;  /*サイトの名前の色*/
  }

  /* ロゴ */
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

  .menu {
    padding-left: 3em;
  }
 
  .item ul {
    display: inline-block;
    margin-top: 25px;
  }

  ul {
    list-style: none;
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

  .top_img img {
    width: 100%;
  }

  /* 検索 */
  #sbox {	
    outline: 0;	
    height: 40px;
    padding: 0 10px; 
    position: absolute; 
    left: 25cm;
    top: 29px; 
    max-width: 270px;
    border-radius: 2px;
    background: #eee;
  }

  #sbtn {
    width: 56px;
    height: 37px;
    position: absolute; 
    left: 30cm; 
    top: 30.5px;
    border-radius: 2px;
    background: #7fbfff;
    color: #fff;
    font-weight: bold;
    font-size: 16px;
    border: none;
  }

  #sbtn:hover {
    background: #eee;
    color: #7fbfff;
  }
}
</style>