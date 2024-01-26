<template>

  <div>
    <TheHeader />

    <main>
      <h1>豚汁</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonjiru.jpg" alt="豚汁">
          <div class="teikyou">
            <p>写真協力：公益社団法人 鹿児島県観光連盟</p>
          </div>
        </div>
          
        <div class = localcuisine_note>
          
          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>豚肉、大根、人参、里芋、こんにゃく、厚揚げ、味噌</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              諸説あり定かではないが薩摩汁の豚を使うものが独立した説がある。
              日本全国で獣肉食が広まったのは明治時代以降であるが、琉球と薩摩地方だけは例外的に豚を含めた獣肉食の習慣があり、
              地方料理に肉入りの味噌汁があった。
            </dd>
          </dl>
        </div>
      </div>

      <div class = "recipe">
        <h3>材料</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>豚肉薄切り</li>
              <li class="quantity">80g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>大根</li>
              <li class="quantity">100g</li>
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
              <li>里芋</li>
              <li class="quantity">100g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>こんにゃく</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>油揚げ</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【薬味】小ねぎ、しょうが</li>
              <li class="quantity">適量</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】いりこ</li>
              <li class="quantity">20g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】水</li>
              <li class="quantity">3カップ</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】麦味噌</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>油</li>
              <li class="quantity">適宜</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              水にいりこを入れ、30分したら火にかけ、沸騰後3分でいりこを取り出す（いりこ出汁）。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              材料は食べやすい大きさに切り、鍋に油をひき、豚肉を炒め、その後小ねぎ・しょうが以外の食材も加え、
              全体に油が回ったら、1のいりこ出汁を加え、アクを取りながら煮る。柔らかくなったら麦味噌を溶かし入れる。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              器に盛り、小口ぎりの小ねぎと千切りのしょうがをのせる。
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