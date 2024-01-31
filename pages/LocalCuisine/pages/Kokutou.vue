<template>

  <div>
    <TheHeader />
    <main>
      <h1>黒糖</h1>
      <div class="localcuisine">
        <div class = localcuisine_img>
            <img src="~/assets/img/Kokutou.jpg" alt="黒糖">
        </div>
        
        <div class = localcuisine_note>

          <dl>
            <dt>伝承地域</dt>
            <dd>奄美地域</dd>
          </dl>

          <dl>
            <dt>材料</dt>
            <dd>さとうきび</dd>
          </dl>

          <dl>
            <dt>歴史</dt>
            <dd>元禄時代（１６８８年）、日本に黒糖（黒砂糖）は伝わった。江戸時代より沖縄、奄美大島、種子島などで生産されており、沖縄で黒糖（黒砂糖）は“ヌチグスイ（命薬）”と呼ばれ薬として飲まれていたこともある。</dd>
          </dl>

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

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}
  h1 {text-align: center;}

/* 画像 */
  .localcuisine_img {text-align: center;}
  .localcuisine_img img {width: 400px;}

/* 提供文字 */
  .teikyou p {margin: 8px 0;}

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
  .localcuisine_img img {width: 400px;}

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