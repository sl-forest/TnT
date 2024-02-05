<template>

  <div>
    <TheHeader />
    <main>
      <h1>「国指定伝統工芸品」</h1>
      <h2 class = craft_headline>本場大島紬</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/OshimaTsumugi-min.jpg" alt="本場大島紬">
        </div>
        
        <div class = explanation>
          <p>
            1,300年の歴史を持ち、絹織物の最高傑作といわれている。<br>
            30数工程もある緻密な手作業により、図案から織り上がるまで半年から1年以上もかかる。<br>
            大島紬村では本場大島紬の製造現場見学や、泥染め・織り体験、着付体験などが楽しめる。
          </p>
          <div class="link-space">
            <a class="btn" href="http://localhost:3000/Craft/pages/AuthenticOshimaTsumugi">本場大島紬はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = craft_headline>川辺仏壇</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/kawabebutudan-min.jpg" alt="川辺仏壇">
        </div>

        <div class = explanation>
          <p>
            川辺仏壇（かわなべぶつだん）は、鹿児島県南九州市川辺町周辺で作られている仏壇。<br>
            川辺仏壇の特徴は、「ガマ戸」と呼ばれる川辺仏壇オリジナルの独特な仏壇がある。<br>
            ”ガマ”とは、鹿児島県の方言で洞窟を表す。
          </p>
          <div class="link-space">
            <a class="btn" href="http://localhost:3000/Craft/pages/KawabeButsudan">川辺仏壇はこちら</a>
          </div>
        </div>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4"><span>4</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4">
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

h2.craft_headline {
  margin: 0;
  padding: 8px 0;
  border-top: 2px solid #d5d4c3;
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
  br {display: none;}

  h1 {
    padding: 8px 0;
    text-align: center;
  }

  .craft {text-align: center;}
  h2.craft_headline {text-align: center;}
  .link-space {margin: 16px 0;}

  .explanation p {
    text-align: left;
    margin-top: 16px;
  }
  
/* 画像 */
  .craft_img img {
    width: 320px;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}
  h1 {padding-top: 16px;}
  
/* 一覧説明 */
  .craft {
    display: flex;
    margin-bottom: 16px;
    column-gap: 1rem;
  }
  
  .explanation {align-self: center;}
  .link-space {margin-top: 0.5rem;}

/* 画像 */
  .craft_img img {
    width: 180px;
    height: auto;
  }
}
</style>