<template>

   <div>
    <TheHeader />

    <main>
      <h1>川辺仏壇</h1>
      <div class="Craft">
          
        <div class = Craft_img>
          <img src="~/assets/img/kawabebutudan.jpg" alt="川辺仏壇">
        </div>

        <div class = Craft_note>

          <dl>
            <dt>読み</dt>
            <dd>かわなべぶつだん</dd>
          </dl>
          
          <dl>
            <dt>工芸品の分類</dt>
            <dd>仏壇・仏具</dd>
          </dl>

          <dl>
            <dt>主な製品</dt>
            <dd>金仏壇</dd>
          </dl>

          <dl>
            <dt>主要製造地域</dt>
            <dd>南九州市</dd>
          </dl>

          <dl>
            <dt>指定年月日</dt>
            <dd>昭和50年（1975年）5月10日</dd>
          </dl>

          <dl>
            <dt>詳しくは</dt>
            <dd><a href="https://www.kawanabe-butudan.or.jp/" target="_blank">鹿児島県川辺仏壇協同組合</a></dd>
          </dl>

        </div>
      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
  .Craft_note dd a {
    text-decoration: none;
    color: blue;
  }

  .Craft_note dd a:hover {color: rgb(71, 1, 92);}
  
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {margin: 0 auto;}

  h1 {
    margin: 16px 0;
    text-align: center;
  }
  
  .Craft {padding-bottom: 16px;}

  .Craft h1 {margin: 1.6px auto;}

  .Craft_img {text-align: center;}

  .Craft_img img {width: 72%;}

  .Craft_img p {margin: 0;}

  .Craft_note {margin-top: 16px;}

  .Craft_note h2 {margin: 8px auto;}

  .Craft_note dl {
    display: table;
    width: 100%;
    font-size: 16px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .Craft_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 24%;
  }

  .Craft_note dd {
    margin: 0px;
    padding: 2%;
    font-size: 16px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }
  
  .Craft {
    display: flex;
    padding-bottom: 24px;
  }

  .Craft h1 {margin: 1.6px auto;}

  .Craft_img {margin: auto;}

  .Craft_img img {height: 8cm;}

  .Craft_img p {margin: 0;}

  .Craft_note {
    margin: auto;
    padding-left: 16px;
  }

  .Craft_note h2 {margin: 8px auto;}

  .Craft_note dl {
    font-size: 18px;
    margin: 3px 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    background-color: #e0e2e2;
  }

  .Craft_note dt {
    vertical-align: middle;
    flex-shrink: 0;
    text-align: center;
    width: 20%;
  }

  .Craft_note dd {
    width: 14cm;
    margin: 0px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>
