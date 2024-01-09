<template>

  <div>
    <TheHeader />

    <main>
      <h1>油ゾーメン</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Zomen.jpg" alt="油ゾーメン">
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>奄美地域</dd>
          </dl>

          <dl>
            <dt>材料</dt>
            <dd>豚肉、そうめん、ニラ、いりこ、だし汁</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>薩摩藩統治時代に薩摩から持ち込まれ、乾麺で保存がきくことから奄美地域でよく食べられるようになったのではないかという説があるが、定かではない。</dd>
          </dl>
        </div>
      </div>
      
      <div class = "recipe">
        <h3>材料（4人分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>塩豚肉（豚もも肉でも良い）</li>
              <li>120g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>そうめん</li>
              <li>180g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>ニラ</li>
              <li>180g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>いりこ</li>
              <li>12g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>サラダ油</li>
              <li>大さじ2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>だし汁</li>
              <li>2cup</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>醤油</li>
              <li>大さじ1・1/2</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>塩、こしょう</li>
              <li>各少々</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>ごま油</li>
              <li>小さじ2</li>
            </ul>
          </li>

        </ul>
          
        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              ［塩豚肉のつくり方］三枚肉のかたまり（300g）の表面全体に塩をすりこむようにしてまぶす。
              ビニール袋に入れて冷蔵庫で保存する（1週間程度保存できる）。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              豚肉は熱湯で三度塩抜きをする。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              豚肉は細切りにしておく。
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              そうめんは少しかためにゆでて、ざるに上げておく。
            </div>
          </li>

          <li>
            <div class = "num">5</div>
            <div class = "text">
              ニラは2cmの長さに切っておく。
            </div>
          </li>

          <li>
            <div class = "num">6</div>
            <div class = "text">
              中華鍋に油を引き、豚肉を炒める。
            </div>
          </li>

          <li>
            <div class = "num">7</div>
            <div class = "text">
              6にいりことそうめんを入れ、混ぜながら炒める。
            </div>
          </li>

          <li>
            <div class = "num">8</div>
            <div class = "text">
              7にだし汁をまわし入れる。
            </div>
          </li>

          <li>
            <div class = "num">9</div>
            <div class = "text">
              8に醤油を回し入れる。
            </div>
          </li>

          <li>
            <div class = "num">10</div>
            <div class = "text">
              9に塩、こしょうをふり、ニラを入れ混ぜ、最後にごま油を入れる。
            </div>
          </li>
          
        </ul>

        <div class = "offer">
          <p>レシピ提供元名 : 「郷土の味」（鹿児島県食生活改善推進員連絡協議会）</p>
          <p>※レシピは地域・家庭によって違いがあります。</p>
        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
h1 {font-family: 'New Tegomin', serif;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {margin: 0 auto;}

  h1 {text-align: center;}

/*郷土料理説明*/
  .localcuisine {padding-bottom: 24px;}

  .localcuisine h1 {margin: 1.6px auto;}

  .localcuisine_img {text-align: center;}

  .localcuisine_img img {
    height: 8cm;
    width: auto;
  }

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
    margin: 0px;
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
    display: inline-block;
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

/*提供*/
  .offer {
    margin: 16px 0px 0px 0px;
    text-align: right;
  }

  .offer p {
    margin: 4px 0px 0px 0px;
    font-size: 80%;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }

/*郷土料理説明*/
  .localcuisine {
    display: flex;
    padding-bottom: 24px;
  }

  .localcuisine h1 {margin: 1.6px auto;}

  .localcuisine_img img {height: 8cm;}

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
    width: 16cm;
    margin: 0px;
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
    display: inline-block;
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

/*提供*/
  .offer {
    margin: 16px 0px 0px 0px;
    text-align: right;
  }

  .offer p {
    margin: 4px 0px 0px 0px;
    font-size: 80%;
  }
}
</style>