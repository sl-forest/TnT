<template>

  <div>
    <TheHeader />

    <main>
      <h1>油ゾーメン</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Zomen.jpg" alt="油ゾーメン">
          <div class="teikyou">
            <p>出典：農林水産省「うちの郷土料理」</p>
          </div>
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>奄美地域</dd>
          </dl>

          <dl>
            <dt>材料</dt>
            <dd>豚肉、そうめん、ニラ、いりこ、だし汁</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              薩摩藩統治時代に薩摩から持ち込まれ、乾麺で保存がきくことから奄美地域でよく食べられるようになったのではないかという
              説があるが、定かではない。
            </dd>
          </dl>
        </div>
      </div>
      
      <div class = "recipe">
        <h3>材料（4人分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>塩豚肉（豚もも肉でも良い）</li>
              <li>120g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>そうめん</li>
              <li>180g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>ニラ</li>
              <li>180g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>いりこ</li>
              <li>12g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>サラダ油</li>
              <li>大さじ2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>だし汁</li>
              <li>2cup</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>醤油</li>
              <li>大さじ1・1/2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>塩、こしょう</li>
              <li>各少々</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>ごま油</li>
              <li>小さじ2</li>
            </ul>
          </li>

        </ul>
          
        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              ［塩豚肉のつくり方］三枚肉のかたまり（300g）の表面全体に塩をすりこむようにしてまぶす。
              ビニール袋に入れて冷蔵庫で保存する（1週間程度保存できる）。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              豚肉は熱湯で三度塩抜きをする。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              豚肉は細切りにしておく。
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              そうめんは少しかためにゆでて、ざるに上げておく。
            </div>
          </li>

          <li>
            <div class = "num">5</div>
            <div class = "text">
              ニラは2cmの長さに切っておく。
            </div>
          </li>

          <li>
            <div class = "num">6</div>
            <div class = "text">
              中華鍋に油を引き、豚肉を炒める。
            </div>
          </li>

          <li>
            <div class = "num">7</div>
            <div class = "text">
              6にいりことそうめんを入れ、混ぜながら炒める。
            </div>
          </li>

          <li>
            <div class = "num">8</div>
            <div class = "text">
              7にだし汁をまわし入れる。
            </div>
          </li>

          <li>
            <div class = "num">9</div>
            <div class = "text">
              8に醤油を回し入れる。
            </div>
          </li>

          <li>
            <div class = "num">10</div>
            <div class = "text">
              9に塩、こしょうをふり、ニラを入れ混ぜ、最後にごま油を入れる。
            </div>
          </li>
          
        </ul>

        <div class = "offer">
          <p>レシピ提供元名 : 「郷土の味」（鹿児島県食生活改善推進員連絡協議会）</p>
          <p>※レシピは地域・家庭によって違いがあります。</p>
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
  padding: 8px 0;                     /* 要素の内側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

.quantity {list-style-type: none;}  /* 点削除 */

/* 提供文字 */
.teikyou {font-weight: bold;} /* 文字の太さ */
.teikyou p {margin: 0;}       /* 要素の外側余白 */

/*郷土料理説明*/
.localcuisine {padding-bottom: 24px;} /* 要素の内側下余白 */

.localcuisine_note dl {
  margin: 3px 0;                /* 要素の外側余白 */
  overflow: hidden;             /* 要素からはみ出た部分を非表示 */
  display: flex;                /* 親要素に対して子要素を横並びにする */
  align-items: center;          /* 上下の中央揃え */
  background-color: #e0e2e2;  /* 背景 */
}

.localcuisine_note dt {
  flex-shrink: 0;         /* 縮小値 */
  text-align: center;     /* 左右の中央揃え */
}

.localcuisine_note dd {
  margin: 0;                 /* 要素の外側余白 */
  display: flex;             /* 親要素に対して子要素を横並びにする */
  background-color: #fff;  /* 背景 */
  padding-left: 1%;          /* 要素の内側左余白 */
  flex-grow: 1;              /* 余白の追加 */
}

.recipe {
  padding: 24px;          /* 要素の内側余白 */
  margin-bottom: 24px;    /* 要素の外側下余白 */
  background: #d2e7f3;  /* 背景 */
}

.recipe h3 {
  margin: 0;  /* 要素の外側余白 */
  padding: 0; /* 要素の内側余白 */
  border-bottom: 1px solid #1b1b1b; /* 背景 */
}

.list {
  display: flex;                      /* 親要素に対して子要素を横並び */
  justify-content: space-between;     /* 横並びの要素を両端揃えで均等に配置 */
  padding: 8px 0 6px;                 /* 要素の内側余白 */
  border-bottom: 1px solid #9e9595; /* 要素の外側下余白 */
}

.list_last {
  display: flex;                  /* 親要素に対して子要素を横並び */
  justify-content: space-between; /* 横並びの要素を両端揃えで均等に配置 */
  padding: 8px 0 64px;            /* 要素の内側余白 */
}

/*作り方*/
.localcuisine_make {
  margin: 0;      /* 要素の外側余白 */
  padding: 0;     /* 要素の内側余白 */
  font-size: 1em; /* 文字の大きさ */
}

.localcuisine_make li {
  display: table;   /* 要素にtableタグの特徴を持たせる */
  padding: 16px 0;  /* 要素の内側余白 */
  border-bottom: 1px solid #9e9595; /* 下線 */
}

.num {
  display: inline-block;  /* インラインブロック要素へ変更 */
  font-size: 1.714em;     /* 文字の大きさ */
  width: 40px;            /* 横幅 */
  margin-top: -5px;       /* 要素の外側上余白 */
  padding-right: 10px;    /* 要素の内側右余白 */
}

.text {
  display: table-cell;  /* tableのように要素を横並び */
  vertical-align: top;  /* 上寄せ */
  width: 100%;          /* 横幅 */
}

/*提供*/
.offer {
  margin: 16px 0 0 0; /* 要素の外側余白 */
  text-align: right;  /* 右寄せ */
}

.offer p {
  margin: 4px 0 0 0;  /* 要素の外側余白 */
  font-size: 80%;     /* 文字の大きさ */
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}  /* 要素の外側上余白 */
  h1 {text-align: center;} /* 左右の中央揃え */

/* 画像 */
  .localcuisine_img {text-align: center;} /* 左右の中央揃え */

  .localcuisine_img img {
    width: 400px; /* 横幅 */
    height: auto; /* 高さ */
  }

/* 提供文字 */
  .teikyou p {margin: 8px 0;} /* 要素の外側余白 */

/*材料*/
  .localcuisine_note {margin-top: 16px;}    /* 要素の外側上余白 */
  .localcuisine_note dl {font-size: 16px;}  /* 文字の大きさ */
  .localcuisine_note dt {width: 30%;}       /* 横幅 */

  .localcuisine_note dd {
    padding: 2%;  /* 要素の内側余白 */
    width: 12cm;  /* 横幅 */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

/*郷土料理説明*/
  .localcuisine {display: flex;}  /* 親要素に対して子要素を横並び */

/* 画像 */
  .localcuisine_img img {
    width: 400px; /* 横幅 */
    height: auto; /* 高さ */
  }

/*材料*/
  .localcuisine_note {
    margin: auto;       /* 要素の外側余白 */
    margin-left: 16px;  /* 要素の外側左余白 */
  }

  .localcuisine_note dl {font-size: 18px;}  /* 文字の大きさ */
  .localcuisine_note dt {width: 25%;}       /* 横幅 */
  .localcuisine_note dd {width: 16cm;}      /* 横幅 */
}
</style>