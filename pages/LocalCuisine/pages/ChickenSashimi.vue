<template>

  <div>
    <TheHeader />

    <main>
      <h1>鳥刺し</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
          <img src="~/assets/img/Torisashi02.jpeg" alt="鳥刺し">
        </div>
          
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>鹿児島県全域</dd>
          </dl>
          
          <dl>
            <dt>食材</dt>
            <dd>鶏肉</dd>
          </dl>
          
          <dl>
            <dt>歴史</dt>
            <dd>鹿児島県では、江戸時代から薩摩武士たちが士風高揚のため、盛んに闘鶏をおこなっており、その際に負けた鶏をその場でしめて食べる習慣があった。闘鶏が禁止された後も、各家庭で鶏が飼われ、来客がある時や祝いの席のために鶏をしめて調理し食べていたという。このように鹿児島県においては、古くから鶏肉を使った料理が身近でにあったことから、鶏肉を刺身で食べる「鶏刺し」が根づいたと考えられてる。</dd>
          </dl>

        </div>
      </div>

      <div class = "recipe">
        <h3>材料</h3>
        <ul class = "localcuisine_memu">

          <li>
            <ul class = "list">
              <li>鶏刺し用鶏肉（もも・ささみ・むね肉）</li>
              <li class="quantity">150g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>玉ねぎ</li>
              <li class="quantity">30g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>ねぎ</li>
              <li class="quantity">5g</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>しょうが</li>
              <li class="quantity">お好みで</li>
            </ul>
          </li>

          <li>
            <ul class = "list">
              <li>にんにく</li>
              <li class="quantity">お好みで</li>
            </ul>
          </li>

          <li>
            <ul class = "list_last">
              <li>青じそ</li>
              <li class="quantity">お好みで</li>
            </ul>
          </li>

        </ul>

        <h3>作り方</h3>

        <ul class = "localcuisine_make">
          
          <li>
            <div class = "num">1</div>
            <div class = "text">
              鶏刺し用の新鮮な鶏肉を用意する。
            </div>
          </li>

          <li>
            <div class = "num">2</div>
            <div class = "text">
              バーナーなどで皮目をあぶり、表面の色が変わったら火を止める。（中は生のまま）
            </div>
          </li>

          <li>
            <div class = "num">3</div>
            <div class = "text">
                3mm幅に皮目から切る。肉の繊維の方向を見て繊維を断ち切るようにくらいの刺身に切る。
            </div>
          </li>

          <li>
            <div class = "num">4</div>
            <div class = "text">
              青じそを敷き部位ごとに盛り付け玉ねぎはスライス、ネギは小口切り。しょうがニンニクはすりおろして一緒に盛り付け、好みで醤油やポン酢で味わう。
            </div>
          </li>

        </ul>

        <div class = "offer">
          <p>レシピ提供元名 : 株式会社Table of Smile</p>
          <p>※レシピは地域・家庭によって違いがあります。</p>
        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
.quantity {list-style-type: none;}

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
    width: 20cm;
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