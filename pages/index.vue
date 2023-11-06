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
          <p>そんな魅力溢れる鹿児島を体験してみてください。</p>
        </center>
      </div>

      <div class= "talk">
        <div class = human01><img src ="" alt="ジジイ"></div>
        <p></p>
        <div class = human02><img src ="" alt="息子"></div>
        <p></p>
      </div>

      <div class = "introduction">

        <div class="flex">
          
          <figure class="image"><img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子"></figure>
          <div class="right">
            <h2 class="title">工芸品</h2>
            <p class="text">ここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入ります</p>
          </div>

          <figure class="image"><img src="~/assets/img/segodon.jpeg" alt="西郷隆盛"></figure>
          <div class="right">
            <h2 class="title">歴史</h2>
            <p class="text">ここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入ります</p>
          </div>

        </div>

        <div class="flex">
          
          <figure class="image"><img src="~/assets/img/Keihan.jpg" alt="鶏飯"></figure>
          <div class="right">
            <h2 class="title">郷土料理</h2>
            <p class="text">ここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入ります</p>
          </div>

          <figure class="image"><img src="~/assets/img/Jingu.jpg" alt="霧島神宮"></figure>
          <div class="right">
            <h2 class="title">観光地</h2>
            <p class="text">ここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入ります</p>
          </div>

        </div>
        
        <div class="flex">
          
          <figure class="image"><img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）"></figure>
          <div class="right">
            <h2 class="title">世界遺産</h2>
            <p class="text">ここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入りますここにテキストが入ります</p>
          </div>

        </div>

      </div>


    </body>
    
    <footer class="footer">

      <p class="copyright">© 2023 TnT Inc.</p>
      <ul class="md-flex">
        <li><a href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
        <li><a href="http://localhost:3000/History/pages/1">歴史</a></li>
        <li><a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
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

  .Kagoshima_about h1 {
    margin-bottom: 8px;
  }

  .Kagoshima_about p {
    font-size: 25px;
    margin: 0;
  }

  .image img {
    width: 15em;
  }
  
  html {
    font-family: sans-serif;
  }

  a {
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  /* 横並び */
  .flex {
    display: flex; /*横並び*/
    margin-left: 24px;
    margin-bottom: 64px;
  }

  .flex .image {
    width: 15em; /*画像サイズ指定*/
    height: 15em;
    margin: 0;
    padding: 0;
    overflow: hidden;
    position: relative;
  }

  .flex .right {
    margin: 0 0 0 20px;
    padding: 0;
  }

  .flex .title {
    margin: 0;
    padding: 0;
    font-weight: bold;
  }

  .flex .text {
    margin: 10px 0 0;
    padding: 0;
    width: 18em;
  }

  /* 画像を天地中央表示 */

  .flex .image {
    overflow: hidden;
    position: relative;
  }

  .flex .image::before {
    content: "";
    display: block;
    padding-top: 58%;
  }

  .flex .image img {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
  }

  /* フッター */
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