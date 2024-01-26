<template>

  <div>
    <TheHeader />

    <main>
      <h1>神酒（みき）</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Miki.jpg" alt="みき">
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
            <dd>米粉、白砂糖、さつまいも、水</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              祭り事の際に神に捧げられた口噛み酒がルーツであるという。
              口噛み酒は、若い女性が口に含み、2噛みから3噛みほどした米を混ぜてつくった酒のこと。
            </dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料（パック1本分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>米粉</li>
              <li class="quantity">500g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>水</li>
              <li class="quantity">1.4L</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>さつまいも</li>
              <li class="quantity">100g（なるべく色が薄いもの）</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>白砂糖</li>
              <li class="quantity">100g</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              大きな鍋に湯を沸かし、その中に米粉を少しずつ入れてよくかき混ぜていく。
              米粉が溶けたら砂糖を入れて15～20分間、加熱しながらかき混ぜる。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              さつまいもをすり下ろし、絞り汁をとっておく。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              【1】の鍋を30℃くらいに冷まし、さつまいもの絞り汁を入れて混ぜる。
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              壺やパックなどに入れ、ふたをして冷暗所におく。夏は一晩、冬は二～三晩おく。途中、木べらなどでかき混ぜる。
            </div>
          </li>

        </ul>

        <div class = "offer">
          <p>レシピ提供元名 : 「奄美の食と文化」（久留ひろみ著）</p>
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

/* 提供文字 */
.teikyou {font-weight: bold;} /* 文字の太さ */

.teikyou p {margin: 0;} /* 要素の外側余白 */

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

/* 提供文字 */
  .teikyou p {margin: 8px 0;} /* 要素の外側余白 */

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