<template>

  <div>
    <TheHeader />

    <main>
      <h1>豚骨</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonkotsu.jpg" alt="豚骨">
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島県全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>豚骨（スペアリブ）、こんにゃく、大根、ごぼう、焼酎、味噌、砂糖</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              薩摩武士たちが狩場や戦場などでつくった野外料理がはじまりで、かの西郷隆盛も好物であったといわれている。
              「豚骨」には、豚肉と麦味噌、黒砂糖、そして芋焼酎という、鹿児島県ならではの食材がふんだんに盛り込まれているため、今日にいたるまで鹿児島県を代表する郷土料理として親しまれている。
            </dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料（3～4人分）</h3>
        <ul class = "LocalCuisine_memu">

          <li>
            <ul class = "list">
              <li>豚骨（スペアリブ）</li>
              <li class="quantity">400g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>大根</li>
              <li class="quantity">8cm</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>人参</li>
              <li class="quantity">1本</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>こんにゃく</li>
              <li class="quantity">1袋（200g）</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>油</li>
              <li class="quantity">適量</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>焼酎</li>
              <li class="quantity">1/4cup</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>しょうが</li>
              <li class="quantity">1片</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>だし汁</li>
              <li class="quantity">3cup</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>砂糖（おすすめは黒砂糖）</li>
              <li class="quantity">大さじ2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>合わせ味噌</li>
              <li class="quantity">大さじ5</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>酒</li>
              <li class="quantity">大さじ2</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>醤油</li>
              <li class="quantity">大さじ2</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              大根は2cm幅の半月切りに、人参も程よい大きさにカットしておく。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              こんにゃくは味が染みやすいよう切り込みを入れて食べやすい大きさに切り、熱湯で下湯でしておく。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
                フライパンに油を入れて熱し、豚骨を焼き付けて、焼酎を加え水気が無くなるまで煮絡める。（臭みが取れる）
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              圧力鍋に豚骨と☆を加え（味噌は味噌漉しで溶く）１０分加圧する。
            </div>
          </li>

          <li>
            <div class = "num">5</div>
            <div class = "text">
              自然に圧が抜けたら大根・人参・こんにゃくと醤油を入れ、再度5分加圧する。
            </div>
          </li>

          <li>
            <div class = "num">6</div>
            <div class = "text">
              圧が抜けたら落し蓋（クシャクシャにしたアルミホイル使用）をし、味を見ながら煮汁が半量位になるまで煮詰める。
            </div>
          </li>

          <li>
            <div class = "num">7</div>
            <div class = "text">
              前日に仕込んで味を染み込ませまる。表面に脂肪が浮いて来るので丁寧に取り除くことでカロリーダウンになる。
            </div>
          </li>

          <li>
            <div class = "num">8</div>
            <div class = "text">
              温めて器に盛り、お好みで塩茹でしたいんげん等添えると彩りが良い。
            </div>
          </li>

        </ul>
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