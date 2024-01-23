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
            集成館では高炉や鑽開台の動力源として水車を使用しており、水が必要だったため、<br>
            新たな水路をこの場所に築いた。<br>
            世界文化遺産「明治日本の産業革命遺産」の構成資産。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/SekiyoshinoSosuiko">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>寺山炭窯跡</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
        <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
        </div>

        <div class = explanation>
          <p>
            集成館事業で使用する白炭を増産するために建設した寺山炭窯の跡。<br>
            炭窯は斜面を造成して凝灰岩を積み上げて建設、その大きさは国内最大級。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/TerayamaCharcoalKiln">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館「反射炉跡」</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
          <div class="teikyou">
            <p>
              写真協力：<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            1851年、薩摩藩主に就任した島津斉彬は、富国強兵・殖産興業を<br>
            唱え、集成館事業を興した。<br>
            集成館事業の中核となったのが、鹿児島市磯に築かれた工場群「集成館」。<br>
            製鉄大砲鋳造、洋式艦船の建造、製鉄や紡績、ガラス製造、活版印刷などが<br>
            おこなわれた。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/ReverberatoryFurnaceRuins">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline_small>旧集成館「旧鹿児島紡績所技師館」（異人館）</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Ijinkan.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
          <div class="teikyou">
            <p>
              写真協力：<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            日本で最初期の木造西洋建築。<br>
            西欧人たちがアジアなどの植民地によく建設したコロニアル様式の建物。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/Ijinkan">スポット情報</a>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館機械工場（尚古集成館）</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
        </div>

        <div class = explanation>
          <p>
            洋式船や蒸気機関の修理、部品製造を行った集成館の機械工場。<br>
            竹下清右衛門は長崎製鉄所などの西洋式の建物を参考に工場を建設。<br>
            現在は博物館（尚古集成館）として島津家や集成館事業の歴史を学ぶことができる。
          </p>
        </div>
        <div class="link-space">
          <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/ShokoShuseikanMuseum">スポット情報</a>
        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}       /* 要素の外側余白 */

main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;                          /* 要素の外側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

h2.worldheritage_headline {
  margin: 0px;                       /* 全余白の指定 */
  padding: 8px 0px;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

h2.worldheritage_headline_small {
  margin: 0px;                       /* 全余白の指定 */
  padding: 8px 0px;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

/* 提供 */
.teikyou {font-weight: bold;} /* 文字の太さ */

.teikyou p {
  margin: 0px;        /* 全余白の指定 */
  font-size: 13px;    /* 文字の大きさ */
}

.explanation p {
  margin: 0px;          /* 全余白の指定 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 16px;      /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;
  padding: 0.3em 1.2em;
  text-decoration: none;
  color: black;
  border: solid 2px black;
  border-radius: 3px;
  transition: .4s;
}

.btn:hover {
  background: black;
  color: white;
}

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

.Pagination-Item-Link-Icon {width: 20px;}

.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */
  
  br {display: none;}     /* 表示しない */

  h1 {
    padding: 8px 0px;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
  }

  .worldheritage {text-align: center;}

  h2.worldheritage_headline {text-align: center;}

  h2.worldheritage_headline_small {
    text-align: center;
    font-size: 22px;
  }

  .link-space {margin: 16px 0;}

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px;
  }
  
/* 画像 */
  .worldheritage_img img {width: 80%;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .worldheritage {
    display: flex;
    margin-bottom: 16px;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

/* 画像 */
  .worldheritage_img img {width: 5cm;}
}
</style>