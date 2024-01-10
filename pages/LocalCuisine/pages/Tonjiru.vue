<template>

  <div>
    <TheHeader />

    <main>
      <h1>豚汁</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Tonjiru02.jpg" alt="豚汁">
          <div class="teikyou">
            <p><b>写真協力：公益社団法人 鹿児島県観光連盟</b></p>
          </div>
        </div>
          
        <div class = localcuisine_note>
          
          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>豚肉、大根、人参、里芋、こんにゃく、厚揚げ、味噌</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              諸説あり定かではないが薩摩汁の豚を使うものが独立した説がある。
              日本全国で獣肉食が広まったのは明治時代以降であるが、琉球と薩摩地方だけは例外的に豚を含めた獣肉食の習慣があり、
              地方料理に肉入りの味噌汁があった。
            </dd>
          </dl>
        </div>
      </div>

      <div class = "recipe">
        <h3>材料</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>豚肉薄切り</li>
              <li class="quantity">80g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>大根</li>
              <li class="quantity">100g</li>
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
              <li>里芋</li>
              <li class="quantity">100g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>こんにゃく</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>油揚げ</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【薬味】小ねぎ、しょうが</li>
              <li class="quantity">適量</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】いりこ</li>
              <li class="quantity">20g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】水</li>
              <li class="quantity">3カップ</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【汁】麦味噌</li>
              <li class="quantity">50g</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>油</li>
              <li class="quantity">適宜</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              水にいりこを入れ、30分したら火にかけ、沸騰後3分でいりこを取り出す（いりこ出汁）。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              材料は食べやすい大きさに切り、鍋に油をひき、豚肉を炒め、その後小ねぎ・しょうが以外の食材も加え、
              全体に油が回ったら、1のいりこ出汁を加え、アクを取りながら煮る。柔らかくなったら麦味噌を溶かし入れる。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              器に盛り、小口ぎりの小ねぎと千切りのしょうがをのせる。
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
main {margin: 0 auto;}

.quantity {list-style-type: none;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  h1 {text-align: center;}

/*郷土料理説明*/
  .localcuisine {padding-bottom: 24px;}

  .localcuisine h1 {margin: 1.6px auto;}

  .localcuisine_img {text-align: center;}

  .localcuisine_img img {
    height: 8cm;
    width: auto;
  }

/* 写真提供 */
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

/*レシピ提供*/
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

  .localcuisine h1 {margin: 1.6px auto;}

  .localcuisine_img img {height: 8cm;}

/* 写真提供 */
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

/*レシピ提供*/
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