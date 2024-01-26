<template>

  <div>
    <TheHeader />

    <main>
      <h1>がね</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Gane.jpg" alt="がね">
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島県全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>さつまいも、人参、ニラ、小麦粉</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              「がね」は、さつまいもや野菜を太めの千切りにし、衣をつけて揚げる料理。その見た目が“かに（鹿児島弁でがねという）”に似ていることからこの名がついた。
              砂糖を多く入れ甘めな味付けが特徴で地域により具材や衣の材料は違う。
            </dd>
          </dl>
            
        </div>
      </div>

      <div class = "recipe">
        <h3>材料（8～10個分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>さつまいも</li>
              <li class="quantity">200g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>人参</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>ニラ</li>
              <li class="quantity">30g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】小麦粉</li>
              <li class="quantity">100g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】もち米粉</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】砂糖</li>
              <li class="quantity">40g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】卵</li>
              <li class="quantity">1個</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】淡口醤油</li>
              <li class="quantity">大さじ1.5</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】塩</li>
              <li class="quantity">ふたつまみ</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【衣】水</li>
              <li class="quantity">80cc</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>油</li>
              <li class="quantity">適量</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              さつまいもは薄く皮を剥き（ところどころ皮を残す）、5mm角×7～8cmの細切りにする。
              ボウルに水を張り、さつまいもが完全に浸るようにさらしてざるに開ける。
              人参は薄く皮を剥き、さつまいもより短めの2～3cmに切る。ニラは7～8cmの長さに切る。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              ボウルに1と水以外の材料を加えながら衣が具にまとわりつく感じになるまで混ぜる。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              鍋に油を3cm以上の深さになるように入れて、170度になるように熱する。（臭みが取れる）
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              木杓子で具をすくい、横長にカニの姿のようにかたちをととのえる。
              菜箸で向こう側に押すように鍋に落とし、2、3分でひっくり返し、さつまいもの甘い匂いがしてきて全体がきつね色になったら揚げ上がり。
              バットにキッチンペーパーを敷き、立てて並べると油の切れが良い。
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
/* 共通 */
body {margin: 0;}       /* 要素の外側余白 */

main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;            /* 要素の外側余白 */
  padding: 8px 0;       /* 要素の内側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

.quantity {list-style-type: none;}  /* 点削除 */

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

  .localcuisine_img img {width: 400px;}   /* 横幅 */

/*材料*/
  .localcuisine_note {margin-top: 16px;}    /* 要素の外側上余白 */

  .localcuisine_note dl {font-size: 16px;}  /* 文字の大きさ */

  .localcuisine_note dt {width: 30%;}   /* 横幅 */

  .localcuisine_note dd {width: 12cm;}  /* 横幅 */

  .localcuisine_note > dd {
    border: 1px solid #ddd; /* 枠線 */
    border-top: none;         /* 上線削除 */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

/*郷土料理説明*/
  .localcuisine {display: flex;}  /* 親要素に対して子要素を横並び */

/* 画像 */
  .localcuisine_img img {width: 400px;} /* 横幅 */

/*材料*/
  .localcuisine_note {
    margin: auto;       /* 要素の外側余白 */
    margin-left: 16px;  /* 要素の外側左余白 */
  }

  .localcuisine_note dl {font-size: 18px;}  /* 文字の大きさ */

  .localcuisine_note dt {width: 25%;}   /* 横幅 */

  .localcuisine_note dd {width: 16cm;}  /* 横幅 */
}
</style>