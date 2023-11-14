<template>

  <div>
    <TheHeader />

    <main>
      <h1>黒糖</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Kokutou.jpg" alt="黒糖">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>奄美地域</p>
                <h2>食材</h2>
                <p>さとうきび</p>
                <h2>歴史</h2>
                <p>元禄時代（１６８８年）、日本に黒糖（黒砂糖）は伝わった。江戸時代より沖縄、奄美大島、種子島などで生産されており、沖縄で黒糖（黒砂糖）は“ヌチグスイ（命薬）”と呼ばれ薬として飲まれていたこともある。</p>
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
    }
</style>