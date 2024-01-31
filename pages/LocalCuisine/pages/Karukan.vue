<template>

  <div>
    <TheHeader />

    <main>
      <h1>かるかん</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Karukan.jpg" alt="かるかん">
          <div class="teikyou">
            <p>画像提供元：鹿児島県</p>
          </div>
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島全域</dd>
          </dl>

          <dl>
            <dt>食材</dt>
            <dd>かるかん粉、大和芋、あん</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>
              諸説あるが、薩摩藩の第11代藩主であった島津斉彬が、
              保存食の研究のために江戸から招聘した明石出身の菓子職人・八島六兵衛によって考案されたという説が有力とされている。
            </dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料（10個分）</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>かるかん粉</li>
              <li class="quantity">125g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>大和芋</li>
              <li class="quantity">100g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>砂糖</li>
              <li class="quantity">150g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>水</li>
              <li class="quantity">75cc</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>あん</li>
              <li class="quantity">110g</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              あんは10等分し、丸め、中心部を少しへこませたかたちにしておく。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              大和芋をすりおろし、水を少しづつ加え混ぜる。
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
              【2】に砂糖、かるかん粉を加え混ぜ合わせる。
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              かるかん型に【3】を10等分し、あんを中心部におき、楊枝であんの上に生地をかぶせるようにする。
            </div>
          </li>

          <li>
            <div class = "num">5</div>
            <div class = "text">
              蒸気の上がった蒸し器に4を入れ、強火のままで25分蒸し、型から外す。
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