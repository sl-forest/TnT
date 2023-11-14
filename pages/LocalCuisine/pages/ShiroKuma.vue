<template>

  <div>
    <TheHeader />

    <main>
      <h1>白熊</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Shirokuma.jpg" alt="白熊">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>氷、練乳、小豆、果物</p>
                <h2>歴史</h2>
                <p>諸説あるが、昭和7年頃、鹿児島のある綿屋さんが夏の副業にかき氷屋を営んでおり、かき氷に練乳をかけフルーツをトッピングした高級かき氷として登場したのが始まりと言われている。</p>
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