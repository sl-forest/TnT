<template>

  <div>
    <TheHeader />

    <main>
      <h1>種子島宇宙センター</h1>
      <div class="TouristSpot">

        <div class = TouristSpot_img>
          <img src="~/assets/img/SpaceCenter.jpg" alt="種子島宇宙センター">
        </div>
        
        <div class = TouristSpot_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>9:30～16:30</dd>
          </dl>

          <dl>
            <dt>定休日</dt>
            <dd>月曜（祝日の場合は翌日、8月は第1月曜日及び第5月曜日のみ休館）、年末年始
                <br>
                ※その他、ロケットの打ち上げによる休館や臨時休館あり
            </dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>無料</dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県熊毛郡南種子町大字茎永字麻津</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【車】種子島空港からタクシー約50分</dd>
          </dl>

          <dl>
            <dt>詳しく</dt>
            <dd><a href="https://fanfun.jaxa.jp/visit/tanegashima/index.html" target="_blank">種子島宇宙センター 施設見学（JAXA公式ページ）</a></dd>
          </dl>
          <a href = "https://travel.rakuten.co.jp/yado/spot/kagoshima/S46000121.html" class = "btn" target="_blank">種子島宇宙センター 周辺のホテル・旅館</a>

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

.TouristSpot_note dd a {
  text-decoration: none;  /* 下線削除 */
  color: blue;          /* 文字の色 */
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

  h1 {text-align: center;} /* 左右の中央揃え */

  .TouristSpot_img {text-align: center;}

  .TouristSpot_img img {height: 8cm;}

  .TouristSpot_note {margin-top: 16px;}

  .TouristSpot_note h2 {margin: 8px auto;}

  .TouristSpot_note dl {
    display: table;
    width: 100%;
    font-size: 15px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .TouristSpot_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 20%;
  }

  .TouristSpot_note dd {
    margin: 0;
    padding: 2%;
    font-size: 15px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .TouristSpot {
    display: flex;            /* 親要素に対して子要素を横並びにする */
    justify-content: center;  /* 横並び要素の左右中央揃え */
    padding-bottom: 24px;     /* 要素の内側下余白 */
  }
  
  .TouristSpot_img img {height: 10cm;}

  .TouristSpot_note {
    margin: auto;
    padding-left: 16px;
  }

  .TouristSpot_note h2 {margin: 8px auto;}

  .TouristSpot_note dl {
    font-size: 18px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .TouristSpot_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 20%;
  }

  .TouristSpot_note dd {
    width: 14cm;
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }

  .TouristSpot_note dd a:hover {color: rgb(71, 1, 92);}
}
</style>