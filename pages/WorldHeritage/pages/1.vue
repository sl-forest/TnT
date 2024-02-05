<template>

  <div>
    <TheHeader />

    <main>
      <h1>「世界遺産」</h1>
      <h2 class = worldheritage_headline>関吉の疎水溝</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Sekiyoshi-min.jpg" alt="関吉の疎水溝">
        </div>
        
        <div class = explanation>
          <p>
            集成館では高炉や鑽開台の動力源として水車を使用しており、水が必要だったため、<br>
            新たな水路をこの場所に築いた。<br>
            世界文化遺産「明治日本の産業革命遺産」の構成資産。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/SekiyoshinoSosuiko">関吉の疎水溝はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = worldheritage_headline>寺山炭窯跡</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
        <img src="~/assets/img/Sumigamaato-min.jpg" alt="寺山炭窯跡">
        </div>

        <div class = explanation>
          <p>
            集成館事業で使用する白炭を増産するために建設した寺山炭窯の跡。<br>
            炭窯は斜面を造成して凝灰岩を積み上げて建設、その大きさは国内最大級。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/TerayamaCharcoalKiln">寺山炭窯跡はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館「反射炉跡」</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Reverberatory furnace ruins-min.jpeg" alt="旧集成館「反射炉跡」">
          <div class="teikyou">
            <p>
              写真協力：<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            1851年、薩摩藩主に就任した島津斉彬は、富国強兵・殖産興業を唱え、集成館事業を興した。<br>
            集成館事業の中核となったのが、鹿児島市磯に築かれた工場群「集成館」。<br>
            製鉄大砲鋳造、洋式艦船の建造、製鉄や紡績、ガラス製造、活版印刷などがおこなわれた。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/ReverberatoryFurnaceRuins">旧集成館「反射炉跡」はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = worldheritage_headline_small>旧集成館「旧鹿児島紡績所技師館」（異人館）</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Ijinkan-min.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
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
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/Ijinkan">旧集成館「旧鹿児島紡績所技師館」（異人館）はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = worldheritage_headline>旧集成館機械工場（尚古集成館）</h2>
      <div class="worldheritage">
        <div class = worldheritage_img>
          <img src="~/assets/img/Shoko Shuseikan Museum-min.jpg" alt="旧集成館機械工場（尚古集成館）">
        </div>

        <div class = explanation>
          <p>
            洋式船や蒸気機関の修理、部品製造を行った集成館の機械工場。<br>
            竹下清右衛門は長崎製鉄所などの西洋式の建物を参考に工場を建設。<br>
            現在は博物館（尚古集成館）として島津家や集成館事業の歴史を学ぶことができる。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/WorldHeritage/pages/ShokoShuseikanMuseum">旧集成館機械工場（尚古集成館）はこちら</a>
          </div>
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
  margin: 0;                       /* 全余白の指定 */
  padding: 8px 0;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3; /* 上線 */
}

h2.worldheritage_headline_small {
  margin: 0;                        /* 全余白の指定 */
  padding: 8px 0;                   /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;  /* 上線 */
}

/* 提供 */
.teikyou {font-weight: bold;} /* 文字の太さ */

.teikyou p {
  margin: 0;        /* 全余白の指定 */
  font-size: 13px;  /* 文字の大きさ */
}

.explanation p {
  margin: 0;           /* 全余白の指定 */
  font-family: serif;  /* フォントの変更 */
  font-weight: bold;   /* 文字の太さ */
  font-size: 16px;     /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;      /* インラインブロック要素へ変更 */
  padding: 0.3em 0.6em;       /* 要素の内側余白 */
  text-decoration: none;      /* 下線無効 */
  color: black;             /* 文字の色 */
  border: solid 2px black;  /* 枠線 */
  border-radius: 3px;         /* 要素の境界の外側の角を丸める */
  transition: .4s;            /* 要素の2つの状態間の変化を定義する */
}

/* マウスオーバー */
.btn:hover {
  background: black;  /* 背景 */
  color: white;       /* 文字の色 */
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */
  br {display: none;}     /* 表示しない */

  h1 {
    padding: 8px 0;       /* 要素の内側余白 */
    text-align: center;   /* 中央揃え */
  }

  .worldheritage {text-align: center;}            /* 中央揃え */
  h2.worldheritage_headline {text-align: center;} /* 中央揃え */

  h2.worldheritage_headline_small {
    text-align: center; /* 中央揃え */
    font-size: 22px;    /* 文字の大きさ */
  }

  .link-space {margin: 16px 0;} /* 要素の外側余白 */

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px; /* 要素の外側上余白 */
  }
  
/* 画像 */
  .worldheritage_img img {
    width: 320px; /* 横幅 */
    height: auto; /* 高さ */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .worldheritage {
    display: flex;        /* 親要素に対して子要素を横並び */
    margin-bottom: 16px;  /* 要素の外側下余白 */
    column-gap: 1rem;     /* 行や列の間のすき間を定義 */
  }

  .explanation {align-self: center;}  /* 中央揃え */
  .link-space {margin-top: 0.5rem;}   /* 要素の外側上余白 */

/* 画像 */
  .worldheritage_img img {
    width: 200px; /* 横幅 */
    height: auto; /* 高さ */
  }
}
</style>