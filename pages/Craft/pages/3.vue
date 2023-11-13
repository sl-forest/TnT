<template>

  <div>
    <TheHeader />

    <main>
      <h1>「伝統工芸品」</h1>
      <h2 class = craft_headline>太鼓（チヂン）</h2>
      <div class="craft">
        <div class = craft01_img>
          <img src="~/assets/img/Tijin.jpg" alt="太鼓（チヂン）">
        </div>
        
        <div class = explanation>
          <p>奄美地方の島唄・八月踊りの伴奏に欠かせない太鼓。</p> 
          <p> 明治時代以前とから製作されてきた。</p>
        </div>
        <a class ="explanation-link" href="#">詳細はこちら</a>
      </div>

      <h2 class = craft_headline>甲冑（かっちゅう）</h2>
      <div class="craft">
        <div class = craft02_img>
          <img src="~/assets/img/Kattyu.jpeg" alt="甲冑">
          <p>写真協力：</p>
          <p>公益社団法人 鹿児島県観光連盟</p>
        </div>

        <div class = explanation>
          <p>昔ながらの製法を守りながら、映画・テレビなどの時代劇に使用される鎧やかぶとの全国シェア９割以上の生産を誇り、全国各地のお祭りの武者行列などでも使用されている。</p>
        </div>
        <a class ="explanation-link" href="#">詳細はこちら</a>
      </div>        

      <h2 class = craft_headline>竹製品</h2>
      <div class="craft">
        <div class = craft02_img>
          <img src="~/assets/img/bambooproducts.jpg" alt="竹製品">
        </div>

        <div class = explanation>
          <p>鹿児島は竹林面積日本一の「竹」のふるさと。</p>
          <p>古くから竹を使って様々な生活道具が作られており、庶民生活には欠かせないもの。</p>
        </div>
        <a class ="explanation-link" href="http://localhost:3000/Craft/pages/BambooProducts">詳細はこちら</a>
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
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
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
      
      /* 工芸品一覧説明 */
      .craft {
        display: flex;
      }

      .craft p {
        margin: 0;
        font-size: 14px;
      }

      h2.craft_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }

      .explanation {
        margin: auto;
        width: 44em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 工芸品画像 */
      .craft01_img img{
        width: 4.5cm;
        height: auto;
      }

      .craft02_img img{
        width: 4.5cm;
        height: 4cm;
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