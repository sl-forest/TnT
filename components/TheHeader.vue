<template>
  <div>
    <head><head><meta name="viewport" content="width=device-width,initial-scale=1"></head></head>

    <header>
      <!-- ロゴ -->
      <div class="logo">
        <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>
      </div>

      <!--  サイトの名前 -->
      <div class="site-name">
        <h1>鹿児島紹介サイト</h1>
      </div>

      <!-- メニュー -->
        <div class="menu">
          
          <span></span>
          <span></span>
          <span></span>
          
          <nav class="globalMenuSp">
            
            <ul class="item">
              <li><a class="item-link" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
              <li><a class="item-link" href="http://localhost:3000/History/pages/1">歴史</a></li>
              <li><a class="item-link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
              <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
              <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
            </ul>
          </nav>
        </div>

        <form method="get" action="http://www.google.co.jp/search" target="_blank">
          <input type="text" name="q" size="20" maxlength="80" value="">
          <input type="submit" name="btng" value="検索">
          <input type="hidden" name="hl" value="ja">
        </form>

    </header>
  </div>
</template>

<style>
  /* スマホ向けスタイル */
  @media screen and (max-width:480px) {

    * {
	  float: none;
	  position: static;
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

  /*　ハンバーガーメニューボタン　*/
  .hamburger {
    display : block;
    position: fixed;
    z-index : 3;
    right : 20px;
    top   : 20px;
    width : 42px;
    height: 42px;
    cursor: pointer;
    text-align: center;
  }

  .hamburger span {
    display : block;
    position: absolute;
    width   : 30px;
    height  : 2px ;
    left    : 6px;
    background : #BBBBBB;
    -webkit-transition: 0.3s ease-in-out;
    -moz-transition   : 0.3s ease-in-out;
    transition        : 0.3s ease-in-out;
  }

  .hamburger span:nth-child(1) {
    top: 10px;
  }

  .hamburger span:nth-child(2) {
    top: 20px;
  }

  .hamburger span:nth-child(3) {
    top: 30px;
  }

  /* スマホメニューを開いてる時のボタン */
  .hamburger.active span:nth-child(1) {
    top : 16px;
    left: 6px;
    background :#fff;
    -webkit-transform: rotate(-45deg);
    -moz-transform   : rotate(-45deg);
    transform        : rotate(-45deg);
  }

  .hamburger.active span:nth-child(2),
  .hamburger.active span:nth-child(3) {
    top: 16px;
    background :#fff;
    -webkit-transform: rotate(45deg);
    -moz-transform   : rotate(45deg);
    transform        : rotate(45deg);
  }

  /* メニュー背景　*/
  nav.globalMenuSp {
    position: fixed;
    z-index : 2;
    top  : 0;
    left : 0;
    color: #fff;
    background: rgba( 71,70,73,0.6 );
    text-align: center;
    width: 100%;
    transform: translateY(1000%);
    transition: all 0.6s;
  }

  nav.globalMenuSp ul {
    margin: 0 auto;
    padding: 0;
    width: 100%;
  }

  nav.globalMenuSp ul li {
    list-style-type: none;
    padding: 0;
    width: 100%;
    transition: .4s all;
  }

  nav.globalMenuSp ul li:last-child {
    padding-bottom: 0;
  }

  nav.globalMenuSp ul li:hover{
    background :#ddd;
  }

  nav.globalMenuSp ul li a {
    display: block;
    color: #fff;
    padding: 1em 0;
    text-decoration :none;
  }

  /* クリックでjQueryで追加・削除 */
  nav.globalMenuSp.active {
    opacity: 100;
    display: block;
    transform: translateY(0%);
  }

  .top_img img {
    width: 100%;
  }
}
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

  form {
    margin: auto;
  }

  .top_img img {
    width: 100%;
  }
}
</style>