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
            <li><a class="item-link" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a class="item-link" href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000/TraditionalCulture/pages/1">伝統芸能</a></li>
            <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </nav>
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
    
    <footer class="footer">
      <p class="copyright">© 2023 TnT Inc.</p>
      <ul class="md-flex">
        <li><a href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
        <li><a href="http://localhost:3000/History/pages/1">歴史</a></li>
        <li><a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
        <li><a href="http://localhost:3000/TraditionalCulture/pages/1">伝統芸能</a></li>
        <li><a href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
        <li><a href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
    </ul>
    </footer>

  </div>
</template>

<style>
  @media (min-width: 768px) {
  .footer {
    display: flex;
    justify-content: space-between;
  }

  .md-flex {
    display: flex;
  }

  .md-flex li + li {
    margin-left: 16px;
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
  
  html {
    font-family: sans-serif;
  }

  bo  dy {
    background: rgb(0, 0, 0);
  }

  a {
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  .footer {
    padding: 2rem;
    font-size: 15px;
    color: rgb(255, 255, 255);
    background: rgb(0, 0, 0);
    border-top: 1px solid #e5e7eb;
  }

  .footer a:hover {
    color: rgb(2, 243, 252);
  }
}
</style>