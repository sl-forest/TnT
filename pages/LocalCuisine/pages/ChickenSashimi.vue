<template>

  <div>
    <TheHeader />

    <main>
      <h1>鳥刺し</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Torisashi02.jpeg" alt="鳥刺し">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>鶏肉</p>
                <h2>歴史</h2>
                <p>鹿児島県では、江戸時代から薩摩武士たちが士風高揚のため、盛んに闘鶏をおこなっており、その際に負けた鶏をその場でしめて食べる習慣があった。闘鶏が禁止された後も、各家庭で鶏が飼われ、来客がある時や祝いの席のために鶏をしめて調理し食べていたという。このように鹿児島県においては、古くから鶏肉を使った料理が身近でにあったことから、鶏肉を刺身で食べる「鶏刺し」が根づいたと考えられてる。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>鶏刺し用鶏肉（もも・ささみ・むね肉）</li>
                <li>150g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>玉ねぎ</li>
                <li>30g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>ねぎ</li>
                <li>5g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>しょうが</li>
                <li>お好みで</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>にんにく</li>
                <li>お好みで</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>青じそ</li>
                <li>お好みで</li>
              </ul>
            </li>

          </ul>

          <h3>作り方</h3>

          <ul class = "LocalCuisine_make">
            
            <li>
              <div class = "num">1</div>
              <div class = "text">
                鶏刺し用の新鮮な鶏肉を用意する。
              </div>
            </li>

            <li>
              <div class = "num">2</div>
              <div class = "text">
                バーナーなどで皮目をあぶり、表面の色が変わったら火を止める。（中は生のまま）
              </div>
            </li>

            <li>
              <div class = "num">3</div>
              <div class = "text">
                  3mm幅に皮目から切る。肉の繊維の方向を見て繊維を断ち切るようにくらいの刺身に切る。
              </div>
            </li>

            <li>
              <div class = "num">4</div>
              <div class = "text">
                青じそを敷き部位ごとに盛り付け玉ねぎはスライス、ネギは小口切り。しょうがニンニクはすりおろして一緒に盛り付け、好みで醤油やポン酢で味わう。
              </div>
            </li>

          </ul>

          <div class = "offer">
            <p>レシピ提供元名 : 株式会社Table of Smile</p>
            <p>※レシピは地域・家庭によって違いがあります。</p>
          </div>

        </div>
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
      
    /*郷土料理説明*/
      .LocalCuisine {
        display: flex;
        padding-bottom: 24px;
      }

      .LocalCuisine h1 {
        margin: 1.6px auto;
      }

      .LocalCuisine_img img {
        height: 12cm;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 1.8cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 8px auto;
      }

      .recipe {
        background: #d2e7f3;
        padding: 24px;
        margin-bottom: 24px;
      }

      .recipe h3 {
        margin: 0;
        padding: 0;
        border-bottom: 1px solid #1b1b1b;
      }

      .list {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 6px;
        border-bottom: 1px solid #9e9595;
      }

      .list_last {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 64px;
      }

    /*作り方*/
      .LocalCuisine_make {
        list-style: none;
        margin: 0;
        font-size: 1em;
        padding: 0;
      }

      .LocalCuisine_make li {
        display: table;
        padding: 16px 0;
        border-bottom: 1px solid #9e9595;
      }

      .num {
        display: inline-block;
        font-size: 1.714em;
        width: 40px;
        margin-top: -5px;
        padding-right: 10px;
      }

      .text {
        display: table-cell;
        vertical-align: top;
        width: 100%;
      }

    /*提供*/
      .offer {
        margin: 16px 0px 0px 0px;
        text-align: right;
      }

      .offer p {
        margin: 4px 0px 0px 0px;
        font-size: 80%;
      }
    }
</style>