<template>
    <header>
    <div class="main-menu">
    <!-- ロゴ -->
      <div class="logo">
        <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>
      </div>

      <!--  サイトの名前 -->
      <div class="site-name">
        <h1>鹿児島紹介サイト</h1>
      </div>

      <div class="pc-menu">

        <ul>
          <li>
            <a href="http://localhost:3000/Craft/pages/1">工芸品</a>
          </li>

          <li>
            <a href="http://localhost:3000/History/pages/1">歴史</a>
          </li>

          <li>
            <a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a>
          </li>

          <li>
            <a href="http://localhost:3000/TouristSpot/pages/1">観光地</a>
          </li>

          <li>
            <a href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a>
          </li>
          
        </ul>

      </div>

      <div>
        <form method="get" action="http://www.google.co.jp/search" class="search-form-005" target="_blank">
          <label>  
            <input type="text" name="q" value="キーワードを入力">
          </label>
          <button type="submit" name="btng" value="検索"></button>
        </form>
      </div>
      
      <div class="sp-menu">

      <input type="checkbox" id="sp-menu__check">
      <label for="sp-menu__check" class="sp-menu__box">
        <span></span>
      </label>

      <div class="sp-menu__content">
        <ul class="sp-menu__list">
          <li class="sp-menu__item">
            <a class="sp-menu__link" href="http://localhost:3000/Craft/pages/1">工芸品</a>
          </li>
          <li class="sp-menu__item">
            <a class="sp-menu__link" href="http://localhost:3000/History/pages/1">歴史</a>
          </li>
          <li class="sp-menu__item">
            <a class="sp-menu__link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a>
          </li>
          <li class="sp-menu__item">
            <a class="sp-menu__link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a>
          </li>
          <li class="sp-menu__item">
            <a class="sp-menu__link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a>
          </li>
        </ul>

        <div>
          <form method="get" action="http://www.google.co.jp/search" class="search-form-005" target="_blank">
            <label>  
              <input type="text" name="q" value="キーワードを入力">
            </label>
            <button type="submit" name="btng" value="検索"></button>
          </form>
        </div>
        
      </div>
    </div>
  </div>
</header>
</template>

