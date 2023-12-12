<template>

  <div>
    <TheHeader />

    <main>
      <h1>「県指定伝統工芸品」</h1>
      <h2 class = craft_headline>屋久杉</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Yakusugi.jpg" alt="屋久杉">
        </div>

        <div class = explanation>
          <p>
            世界自然遺産に登録されている「屋久島」は1,000メートル以上の高峰が連なっており、<br class="pc">
            この大自然の中で育った樹齢1,000年以上のものを「屋久杉」と呼んでいる。<br class="pc">
            現在は自然保護のため、倒木や土埋木だけを工芸品として加工している。
          </p>
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/Yakusugi"><b>基本情報はこちら</b></a>
        </div>

      </div>

      <h2 class = craft_headline>薩摩切子</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子">
        </div>

        <div class = explanation>
          <p>
            江戸末期に薩摩藩で造られた切子ガラス。鉛を24～25%含むクリスタルガラスを使用。<br class="pc">
            無色のガラス（クリアガラス）の表面に色ガラスを1～2mm程度溶着させた <br class="pc">
            ”色被せガラス”にカットを施し、磨きあげた製品を「薩摩切子」と言う。
          </p> 
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/SatsumaKiriko"><b>基本情報はこちら</b></a>
        </div>

      </div>

      <h2 class = craft_headline>薩摩つげ櫛</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Tugegushi.jpg" alt="薩摩つげ櫛">
        </div>

        <div class = explanation>
          <p>
            江戸時代から「櫛になりたや薩摩の櫛に、諸国娘の手に渡ろ」とうたわれ、<br class="pc">全国に名を馳せていた。
            材質が硬く、色艶が美しいのが特徴。<br class="pc">
            なめらかな櫛どおりで、静電気・抜け毛・切れ毛が少ないといわれている。
          </p>
        </div>

        <div class="link-space">
          <a class="explanation-link" href="http://localhost:3000/Craft/pages/SatsumaBoxwoodComb"><b>基本情報はこちら</b></a>
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