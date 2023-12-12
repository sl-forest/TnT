<template>

  <div>
    <TheHeader />

    <main>
      <h1>がね</h1>
        <div class="localcuisine">
          <div class = localcuisine_img>
            <img src="~/assets/img/Gane.jpg" alt="がね">
          </div>
          
          <div class = localcuisine_note>

            <dl>
              <dt>伝承地域</dt>
              <dd>鹿児島県全域</dd>
            </dl>

            <dl>
              <dt>食材</dt>
              <dd>さつまいも、人参、ニラ、小麦粉</dd>
            </dl>

            <dl>
              <dt>歴史</dt>
              <dd>
                「がね」は、さつまいもや野菜を太めの千切りにし、衣をつけて揚げる料理。その見た目が“かに（鹿児島弁でがねという）”に似ていることからこの名がついた。
                砂糖を多く入れ甘めな味付けが特徴で地域により具材や衣の材料は違う。
              </dd>
            </dl>
              
          </div>
        </div>

        <div class = "recipe">
          <h3>材料（8～10個分）</h3>
          <ul class = "localcuisine_memu">

            <li>
              <ul class = "list">
                <li>さつまいも</li>
                <li class="quantity">200g</li>
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
                <li>ニラ</li>
                <li class="quantity">30g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】小麦粉</li>
                <li class="quantity">100g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】もち米粉</li>
                <li class="quantity">50g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】砂糖</li>
                <li class="quantity">40g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】卵</li>
                <li class="quantity">1個</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】淡口醤油</li>
                <li class="quantity">大さじ1.5</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】塩</li>
                <li class="quantity">ふたつまみ</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>【衣】水</li>
                <li class="quantity">80cc</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>油</li>
                <li class="quantity">適量</li>
              </ul>
            </li>

          </ul>

          <h3>作り方</h3>

          <ul class = "localcuisine_make">
            
            <li>
              <div class = "num">1</div>
              <div class = "text">
                さつまいもは薄く皮を剥き（ところどころ皮を残す）、5mm角×7～8cmの細切りにする。
                ボウルに水を張り、さつまいもが完全に浸るようにさらしてざるに開ける。
                人参は薄く皮を剥き、さつまいもより短めの2～3cmに切る。ニラは7～8cmの長さに切る。
              </div>
            </li>

            <li>
              <div class = "num">2</div>
              <div class = "text">
                ボウルに1と水以外の材料を加えながら衣が具にまとわりつく感じになるまで混ぜる。
              </div>
            </li>

            <li>
              <div class = "num">3</div>
              <div class = "text">
                鍋に油を3cm以上の深さになるように入れて、170度になるように熱する。（臭みが取れる）
              </div>
            </li>

            <li>
              <div class = "num">4</div>
              <div class = "text">
                木杓子で具をすくい、横長にカニの姿のようにかたちをととのえる。
                菜箸で向こう側に押すように鍋に落とし、2、3分でひっくり返し、さつまいもの甘い匂いがしてきて全体がきつね色になったら揚げ上がり。
                バットにキッチンペーパーを敷き、立てて並べると油の切れが良い。
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
.quantity {
  list-style-type: none;
}
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {
    margin: 0 auto;
  }

  h1 {
    text-align: center;
  }

/*郷土料理説明*/
  .localcuisine {
    padding-bottom: 24px;
  }

  .localcuisine h1 {
    margin: 1.6px auto;
  }

  .localcuisine_img {
    text-align: center;
  }

  .localcuisine_img img {
    height: 8cm;
    width: auto;
  }

/*材料*/
  .localcuisine_note {
    margin-top: 16px;
  }

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

  .localcuisine_note dd a {
    text-decoration: none;
    color: blue;
  }

  .localcuisine_note > dd {
    border: 1px solid #ddd;
    border-top: none;
  }

  .localcuisine_note > dt,
  .localcuisine_note > dd {
    text-align: center;
  }

  .localcuisine_note > dd > ul {
    text-align: left;
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

  .localcuisine h1 {
    margin: 1.6px auto;
  }

  .localcuisine_img img {
    height: 8cm;
  }

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
    margin: 0px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }

  .localcuisine_note dd a {
    text-decoration: none;
    color: blue;
  }

  .localcuisine_note dd a:hover {
    color: rgb(71, 1, 92);
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