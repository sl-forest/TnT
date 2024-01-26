<template>

  <div>
    <TheHeader />

    <main>
      <h1>ぶり大根</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Buridaikon.jpg" alt="ぶり大根">
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島県全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>大根、ブリ</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              内湾が多く、ブリの稚魚のモジャコがとれる鹿児島県はブリの養殖生産量で全国1位。
              なかでも養殖ブリの生産量日本一を誇る長島町では、厳しい管理基準を設け育った養殖ブリを「鰤王」と名付け、
              国内のみならず、海外への輸出もおこなっている。
            </dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>ぶりの切り身</li>
              <li class="quantity">50g×4切れ</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>ブリのあら</li>
              <li class="quantity">200g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>大根</li>
              <li class="quantity">500g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>しょうが</li>
              <li class="quantity">50cc</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>酒</li>
              <li class="quantity">50cc</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【A】濃口醤油</li>
              <li class="quantity">大さじ2～3</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【A】淡口醤油</li>
              <li class="quantity">大さじ2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【A】本みりん</li>
              <li class="quantity">大さじ4～5</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>【A】砂糖</li>
              <li class="quantity">お好みで</li>
            </ul>
          </li>
        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
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