<template>

  <div>
    <TheHeader />

    <main>
      <h1>両棒餅（じゃんぼ餅）</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Janbomoti-min.jpg" alt="両棒餅">
          <div class="teikyou">
            <p>出典：農林水産省「うちの郷土料理」</p>
          </div>
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島市</dd>
          </dl>

          <dl>
            <dt>材料</dt>
            <dd>もち米粉、つきたての餅</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              南北朝時代、後醍醐天皇の子である懐良親王が、鹿児島市の谷山城に滞在していた際、
              谷山城主の谷山隆信が親王を慰めようと、餅をつくってそこへ2本の串をさし、味噌と黒砂糖を煮つめたものをかけて出したところ、
              料理の名を聞かれ、とっさに「両棒（じゃんぼ）」といったのがはじまりだという逸話がある。
            </dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料（12本分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>もち米粉</li>
              <li class="quantity">130g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>水</li>
              <li class="quantity">110cc～120cc</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>竹串</li>
              <li class="quantity">24本</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【醤油ダレ】 淡口醤油</li>
              <li class="quantity">大さじ1</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【醤油ダレ】 砂糖</li>
              <li class="quantity">大さじ5</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【醤油ダレ】 本みりん</li>
              <li class="quantity">大さじ1</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>【醤油ダレ】 片栗粉</li>
              <li class="quantity">大さじ1</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>【醤油ダレ】 水</li>
              <li class="quantity">50cc</li>
            </ul>
          </li>
          
        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              もち米粉に水を加え耳たぶくらいのかたさにこねあげ、直径3cmほどの平たい円形にし、沸騰した湯でゆで、浮いてきたら水にとって冷まし、水気を切る。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              醤油ダレは、片栗粉をあらかじめ水で溶いておき、他の材料と共に火にかけとろみをつける。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              【1】を素焼きにし、1個につき2本の串を刺し2のタレを付けて皿に盛る。
            </div>
          </li>
          
        </ul>
        
        <div class = "offer">
          <p>レシピ提供元名 : NPO法人 霧島食育研究会</p>
          <p>※レシピは地域・家庭によって違いがあります。</p>
        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}
main {margin: 0 auto;}

h1 {
  margin: 0;
  padding: 8px 0;
  font-family: 'New Tegomin', serif;
}

.quantity {list-style-type: none;}

/* 提供文字 */
.teikyou {font-weight: bold;}
.teikyou p {margin: 0;}

/*郷土料理説明*/
.localcuisine {padding-bottom: 24px;}

.localcuisine_note dl {
  margin: 3px 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  background-color: #e0e2e2;
}

.localcuisine_note dt {
  flex-shrink: 0;
  text-align: center;
}

.localcuisine_note dd {
  margin: 0;
  display: flex;
  background-color: #fff;
  padding-left: 1%;
  flex-grow: 1;
}

.recipe {
  padding: 24px;
  margin-bottom: 24px;
  background: #d2e7f3;
}

.recipe h3 {
  margin: 0;
  padding: 0;
  border-bottom: 1px solid #1b1b1b;
}

.list {
  display: flex;
  justify-content: space-between;
  padding: 8px 0 6px;
  border-bottom: 1px solid #9e9595;
}

.list_last {
  display: flex;
  justify-content: space-between;
  padding: 8px 0 64px;
}

/*作り方*/
.localcuisine_make {
  margin: 0;
  padding: 0;
  font-size: 1em;
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
  margin: 16px 0 0 0;
  text-align: right;
}

.offer p {
  margin: 4px 0 0 0;
  font-size: 80%;
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}
  h1 {text-align: center;}

/* 画像 */
  .localcuisine_img {text-align: center;}

  .localcuisine_img img {
    width: 400px;
    height: auto;
  }

/* 提供文字 */
  .teikyou p {margin: 8px 0;} /* 要素の外側余白 */

/*材料*/
  .localcuisine_note {margin-top: 16px;}
  .localcuisine_note dl {font-size: 16px;}
  .localcuisine_note dt {width: 30%;}
  .localcuisine_note dd {width: 12cm;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}

/*郷土料理説明*/
  .localcuisine {display: flex;}

/* 画像 */
  .localcuisine_img img {
    width: 400px;
    height: auto;
  }

/*材料*/
  .localcuisine_note {
    margin: auto;
    margin-left: 16px;
  }

  .localcuisine_note dl {font-size: 18px;}
  .localcuisine_note dt {width: 25%;}
  .localcuisine_note dd {width: 16cm;}
}
</style>