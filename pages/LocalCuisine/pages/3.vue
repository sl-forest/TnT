<template>

  <div>
    <TheHeader />

    <main>
      <h1>「郷土料理」</h1>
      <h2 class = localcuisine_headline>白熊</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Shirokuma.jpg" alt="白熊">
          <p>出典：</p>
          <p>農林水産省「うちの郷土料理」</p>
        </div>
        
        <div class = explanation>
          <p>「白熊」は、削った氷に練乳をかけ、その上にチェリーやレーズン、みかん、パイン、小豆、寒天と、色とりどりのトッピングをのせた氷菓子。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/ShiroKuma" target=”_blank”><b>詳細はこちら</b></a>
      </div>

      <h2 class = localcuisine_headline>かるかん</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Karukan02.jpg" alt="かるかん">
          <p>画像提供元 : 鹿児島県</p>
        </div>

        <div class = explanation>
          <p>「かるかん」は、かるかん粉、山芋、水を使ってつくる鹿児島県の銘菓。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/Karukan" target=”_blank”><b>詳細はこちら</b></a>
      </div>

      <h2 class = localcuisine_headline>両棒餅（じゃんぼ餅）</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Janbomoti.jpg" alt="じゃんぼ餅">
          <p>出典：</p>
          <p>農林水産省「うちの郷土料理」</p>
        </div>

        <div class = explanation>
          <p>「じゃんぼ餅」とは、つきたての餅やもち米粉を使っただんご串を2本さして、とろみのある砂糖醤油ダレをかけて食べる、鹿児島県で古くから親しまれている料理である。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/JumboMochi" target=”_blank”><b>詳細はこちら</b></a>
      </div>

      <h2 class = localcuisine_headline>神酒（みき）</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Miki.jpg" alt="みき">
          <p>出典：</p>
          <p>農林水産省「うちの郷土料理」</p>
        </div>

        <div class = explanation>
          <p>米とさつまいも、砂糖を使った乳酸菌発酵飲料で、奄美地域の他に沖縄県でも飲まれている。</p>
          <p>沖縄県では、さつまいもではなく麦を使う。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/Miki" target=”_blank”><b>詳細はこちら</b></a>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/1"><span>1</span></a>
          </li>
          
          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/2"><span>2</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link isActive" href="http://localhost:3000/LocalCuisine/pages/3"><span>3</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/3">
              <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M13 5l7 7-7 7M5 5l7 7-7 7" />
              </svg>
            </a>
          </li>
        </ul>
      </main>
    <TheFooter />
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

      h1 {
        margin-bottom: 0;
      }

      h2.localcuisine_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 工芸品一覧説明 */
      .localcuisine {
        display: flex;
      }

      .localcuisine p {
        margin: 0;
        font-size: 14px;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
        text-decoration: none;
        color: blue;
      }

      a:hover.explanation-link {
        color: rgb(71, 1, 92);
      }

      /* 郷土料理画像 */
      .localcuisine_img img{
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