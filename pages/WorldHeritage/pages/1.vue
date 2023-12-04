<template>

  <div>
    <TheHeader />

    <main>
      <h1>「世界遺産」</h1>
      <h2 class = worldheritage_headline>関吉の疎水溝</h2>
      <div class="worldheritage">
          <div class = worldheritage_img>
            <img src="~/assets/img/Sekiyoshi.jpg" alt="関吉の疎水溝">
          </div>
          
          <div class = explanation>
            <p>集成館では高炉や鑽開台の動力源として水車を使用しており、水が必要だったため、新たな水路をこの場所に築いた。</p>
            <p>世界文化遺産「明治日本の産業革命遺産」の構成資産。</p>
          </div>
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/SekiyoshinoSosuiko">スポット情報</a>
      </div>

      <h2 class = worldheritage_headline>寺山炭窯跡</h2>
      <div class="worldheritage">
          <div class = worldheritage_img>
          <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
          </div>

          <div class = explanation>
            <p>集成館事業で使用する白炭を増産するために建設した寺山炭窯の跡。</p>
            <p>炭窯は斜面を造成して凝灰岩を積み上げて建設、その大きさは国内最大級。</p>
          </div>
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/TerayamaCharcoalKiln">スポット情報</a>
      </div>

      <h2 class = worldheritage_headline>旧集成館「反射炉跡」</h2>
      <div class="worldheritage">
          <div class = worldheritage_img>
            <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
            <p>写真協力：</p>
            <p>公益社団法人　鹿児島県観光連盟</p>
          </div>

          <div class = explanation>
            <p>1851年、薩摩藩主に就任した島津斉彬は、富国強兵・殖産興業を唱え、集成館事業を興した。</p>
            <p>集成館事業の中核となったのが、鹿児島市磯に築かれた工場群「集成館」。</p>
            <p>製鉄大砲鋳造、洋式艦船の建造、製鉄や紡績、ガラス製造、活版印刷などがおこなわれた。</p>
          </div>
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ReverberatoryFurnaceRuins">スポット情報</a>
      </div>

      <h2 class = worldheritage_headline>旧集成館「旧鹿児島紡績所技師館」（異人館）</h2>
      <div class="worldheritage">
          <div class = worldheritage_img>
            <img src="~/assets/img/Ijinkan.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
            <p>写真協力：</p>
            <p>公益社団法人　鹿児島県観光連盟</p>
          </div>

          <div class = explanation>
            <p>日本で最初期の木造西洋建築。</p>
            <p>西欧人たちがアジアなどの植民地によく建設したコロニアル様式の建物。</p>
            <p></p>
          </div>
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/Ijinkan">スポット情報</a>
      </div>

      <h2 class = worldheritage_headline>旧集成館機械工場（尚古集成館）</h2>
      <div class="worldheritage_last">
          <div class = worldheritage_img>
            <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
          </div>

          <div class = explanation>
            <p>洋式船や蒸気機関の修理、部品製造を行った集成館の機械工場。</p>
            <p>竹下清右衛門は長崎製鉄所などの西洋式の建物を参考に工場を建設。</p>
            <p>現在は博物館（尚古集成館）として島津家や集成館事業の歴史を学ぶことができる。</p>
          </div>
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ShokoShuseikanMuseum">スポット情報</a>
      
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

      h1 {
        margin-bottom: 0;
      }

      h2.worldheritage_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 世界遺産一覧説明 */
      .worldheritage {
        display: flex;
      }

      .worldheritage_last {
        display: flex;
        margin-bottom: 16px;
      }

      .worldheritage p {
        margin: 0;
        font-size: 14px;
      }

      .worldheritage_last p {
        margin: 0;
        font-size: 14px;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
        text-decoration: none;
        color: blue;
      }

      a:hover.explanation-link {
        color: rgb(71, 1, 92);
      }

      /* 世界遺産画像 */
      .worldheritage_img img{
        width: 5cm;
        height: auto;
      }
    }

</style>