<template>

  <div>
    <TheHeader />

    <main>
      <h1>「郷土料理」</h1>
      <h2 class = localcuisine_headline>豚骨</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonkotsu-min.jpg" alt="豚骨">
        </div>
          
        <div class = explanation>
          <p>
            「豚骨」とは、豚の骨付きあばら肉を焼いて芋焼酎で炒りつけてこんにゃくや大根などの<br>
            野菜とともに、味噌と黒砂糖で煮こんでつくる郷土料理。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Tonkotsu">豚骨はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = localcuisine_headline>がね</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Gane-min.jpg" alt="がね">
        </div>

        <div class = explanation>
          <p>「がね」は鹿児島県の特産品として全国に知られるさつまいもを食材とした郷土料理。</p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Gane">がねはこちら</a>
          </div>
        </div>
      </div>

      <h2 class = localcuisine_headline>油ゾーメン</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Zomen-min.jpg" alt="油ゾーメン">
          <div class="teikyou">
            <p>
              出典：<br>
              農林水産省「うちの郷土料理」
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            「油ゾーメン」は、豚肉と野菜、そうめんを炒めた郷土料理。<br>
            沖縄の「そうめんチャンプルー」に似ているが、奄美地域の「油ゾーメン」は、炒める時にだし汁を入れるのが特徴。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/AburaZomen">油ゾーメンはこちら</a>
          </div>
        </div>  
      </div>

      <h2 class = localcuisine_headline>黒糖</h2>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Kokutou-min.jpg" alt="黒糖">
        </div>

        <div class = explanation>
          <p>
            「黒糖」は、とうきびを細かくカットし、圧搾機にかけて絞り出した汁を煮詰めてつくる砂糖。<br>
            奄美地域および沖縄県の特産品。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/LocalCuisine/pages/Kokutou">黒糖はこちら</a>
          </div>
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
body {margin: 0;}
main {margin: 0 auto;}

h1 {
  margin: 0;
  font-family: 'New Tegomin', serif;
}

h2.localcuisine_headline {
  margin: 0;
  padding: 8px 0;
  border-top: 2px solid #d5d4c3;
}

/* 提供文字 */
.teikyou {font-weight: bold;}

.teikyou p {
  margin: 0;
  font-size: 13px;
}

.explanation p {
  margin: 0;
  font-family: serif;
  font-weight: bold;
  font-size: 15px;
}

/* ボタン */
.btn {
  display: inline-block;
  padding: 0.3em 0.6em;
  text-decoration: none;
  color: black;
  border: solid 2px black;
  border-radius: 3px;
  transition: .4s;
}

/* マウスオーバー */
.btn:hover {
  background: black;
  color: white;
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

/* アクティブボタン */
.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

/* マウスオーバー */
.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}

  h1 {
    padding: 8px 0;
    text-align: center;
  }

  br {display: none;}
  .localcuisine {text-align: center;}
  h2.localcuisine_headline {text-align: center;}

  .explanation p {
    text-align: left;
    margin-top: 16px;
  }

  .link-space {margin: 16px 0;}

/* 画像 */
  .localcuisine_img img {
    width: 320px;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}

  h1 {padding-top: 16px;}
  
/* 一覧説明 */
  .localcuisine {
    display: flex;
    margin-bottom: 16px;
    column-gap: 1rem;
  }
  
  .explanation {align-self: center;}
  .link-space {margin-top: 0.5rem;}

/* 画像 */
  .localcuisine_img img {
    width: 190px;
    height: auto;
  }
}
</style>