<template>

  <div>
    <TheHeader />

    <main>
      <h1>「郷土料理」</h1>
      <h2 class = localcuisine_headline>豚骨</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonkotsu.jpg" alt="豚骨">
        </div>
          
        <div class = explanation>
          <p>
            「豚骨」とは、豚の骨付きあばら肉を焼いて芋焼酎で炒りつけてこんにゃくや大根などの野菜と<br>
            ともに、味噌と黒砂糖で煮こんでつくる郷土料理。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/Tonkotsu"><b>詳細はこちら</b></a>
        </div>
      </div>

      <h2 class = localcuisine_headline>がね</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Gane.jpg" alt="がね">
        </div>

        <div class = explanation>
          <p>「がね」は鹿児島県の特産品として全国に知られるさつまいもを食材とした郷土料理。</p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/Gane"><b>詳細はこちら</b></a>
        </div>
      </div>

      <h2 class = localcuisine_headline>油ゾーメン</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Zomen.jpg" alt="油ゾーメン">
          <div class="teikyou">
            <p><b>出典</b></p>
            <p><b>農林水産省「うちの郷土料理」</b></p>
          </div>
        </div>

        <div class = explanation>
          <p>
            「油ゾーメン」は、豚肉と野菜、そうめんを炒めた郷土料理。
            沖縄の「そうめんチャンプルー」に<br>似ているが、奄美地域の「油ゾーメン」は、炒める時にだし汁を入れるのが特徴。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/AburaZomen"><b>詳細はこちら</b></a>
        </div>  
      </div>

      <h2 class = localcuisine_headline>黒糖</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Kokutou.jpg" alt="黒糖">
        </div>

        <div class = explanation>
          <p>
            「黒糖」は、とうきびを細かくカットし、圧搾機にかけて絞り出した汁を煮詰めてつくる砂糖。<br>
            奄美地域および沖縄県の特産品。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/LocalCuisine/pages/Kokutou"><b>詳細はこちら</b></a>
        </div>
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
            <a class="Pagination-Item-Link isActive" href="http://localhost:3000/LocalCuisine/pages/2"><span>2</span></a>
          </li>

          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/LocalCuisine/pages/3"><span>3</span></a>
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
/* 共通 */
main {margin: 0 auto;}

h1 {font-family: 'New Tegomin', serif;}

.LocalCuisine p {
  font-family: serif;
  font-weight: bold;
}

.link-space a {
  margin: 0;
  font-weight: bold;
  font-size: 15px;
}

/* ページネーション */
.Pagination {
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
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

.Pagination-Item-Link-Icon {width: 20px;}

.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  br {display: none;}

  .localcuisine {text-align: center;}

  h2.localcuisine_headline {
    margin: 0;
    text-align: center;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  .link-space {margin: 8px 0;}

  .explanation p {
    font-size: 15px;
    text-align: left; /* 左寄せ */
    margin-top: 16px;
    margin-bottom: 0;
  }
  
  .explanation-link {
    text-decoration: none;
    color: blue;
  }

/* 提供 */
  .teikyou p {
    margin: 0;
    font-size: 14px;
  }
  
/* 郷土料理画像 */
  .localcuisine_img img{
    width: 8cm;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}

  h1 {margin-bottom: 0;}
  
/* 郷土料理一覧説明 */
  .localcuisine {display: flex;}

  .localcuisine p {
    margin: 0;
    font-size: 14px;
  }

  h2.localcuisine_headline {
    margin: 0;
    padding-top: 8px;
    border-top: 2px solid #d5d4c3;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

  .explanation-link {
    align-self: end;
    text-decoration: none;
    color: blue;
  }

  a:hover.explanation-link {color: rgb(71, 1, 92);}

/* 郷土料理画像 */
  .localcuisine_img img{
    width: 5cm;
    height: auto;
  }

/* 提供 */
  .teikyou p {font-size: 13px;}
}
</style>