<template>

  <div>
    <TheHeader />

    <main>
      <h1>神酒（みき）</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Miki.jpg" alt="みき">
                <p>出典：農林水産省「うちの郷土料理」</p>
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>奄美地域</p>
                <h2>食材</h2>
                <p>米粉、白砂糖、さつまいも、水</p>
                <h2>歴史</h2>
                <p>祭り事の際に神に捧げられた口噛み酒がルーツであるという。
                   口噛み酒は、若い女性が口に含み、2噛みから3噛みほどした米を混ぜてつくった酒のこと。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（パック1本分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>米粉</li>
                <li>500g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>水</li>
                <li>1.4L</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>さつまいも</li>
                <li>100g（なるべく色が薄いもの）</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>白砂糖</li>
                <li>100g</li>
              </ul>
            </li>

          </ul>

          <h3>作り方</h3>

          <ul class = "LocalCuisine_make">
            
            <li>
              <div class = "num">1</div>
              <div class = "text">
                大きな鍋に湯を沸かし、その中に米粉を少しずつ入れてよくかき混ぜていく。
                米粉が溶けたら砂糖を入れて15～20分間、加熱しながらかき混ぜる。
              </div>
            </li>

            <li>
              <div class = "num">2</div>
              <div class = "text">
                さつまいもをすり下ろし、絞り汁をとっておく。
              </div>
            </li>

            <li>
              <div class = "num">3</div>
              <div class = "text">
                【1】の鍋を30℃くらいに冷まし、さつまいもの絞り汁を入れて混ぜる。
              </div>
            </li>

            <li>
              <div class = "num">4</div>
              <div class = "text">
                壺やパックなどに入れ、ふたをして冷暗所におく。夏は一晩、冬は二～三晩おく。途中、木べらなどでかき混ぜる。
              </div>
            </li>

          </ul>

          <div class = "offer">
            <p>レシピ提供元名 : 「奄美の食と文化」（久留ひろみ著）</p>
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

      .LocalCuisine_note {
        margin-top: 1.2cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 0 auto;
      }

    /*材料*/
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