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
    </header>

    <main>
        <h1>「伝統工芸品」</h1>
        <h2 class = craft_headline>本場大島紬</h2>
        <div class=" craft01 ">
            <div class = craft01_img>
                <img src="~/assets/img/OshimaTsumugi.jpg" alt="本場大島紬">
            </div>
            
            <div class = explanation01>
                <p>1,300年の歴史を持ち、
                  絹織物の最高傑作といわれています。
                  30数工程もある緻密な手作業により、
                  図案から織り上がるまで半年から1年以上もかかります。
                  大島紬独自の技法「テーチ木泥染」は、
                  7世紀中頃から行われていた古代染色の技法を取り入れたものです。
                  緻密な絣模様や、軽くて暖かく、しなやかで着くずれしないなどの
                  優れた特徴があり、女性の着物として高い人気があります。</p>
            </div>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class=" craft02 ">
            <div class = craft01_img>
                <img src="" alt="???">
            </div>

            <div class = explanation02>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class=" craft03 ">
            <div class = craft03_img>
                <img src="" alt="???">
            </div>

            <div class = explanation03>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class=" craft04 ">
            <div class = craft04_img>
                <img src="" alt="???">
            </div>

            <div class = explanation04>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

        <h2 class = craft_headline>???</h2>
        <div class=" craft05 ">
            <div class = craft05_img>
                <img src="" alt="???">
            </div>

            <div class = explanation05>
                <p></p>
                <p></p>
                <p></p>
                <p></p>
            </div>
        </div>

          <ul class="Pagination">
            <li class="Pagination-Item">
              <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/5">
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
                    <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/5"><span>5</span></a>
                </li>

                <li class="Pagination-Item">
                    <a class="Pagination-Item-Link" href="/pages/5/">
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
    
    nav ul{
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

      h1 {
        margin-bottom: 0;
      }

      h2.craft_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      .craft01 {
        display: flex;
      }

      .craft01_img {
        width: 5cm;
        margin: 0;
        padding: 0;
      }

      .craft01 img {
        width: 5cm;
        height: auto;
      }

      .craft01 p {
        padding: 0, 0, 0, 20;
        margin: 0;
      }

      .explanation01 {
        margin-left: auto;
        margin-right: auto;
        width: 40em;
      }

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