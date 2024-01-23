<template>

   <div>
    <TheHeader />

    <main>
      <h1>薩摩焼</h1>
      <div class="Craft">
            
        <div class = Craft_img>
          <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
        </div>

        <div class = Craft_note>

          <dl>
            <dt>読み</dt>
            <dd>さつまやき</dd>
          </dl>
          
          <dl>
            <dt>工芸品の分類</dt>
            <dd>陶磁器</dd>
          </dl>

          <dl>
            <dt>主な製品</dt>
            <dd>食器、茶器、花器、酒器、装飾品</dd>
          </dl>

          <dl>
            <dt>主要製造地域</dt>
            <dd>鹿児島市、指宿市、日置市</dd>
          </dl>

          <dl>
            <dt>系統</dt>
            <dd>
                ・苗代川なおしろがわ系
                <br>
                ・竪野たての系
                <br>
                ・龍門司りゅうもんじ系
                <br>
                ・西餅田にしもちだ系
                <br>
                ・平佐ひらさ系
            </dd>
          </dl>

          <dl>
            <dt>指定年月日</dt>
            <dd>平成14年（2002年）1月30日</dd>
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
body {margin: 0;}       /* 要素の外側余白 */

main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;            /* 要素の外側余白 */
  padding: 8px 0;       /* 要素の内側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

.Craft_note dd a {
  text-decoration: none;
  color: blue;
}

/* マウスオーバー */
.Craft_note dd a:hover {color: rgb(71, 1, 92);}
  
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}    /* 要素の外側上余白 */

  h1 {text-align: center;}   /* 左右の中央揃え */
  
  .Craft {padding-bottom: 16px;}

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
  main {max-width: 1024px;} /* 最大横幅 */

  .Craft {
    display: flex;
    padding-bottom: 24px;
  }

  .Craft_img {margin: auto;}

  .Craft_img img {height: 8cm;}

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
