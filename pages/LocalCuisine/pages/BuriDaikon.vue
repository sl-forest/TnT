<template>

  <div>
    <TheHeader />

    <main>
      <h1>ぶり大根</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Buridaikon.jpg" alt="ぶり大根">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>大根、ブリ</p>
                <h2>歴史</h2>
                <p>内湾が多く、ブリの稚魚のモジャコがとれる鹿児島県はブリの養殖生産量で全国1位。なかでも養殖ブリの生産量日本一を誇る長島町では、厳しい管理基準を設け育った養殖ブリを「鰤王」と名付け、国内のみならず、海外への輸出もおこなっている。また、垂水（たるみず）市や鹿屋（かのや）市、南大隅町などでもブリの養殖は盛んにおこなわれている。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>ぶりの切り身</li>
                <li>50g×4切れ</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>ブリのあら</li>
                <li>200g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>大根</li>
                <li>500g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>しょうが</li>
                <li>50cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>酒</li>
                <li>50cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】濃口醤油</li>
                <li>大さじ2～3</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】淡口醤油</li>
                <li>大さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【A】本みりん</li>
                <li>大さじ4～5</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>【A】砂糖</li>
                <li>お好みで</li>
              </ul>
            </li>
          </ul>

          <h3>作り方</h3>

          <ul class = "LocalCuisine_make">
            
            <li>
              <div class = "num">1</div>
              <div class = "text">
                大根は3cm厚さの輪切りで面取りをし、片面に十字に浅く切り目を入れ下ゆでする。しょうがは半分を薄切りにし、残りは千切りにする。
              </div>
            </li>

            <li>
              <div class = "num">2</div>
              <div class = "text">
                ブリは水洗いし、熱湯にくぐらせ、血合いやぬめりを取る。
              </div>
            </li>

            <li>
              <div class = "num">3</div>
              <div class = "text">
                鍋に大根・ブリ・酒・薄切りのしょうがを入れ、ひたひたになる程度に水を加え、強火で煮立て、沸騰したら中火にしてアクをとりながら15分ほど煮る。
              </div>
            </li>

            <li>
              <div class = "num">4</div>
              <div class = "text">
                【A】の調味料を加え、味が染みるまで弱火で煮る。甘みが強い方が良い場合は好みで砂糖を加える。
                一晩おくと大根に煮汁が染みこんでさらに美味しくなる。
              </div>
            </li>

            <li>
              <div class = "num">5</div>
              <div class = "text">
                器に盛り付け、千切りのしょうがを飾る。
              </div>
            </li>

          </ul>
          
          <div class = "offer">
            <p>レシピ提供元名 : NPO法人霧島食育研究会</p>
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

    /*材料*/
      .LocalCuisine_note {
        margin-top: 0;
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