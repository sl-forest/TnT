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

.quantity {list-style-type: none;}

/* 提供文字 */
.teikyou {font-weight: bold;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}  /* 要素の外側上余白 */

  h1 {text-align: center;} /* 左右の中央揃え */

/*郷土料理説明*/
  .localcuisine {padding-bottom: 24px;}

/* 画像 */
  .localcuisine_img {text-align: center;}

  .localcuisine_img img {height: 7cm;}

/* 提供文字 */
  .teikyou p {margin: 8px 0;}

/*材料*/
  .localcuisine_note {margin-top: 16px;}

  .localcuisine_note dl {
    font-size: 16px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .localcuisine_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 30%;
  }

  .localcuisine_note dd {
    width: 12cm;
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }

  .localcuisine_note > dd {
    border: 1px solid #ddd;
    border-top: none;
  }

  .localcuisine_note > dt,
  .localcuisine_note > dd {text-align: center;}

  .localcuisine_note > dd > ul {text-align: left;}

  .recipe {
    background: #d2e7f3;
    padding: 24px;
    margin-bottom: 24px;
  }

  .recipe h3 {
    margin: 0;
    padding: 0;
    border-bottom: 1px solid #1b1b1b;
  }

  .list {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    padding: 8px 0 6px;
    border-bottom: 1px solid #9e9595;
  }

  .list_last {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    padding: 8px 0 64px;
  }

/*作り方*/
  .localcuisine_make {
    list-style: none;
    margin: 0;
    font-size: 1em;
    padding: 0;
  }

  .localcuisine_make li {
    display: table;
    padding: 16px 0;
    border-bottom: 1px solid #9e9595;
  }

  .num {
    display: inline-block;  /* インラインブロック要素へ変更 */
    font-size: 1.714em;
    width: 40px;
    margin-top: -5px;
    padding-right: 10px;
  }

  .text {
    display: table-cell;
    vertical-align: top;
    width: 100%;
  }

/*レシピ提供*/
  .offer {
    margin: 16px 0 0 0;
    text-align: right;
  }

  .offer p {
    margin: 4px 0 0 0;
    font-size: 80%;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

/*郷土料理説明*/
  .localcuisine {
    display: flex;
    padding-bottom: 24px;
  }

/* 画像 */
  .localcuisine_img img {height: 8cm;}

/* 提供文字 */
  .teikyou p {margin: 0;}

/*材料*/
  .localcuisine_note {
    margin: auto;
    margin-left: 16px;
  }

  .localcuisine_note dl {
    font-size: 18px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .localcuisine_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 25%;
  }

  .localcuisine_note dd {
    width: 14cm;
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }

  .recipe {
    background: #d2e7f3;
    padding: 24px;
    margin-bottom: 24px;
  }

  .recipe h3 {
    margin: 0;
    padding: 0;
    border-bottom: 1px solid #1b1b1b;
  }

  .list {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    padding: 8px 0 6px;
    border-bottom: 1px solid #9e9595;
  }

  .list_last {
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    padding: 8px 0 64px;
  }

/*作り方*/
  .localcuisine_make {
    list-style: none;
    margin: 0;
    font-size: 1em;
    padding: 0;
  }

  .localcuisine_make li {
    display: table;
    padding: 16px 0;
    border-bottom: 1px solid #9e9595;
  }

  .num {
    display: inline-block;  /* インラインブロック要素へ変更 */
    font-size: 1.714em;
    width: 40px;
    margin-top: -5px;
    padding-right: 10px;
  }

  .text {
    display: table-cell;
    vertical-align: top;
    width: 100%;
  }

/*レシピ提供*/
  .offer {
    margin: 16px 0 0 0;
    text-align: right;
  }

  .offer p {
    margin: 4px 0 0 0;
    font-size: 80%;
  }
}
</style>