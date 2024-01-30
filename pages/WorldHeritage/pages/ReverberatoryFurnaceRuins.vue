<template>

  <div>
    <TheHeader />

    <main>
      <h1>旧集成館「反射炉跡」</h1>
      <div class="WorldHeritage">

        <div class = WorldHeritage_img>
          <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
        </div>
      
        <div class = WorldHeritage_note>    
        
          <dl>
            <dt>営業時間</dt>
            <dd>
              8:30～17:30（3/16～10/31）
              <br>
              8:30～17:20（11/1～3/15）
              </dd>
          </dl>

          <dl>
            <dt>休日</dt>
            <dd>年中無休</dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>
              大人:1,000円 
              <br>
              小人:500円（尚古集成館と共通）
              </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市吉野町9700-1</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>
              【車】鹿児島中央駅から20分
              <br>
              【車】鹿児島空港から40分
              <br>
              【バス】鹿児島市周遊バスで仙巌園前（磯庭園前）下車徒歩1分。
            </dd>
          </dl>

          <dl>
          <dt>詳しくは</dt>
          <dd><a href="https://www.senganen.jp/" target="_blank">仙厳園 公式ホームページ</a></dd>
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

.WorldHeritage_note dl {
  margin: 3px 0;                /* 要素の外側余白 */
  overflow: hidden;             /* 要素からはみ出た部分を非表示 */
  display: flex;                /* 親要素に対して子要素を横並びにする */
  align-items: center;          /* 上下の中央揃え */
  background-color: #e0e2e2;  /* 背景 */
}

.WorldHeritage_note dt {
  flex-shrink: 0;         /* 縮小値 */
  text-align: center;     /* 左右の中央揃え */
}

.WorldHeritage_note dd {
  margin: 0;                 /* 要素の外側余白 */
  display: flex;             /* 親要素に対して子要素を横並び */
  background-color: #fff;  /* 背景 */
  padding-left: 1%;          /* 要素の内側左余白 */
  flex-grow: 1;              /* 余白の追加 */
}

.WorldHeritage_note dd a {
  text-decoration: none;  /* 下線削除 */
  color: blue;          /* 文字の色 */
}

/* マウスオーバー */
.WorldHeritage_note dd a:hover {color: rgb(71, 1, 92);} /* 文字の色 */

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}    /* 要素の外側上余白 */

  h1 {
    text-align: center; /* 左右の中央揃え */
    font-size: 30px;    /* 文字の大きさ */
  }
  
  .WorldHeritage {padding-bottom: 16px;}    /* 要素の外側下余白 */

  .WorldHeritage_img {text-align: center;}  /* 中央揃え */

  .WorldHeritage_img img {width: 400px;}  /* 横幅 */

  .WorldHeritage_note {margin-top: 16px;} /* 要素の外側上余白 */

  .WorldHeritage_note h2 {margin: 8px auto;}  /* 要素の外側余白 */

  .WorldHeritage_note dl {font-size: 16px;} /* 文字の大きさ */

  .WorldHeritage_note dt {width: 24%;}  /* 横幅 */

  .WorldHeritage_note dd {
    padding: 2%;      /* 要素の内側余白 */
    font-size: 16px;  /* 文字の大きさ */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .WorldHeritage {
    display: flex;        /* 親要素に対して子要素を横並びにする */
    padding-bottom: 24px; /* 要素の内側下余白 */
  }

  .WorldHeritage_img {margin: auto;}       /* 要素の外側余白 */

  .WorldHeritage_img img {height: 345px;}  /* 高さ */

  .WorldHeritage_note {
    margin: auto;       /* 要素の外側余白 */
    padding-left: 16px; /* 要素の内側左余白 */
  }

  .WorldHeritage_note h2 {margin: 8px auto;}  /* 要素の外側余白 */

  .WorldHeritage_note dl {font-size: 18px;}   /* 文字の大きさ */

  .WorldHeritage_note dt {width: 18%;}  /* 横幅 */

  .WorldHeritage_note dd {width: 13.5cm;} /* 横幅 */
}
</style>