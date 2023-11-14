<template>

  <div>
    <TheHeader />

    <main>
      <h1>「観光地」</h1>
      <h2 class = spot_headline>曾木の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/SogiTaki.jpg" alt="曾木の滝">
        </div>
          
        <div class = explanation>
          <p>幅約210メートル、高さ約12メートルのスケールを誇り、「東洋のナイアガラ」とも呼ばれる滝。</p>
          <p>春は桜やつつじが彩り、夏は水量も多く豪快。</p>
          <p>秋は紅葉がライトアップされ、冬は雪景色を楽しめる。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Soginotaki" target=”_blank”><b>スポット情報</b></a>
      </div>

      <h2 class = spot_headline>丸尾の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/MaruoTaki.jpg" alt="丸尾の滝">
        </div>

        <div class = explanation>
          <p>高さ約23メートル、幅約16メートルの滝。</p>
          <p>ここを流れる水は温泉の湯であり、霧島地区の温泉水を集めて流れる珍しい「湯の滝」。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Maruonotaki" target=”_blank”><b>スポット情報</b></a>
      </div>

      <h2 class = spot_headline>雄川の滝</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/OgawaTaki.jpg" alt="雄川の滝">
        </div>

        <div class = explanation>
          <p>落差約46メートル、幅約60メートルの滝。</p>
          <p>大河ドラマ『西郷どん』のオープニング映像で話題となった。。</p>
          <p>エメラルドグリーンの美しい滝つぼが特徴で、フォトジェニックな光景が広がる。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Ogawanotaki" target=”_blank”><b>スポット情報</b></a>
      </div>
      
      <h2 class = spot_headline>開聞岳</h2>
      <div class="spot">
        <div class = spot_img>
          <img src="~/assets/img/KaimonDake.jpg" alt="開聞岳">
        </div>

        <div class = explanation>
          <p>薩摩半島の最南端に位置する標高約924メートルの開聞岳は、「日本百名山」にも数えられている南薩を代表する山。</p>
          <p>別名「薩摩富士」と呼ばれ、指宿のシンボルとして親しまれている。</p>
        </div>
          <a class ="explanation-link" href="http://localhost:3000/TouristSpot/pages/Kaimondake" target=”_blank”><b>スポット情報</b></a>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/TouristSpot/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/4"><span>4</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/TouristSpot/pages/4">
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

      h2.spot_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 観光地一覧説明 */
      .spot {
        display: flex;
      }

      .spot p {
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

      /* 観光地画像 */
      .spot_img img{
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