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
main {margin: 0 auto;}

.quantity {list-style-type: none;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  h1 {text-align: center;}

/*郷土料理説明*/
  .localcuisine {padding-bottom: 24px;}

  .localcuisine h1 {margin: 1.6px auto;}

/* 画像 */
  .localcuisine_img {text-align: center;}

  .localcuisine_img img {height: 7cm;}

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
  main {max-width: 1024px;}

/*郷土料理説明*/
  .localcuisine {
    display: flex;
    padding-bottom: 24px;
  }

  .localcuisine h1 {
    margin: 1.6px auto;
  }

/* 画像 */
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