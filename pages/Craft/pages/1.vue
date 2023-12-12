<template>

  <div>
    <TheHeader />

    <main>
      <h1>「国指定伝統工芸品」</h1>
      <h2 class = craft_headline>本場大島紬</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/OshimaTsumugi.jpg" alt="本場大島紬">
        </div>
        
        <div class = explanation>
          <p>
            1,300年の歴史を持ち、絹織物の最高傑作といわれている。<br class="pc">
            30数工程もある緻密な手作業により、図案から織り上がるまで半年から1年以上もかかる。<br class="pc">
            大島紬村では本場大島紬の製造現場見学や、泥染め・織り体験、着付体験などが楽しめる。
          </p>
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/AuthenticOshimaTsumugi"><b>基本情報はこちら</b></a>
        </div>

      </div>

      <h2 class = craft_headline>川辺仏壇</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/kawabebutudan.jpg" alt="川辺仏壇">
        </div>

        <div class = explanation>
          <p>
            川辺仏壇（かわなべぶつだん）は、鹿児島県南九州市川辺町周辺で作られている仏壇。<br class="pc">
            川辺仏壇の特徴は、「ガマ戸」と呼ばれる川辺仏壇オリジナルの独特な仏壇があること。<br class="pc">
            ”ガマ”とは、鹿児島県の方言で洞窟を表す。
          </p>
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/KawabeButsudan"><b>基本情報はこちら</b></a>
        </div>

      </div>

      <h2 class = craft_headline>薩摩焼</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
        </div>

        <div class = explanation>
          <p>
            薩摩焼は、鹿児島県内で焼かれる陶磁器。<br class="pc">
            鉄分が多い土を高温で焼き締めるため、素朴で頑丈な仕上がりが特徴。<br class="pc">
           「白もん」と呼ばれる豪華絢爛な色絵錦手の陶器と<br class="pc">「黒もん」と呼ばれる大衆向けの雑器に分かれる。
          </p>
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/SatsumaPorcelain"><b>基本情報はこちら</b></a>
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
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3">
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
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  .pc {
    display: none;  /* スマホではこのスタイルは起動しない */
  }

  main {
    max-width: 480px;
    margin: 0 auto;
  }

  h1 {
    text-align: center;
    margin-bottom: 0;
  }

  .craft {
    text-align: center;
  }

  h2.craft_headline {
    margin: 0;
    text-align: center;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  .link-space {
    margin: 8px 0;
  }

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
  
/* 工芸品画像 */
  .craft_img img{
    width: 8cm;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }
  
  h1 {
    margin-bottom: 0;
  }
  
/* 工芸品一覧説明 */
  .craft {
    display: flex;
    margin-bottom: 16px;
  }

  .craft p {
    margin: 0;
    font-size: 15px;
  }

  h2.craft_headline {
    margin: 0;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  .explanation {
    margin: auto;
    width: 17cm;
  }

  .link-space {
    align-self: end;
  }

  .link-space a {
    margin: 0;
    font-size: 14px;
  }
  
  .explanation-link {
    text-decoration: none;
    color: blue;
  }

  a:hover.explanation-link {
    color: rgb(71, 1, 92);
  }

/* 工芸品画像 */
  .craft_img img{
    width: 5cm;
    height: auto;
  }
}
</style>