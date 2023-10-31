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
        
        <h1>工芸品</h1>
        
        <ul class = "craft-introduction">
        
          <li class = "craft-image">
            <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
          </li>

          <li class = "craft-image">
            <img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子">
          </li>

        </ul>

         <h1>歴史</h1>

        <ul class = "history-introduction">
        
          <li class = "history-image">
            <img src="~/assets/img/segodon.jpeg" alt="西郷隆盛">
          </li>

          <li class = "history-image">
            <img src="~/assets/img/ookubo.jpg" alt="大久保利通">
          </li>

        </ul>

         <h1>郷土料理</h1>

        <ul class = "LocalCuisine-introduction">
        
          <li class = "LocalCuisine-image">
            <img src="~/assets/img/Keihan.jpg" alt="鶏飯">
          </li>

          <li class = "LocalCuisine-image">
            <img src="~/assets/img/Shirokuma.jpg" alt="白熊">
          </li>

        </ul>

        <h1>観光地</h1>

        <ul class = "TouristSpot-introduction">
        
          <li class = "TouristSpot-image">
            <img src="~/assets/img/Jingu.jpg" alt="霧島神宮">
          </li>

          <li class = "TouristSpot-image">
            <img src="~/assets/img/TenmonKan.jpg" alt="天文館">
          </li>

        </ul>
        
        <h1>世界遺産</h1>

        <ul class = "WorldHeritage-introduction">
        
          <li class = "WorldHeritage-image">
            <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
          </li>

          <li class = "WorldHeritage-image">
            <a href = "http://localhost:3000/Craft/pages/2"><img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）"></a>
          </li>

        </ul>

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

  a {
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  .introduction h1 {
    text-align: center;
  }

/* 工芸品 */
  .craft-introduction {
    display: flex;
    justify-content: center;
  }

  .craft-image {
    list-style: none;
  }

  .craft-image:nth-child(2) {
    margin: 0 4em;
  }

  .craft-image img {
    height: 20em;
  }

/* 歴史 */
  .history-introduction {
    display: flex;
    justify-content: center;
  }

  .history-image {
    list-style: none;
  }

  .history-image:nth-child(2) {
    margin: 0 4em;
  }

  .history-image img {
    height: 15em;
  }

  /* 郷土料理 */
  .LocalCuisine-introduction {
    display: flex;
    justify-content: center;
  }

  .LocalCuisine-image {
    list-style: none;
  }

  .LocalCuisine-image:nth-child(2) {
    margin: 0 4em;
  }

  .LocalCuisine-image img {
    height: 15em;
  }

  /* 観光地 */
  .TouristSpot-introduction {
    display: flex;
    justify-content: center;
  }

  .TouristSpot-image {
    list-style: none;
  }

  .TouristSpot-image:nth-child(2) {
    margin: 0 4em;
  }

  .TouristSpot-image img {
    height: 15em;
  }

  /* 世界遺産 */
  .WorldHeritage-introduction {
    display: flex;
    justify-content: center;
  }

  .WorldHeritage-image {
    list-style: none;
  }

  .WorldHeritage-image:nth-child(2) {
    margin: 0 4em;
  }

  .WorldHeritage-image img {
    height: 15em;
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