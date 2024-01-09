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
          <p>
            集成館では高炉や鑽開台の動力源として水車を使用しており、水が必要だったため、新たな水路をこの場所に築いた。<br class="pc">
            世界文化遺産「明治日本の産業革命遺産」の構成資産。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/SekiyoshinoSosuiko">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>寺山炭窯跡</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
        <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
        </div>

        <div class = explanation>
          <p>
            集成館事業で使用する白炭を増産するために建設した寺山炭窯の跡。<br class="pc">
            炭窯は斜面を造成して凝灰岩を積み上げて建設、その大きさは国内最大級。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/TerayamaCharcoalKiln">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館「反射炉跡」</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
          <div class="teikyou">
            <p><b>写真協力</b></p>
            <p><b>公益社団法人 鹿児島県観光連盟</b></p>
          </div>
        </div>

        <div class = explanation>
          <p>
            1851年、薩摩藩主に就任した島津斉彬は、富国強兵・殖産興業を唱え、集成館事業を興した。<br class="pc">
            集成館事業の中核となったのが、鹿児島市磯に築かれた工場群「集成館」。<br class="pc">
            製鉄大砲鋳造、洋式艦船の建造、製鉄や紡績、ガラス製造、活版印刷などがおこなわれた。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ReverberatoryFurnaceRuins">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館「旧鹿児島紡績所技師館」（異人館）</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Ijinkan.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
          <div class="teikyou">
            <p><b>写真協力</b></p>
            <p><b>公益社団法人 鹿児島県観光連盟</b></p>
          </div>
        </div>

        <div class = explanation>
          <p>
            日本で最初期の木造西洋建築。<br class="pc">
            西欧人たちがアジアなどの植民地によく建設したコロニアル様式の建物。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/Ijinkan">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館機械工場（尚古集成館）</h2>
      <div class="worldheritage_last">
        <div class = worldheritage_img>
          <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
        </div>

        <div class = explanation>
          <p>
            洋式船や蒸気機関の修理、部品製造を行った集成館の機械工場。<br class="pc">
            竹下清右衛門は長崎製鉄所などの西洋式の建物を参考に工場を建設。<br class="pc">
            現在は博物館（尚古集成館）として島津家や集成館事業の歴史を学ぶことができる。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ShokoShuseikanMuseum">スポット情報</a>
        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
h1 {font-family: 'New Tegomin', serif;}
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
  .pc {display: none;}

  main {
    max-width: 480px;
    margin: 0 auto;
  }

  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  .worldheritage {
    text-align: center;
  }

  .worldheritage_last {
    text-align: center;
  }

  h2.worldheritage_headline {
    margin: 0;
    text-align: center;
    font-size: 22px;
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
  
/* 世界遺産画像 */
  .worldheritage_img img{
    width: 8cm;
    height: auto;
  }

  .teikyou p {
    margin: 0;
    font-size: 14px;
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

  h2.worldheritage_headline {
    margin: 0;
    padding-top: 8px;
    border-top: 2px solid #d5d4c3;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {
    align-self: end;
  }

  .link-space a {
    margin: 0;
    font-size: 14px;
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

/* 提供 */
  .teikyou p {
    font-size: 13px;
  }
}
</style>