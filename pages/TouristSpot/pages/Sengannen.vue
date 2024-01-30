<template>

  <div>
    <TheHeader />

    <main>
      <h1>仙厳園</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/Senganen.jpg" alt="仙厳園">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>9:00～17:00
                <br>
                ※年中無休
                <br>
                ※3月第1日曜日は鹿児島マラソンのため休園
            </dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>庭園+尚古集成館+御殿:高校生以上1,500円、小中学生750円
                <br>
                庭園+尚古集成館:高校生以上1,000円、小中学生500円
            </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市吉野町9700-1</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【バス】各種バス「仙巌園前」バス停下車すぐ
                <br>
                【車】九州自動車道「姶良（あいら）」ICより約40分
            </dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://www.senganen.jp/" target="_blank">仙厳園 公式ホームページ</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000332.html" class = "btn" target="_blank">名勝 仙厳園 周辺のホテル・旅館</a>

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

.TouristSpot_note dl {
  margin: 3px 0;                /* 要素の外側余白 */
  overflow: hidden;             /* 要素からはみ出た部分を非表示 */
  display: flex;                /* 親要素に対して子要素を横並びにする */
  align-items: center;          /* 中央揃え */
  background-color: #e0e2e2;  /* 背景 */
}

.TouristSpot_note dt {
  flex-shrink: 0;         /* 縮小値 */
  text-align: center;     /* 中央揃え */
}

.TouristSpot_note dd {
  margin: 0;                 /* 要素の外側余白 */
  display: flex;             /* 親要素に対して子要素を横並び */
  background-color: #fff;  /* 背景 */
  padding-left: 1%;          /* 要素の内側左余白 */
  flex-grow: 1;              /* 余白の追加 */
}

/* ボタン */
a.btn {
  display: block;                /* ブロック要素へ変更 */
  text-align: center;            /* 左右の中央揃え */
  text-decoration: none;         /* 下線削除 */
  width: 320px;                  /* 横幅 */
  margin: 24px auto;             /* 高さ */
  padding: 1rem 4rem;            /* 要素の内側余白 */
  font-weight: bold;             /* 文字の太さ */
  border: 2px solid #27acd9;   /* 枠線 */
  background: #27acd9;         /* 背景 */
  color: #fff;                 /* 文字の色 */
  border-radius: 100vh;          /* 角を丸める */
  transition: 0.5s;              /* アニメーションが完了するまでの時間 */
}

/* マウスオーバー */
a.btn:hover {
  color: #27acd9;   /* 文字の色 */
  background: #fff; /* 背景 */
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}  /* 要素の外側上余白 */

  h1 {text-align: center;} /* 中央揃え */

  .TouristSpot_img {text-align: center;}  /* 中央揃え */

  .TouristSpot_img img {width: 400px;}  /* 横幅 */

  .TouristSpot_note {margin-top: 16px;} /* 要素の外側上余白 */

  .TouristSpot_note h2 {margin: 8px auto;}  /* 要素の外側余白 */

  .TouristSpot_note dl {font-size: 15px;} /* 文字の大きさ */

  .TouristSpot_note dt {width: 20%;}  /* 横幅 */

  .TouristSpot_note dd {
    padding: 2%;      /* 要素の内側余白 */
    font-size: 16px;  /* 文字の大きさ */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .TouristSpot {
    display: flex;            /* 親要素に対して子要素を横並びにする */
    padding-bottom: 24px;     /* 要素の内側下余白 */
  }

  .TouristSpot_img img {height: 345px;}  /* 高さ */

  .TouristSpot_note {
    margin: auto;       /* 要素の外側余白 */
    padding-left: 16px; /* 要素の内側左余白 */
  }

  .TouristSpot_note h2 {margin: 8px auto;}    /* 要素の外側余白 */

  .TouristSpot_note dl {font-size: 18px;}     /* 文字の大きさ */

  .TouristSpot_note dt {width: 20%;}  /* 横幅 */

  .TouristSpot_note dd {width: 14cm;} /* 横幅 */
}
</style>