<style>
/* 画面サイズが1023px以下の時はPC用メニューは非表示 */
@media screen and (max-width: 1023px) {
  .pc-menu {
    display: none;
  }

  /* ロゴ */
  .logo {
    margin-top: 5px;  /*ロゴの位置調整*/
    margin-bottom: 5px; /*ロゴの位置調整*/
    margin-left: 15px;  /*ロゴの位置調整*/
    margin-right: 15px; /*ロゴの位置調整*/
  }

  .logo a img {
    width: 48px;  /*ロゴ画像の幅調整*/
    height: 48px; /*ロゴ画像の高さ調整*/
    padding-top: 12px; /*ロゴの位置調整*/
  }

  .site-name h1 {
    color: #fff;  /*サイトの名前の色*/
    font-size: 24px;
    margin-top: 29px;
    margin-bottom: 0;
  }
}
/* 画面サイズが1024px以上の時はスマホ用メニューは非表示 */
@media screen and (min-width: 1024px) {
  .sp-menu {
    display: none;
  }

  .logo a img {
    width: 56px;  /*ロゴ画像の幅調整*/
    height: 56px; /*ロゴ画像の高さ調整*/
    padding-top: 12px; /*ロゴの位置調整*/
  }

  .site-name h1 {
    color: #fff;  /*サイトの名前の色*/
    margin-top: 21px;
    margin-left: 16px;
    margin-bottom: 0;
  }
}

  header {
    display: flex;  /*ヘッダーの下の要素を並列に*/
    height: 80px; /*ヘッダーの高さ*/
    padding: 0; /*ヘッダーの位置調整*/
    background: #333; /*ヘッダーの背景色*/
  }

  .site-name {
    width: 38em;
  }

  .main-menu {
    margin: 0 auto;
    display: flex;
    width: 1280px;
  }

  .logo {
    text-align: center;
  }

  .pc-menu {
    width: 100%;
  }

  .pc-menu > ul {
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0;
    margin-top: 16px;
  }

  .pc-menu > ul > li {
    text-align: center;
    font-size: 16px;
    width: 12%;
  }

  .pc-menu > ul > li > a {
    display: block;
    text-decoration: none;
    color: #fff;
    line-height: 60px;
  }
  
  .pc-menu > ul > li > a:hover {
    background: #cccccc;
  }

  .sp-menu__box {
    position: fixed;
    top: 18px;
    right: 41.5em;
    display: flex;
    height: 60px;
    width: 60px;
    justify-content: center;
    align-items: center;
    z-index: 90;
    background: #3584bb;
  }

  .sp-menu__box span,
  .sp-menu__box span:before,
  .sp-menu__box span:after {
    content: "";
    display: block;
    height: 3px;
    width: 25px;
    border-radius: 3px;
    background: #ffffff;
    position: absolute;
  }

  .sp-menu__box span:before {
    bottom: 8px;
  }

  .sp-menu__box span:after {
    top: 8px;
  }

  #sp-menu__check {
    display: none;
  }

  #sp-menu__check:checked ~ .sp-menu__box span {
    background: rgba(255, 255, 255, 0);
  }

  #sp-menu__check:checked ~ .sp-menu__box span::before {
    bottom: 0;
    transform: rotate(45deg);
  }

  #sp-menu__check:checked ~ .sp-menu__box span::after {
    top: 0;
    transform: rotate(-45deg);
  }

  #sp-menu__check:checked ~ .sp-menu__content {
    left: 0;
  }

  .sp-menu__content {
    width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    left: 100%;
    z-index: 80;
    background-color: #3584bb;
    transition: all 0.5s;
  }

  .sp-menu__list {
    padding: 70px 10px 0;
  }

  .sp-menu__item {
    border-bottom: solid 1px #ffffff;
    list-style: none;
  }

  .sp-menu__link {
    display: block;
    width: 100%;
    font-size: 15px;
    box-sizing: border-box;
    color: #ffffff;
    text-decoration: none;
    padding: 9px 15px 10px 0;
  }

/* 検索 */
  form {
    margin: auto;
  }

  .search-form-005 {
    display: flex;
    align-items: center;
    overflow: hidden;
    border-radius: 3px;
    margin: 0;
    padding-top: 20px;
    width: 8cm;
  }

  .search-form-005 input {
    width: 250px;
    height: 45px;
    padding: 5px 15px;
    border: none;
    border-radius: 3px 0 0 3px;
    box-sizing: border-box;
    background-color: #e6edf3;
    font-size: 1em;
    outline: none;
  }

  .search-form-005 input::placeholder {
    color: #767d83;
  }

  .search-form-005 button {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 45px;
    border: none;
    border-radius: 0 3px 3px 0;
    background-color: #2589d0;
    cursor: pointer;
  }

  .search-form-005 button::after {
    width: 20px;
    height: 20px;
    background-image: url('data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%3E%20%3Cpath%20d%3D%22M23.7%2020.8%2019%2016.1c-.2-.2-.5-.3-.8-.3h-.8c1.3-1.7%202-3.7%202-6C19.5%204.4%2015.1%200%209.7%200S0%204.4%200%209.7s4.4%209.7%209.7%209.7c2.3%200%204.3-.8%206-2v.8c0%20.3.1.6.3.8l4.7%204.7c.4.4%201.2.4%201.6%200l1.3-1.3c.5-.5.5-1.2.1-1.6zm-14-5.1c-3.3%200-6-2.7-6-6s2.7-6%206-6%206%202.7%206%206-2.6%206-6%206z%22%20fill%3D%22%23fff%22%3E%3C%2Fpath%3E%20%3C%2Fsvg%3E');
    background-repeat: no-repeat;
    content: '';
  }
</style>