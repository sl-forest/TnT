<template>

  <div>
    <TheHeader />

    <main>
      <h1>かるかん</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Karukan.jpg" alt="かるかん">
                <p>出典：農林水産省「うちの郷土料理」</p>
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>かるかん粉、大和芋、あん</p>
                <h2>歴史</h2>
                <p>諸説あるが、薩摩藩の第11代藩主であった島津斉彬が、保存食の研究のために江戸から招聘した明石出身の菓子職人・八島六兵衛によって考案されたという説が有力とされている。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（10個分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>かるかん粉</li>
                <li>125g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>大和芋</li>
                <li>100g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>砂糖</li>
                <li>150g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>水</li>
                <li>75cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>あん</li>
                <li>110g</li>
              </ul>
            </li>

          </ul>

          <h3>作り方</h3>

          <ul class = "LocalCuisine_make">
            
            <li>
              <div class = "num">1</div>
              <div class = "text">
                あんは10等分し、丸め、中心部を少しへこませたかたちにしておく。
              </div>
            </li>

            <li>
              <div class = "num">2</div>
              <div class = "text">
                大和芋をすりおろし、水を少しづつ加え混ぜる。
              </div>
            </li>

            <li>
              <div class = "num">3</div>
              <div class = "text">
                【2】に砂糖、かるかん粉を加え混ぜ合わせる。
              </div>
            </li>

            <li>
              <div class = "num">4</div>
              <div class = "text">
                かるかん型に【3】を10等分し、あんを中心部におき、楊枝であんの上に生地をかぶせるようにする。
              </div>
            </li>

            <li>
              <div class = "num">5</div>
              <div class = "text">
                蒸気の上がった蒸し器に4を入れ、強火のままで25分蒸し、型から外す。
              </div>
            </li>

          </ul>

          <div class = "offer">
            <p>レシピ提供元名 : NPO法人 霧島食育研究会</p>
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
        height: 10cm;
      }

      .LocalCuisine_img p {
        margin: 0;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 1cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 0 auto;
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