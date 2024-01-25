<template>

  <div>
    <TheHeader />

    <main>
      <h1>甲冑</h1>
      <div class="Craft">         

        <div class = Craft_img>
          <img src="~/assets/img/Kattyu.jpeg" alt="甲冑">
        </div>
        
        <div class = Craft_note>
          <dl>
            <dt>読み</dt>
            <dd>かっちゅう</dd>
          </dl>
          
          <dl>
            <dt>工芸品の分類</dt>
            <dd>その他</dd>
          </dl>

          <dl>
            <dt>主な製品</dt>
            <dd>甲冑、兜</dd>
          </dl>

          <dl>
            <dt>主要製造地域</dt>
            <dd>薩摩川内市</dd>
          </dl>

          <dl>
            <dt>指定年月日</dt>
            <dd>平成9年（1997年）3月24日</dd>
          </dl>

          <dl>
            <dt>詳しくは</dt>
            <dd><a href="http://yoroi.co.jp/" target="_blank">甲冑工房 丸武</a></dd>
          </dl>

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

.Craft_note dd a {
  text-decoration: none;
  color: blue;
}

/* マウスオーバー */
.Craft_note dd a:hover {color: rgb(71, 1, 92);}
  
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}  /* 要素の外側上余白 */

  h1 {text-align: center;} /* 左右の中央揃え */
  
  .Craft {padding-bottom: 16px;}

  .Craft_img {text-align: center;}

  .Craft_img img {width: 345px;}

  .Craft_note {margin-top: 16px;}

  .Craft_note h2 {margin: 8px auto;}

  .Craft_note dl {
    display: table;
    width: 100%;                  /* 横幅 */
    font-size: 16px;              /* 文字の大きさ */
    margin: 3px 0;                /* 要素の外側余白 */
    overflow: hidden;             /* 要素からはみ出た部分を非表示 */
    display: flex;                /* 親要素に対して子要素を横並びにする */
    align-items: center;          /* 上下の中央揃え */
    background-color: #e0e2e2;  /* 背景 */
  }

  .Craft_note dt {
    vertical-align: middle; 
    flex-shrink: 0;         /* 縮小値 */
    text-align: center;     /* 左右の中央揃え */
    width: 24%;             /* 横幅 */
  }

  .Craft_note dd {
    margin: 0;                /* 要素の外側余白 */
    padding: 2%;              /* 要素の内側余白 */
    font-size: 16px;          /* 文字の大きさ */
    display: flex;            /* 親要素に対して子要素を横並びにする */
    background-color: #fff; /* 背景 */
    padding-left: 1%;         /* 要素の内側左余白 */
    flex-grow: 1;             /* 余白の追加 */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .Craft {
    display: flex;        /* 親要素に対して子要素を横並びにする */
    padding-bottom: 24px; /* 要素の内側下余白 */
  }

  .Craft_img {margin: auto;}  /* 要素の外側余白 */

  .Craft_img img {width: 450px;}  /* 横幅 */

  .Craft_note {
    margin: auto;       /* 要素の外側余白 */
    padding-left: 16px; /* 要素の内側左余白 */
  }

  .Craft_note h2 {margin: 8px auto;}  /* 要素の外側余白 */

  .Craft_note dl {
    font-size: 18px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .Craft_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 20%;
  }

  .Craft_note dd {
    width: 14cm;
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>
