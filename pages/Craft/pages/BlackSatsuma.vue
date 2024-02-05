<template>

   <div>
    <TheHeader />

    <main>
      <h1>黒薩摩</h1>
      <div class="Craft">
            
        <div class = Craft_img>
          <img src="~/assets/img/KuroSatsuma-min.jpg" alt="黒薩摩">
        </div>

        <div class = Craft_note>

          <dl>
            <dt>読み</dt>
            <dd>くろさつま</dd>
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
            <dt>詳しくは</dt>
            <dd><a href="https://artsandculture.google.com/story/SgUB0NWQJzwfLg?hl=ja" target="_blank">Google Arts&culture</a></dd>
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

.Craft_note dl {
  margin: 3px 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  background-color: #e0e2e2;
}

.Craft_note dt {
  flex-shrink: 0;
  text-align: center;
}

.Craft_note dd {
  margin: 0;
  display: flex;
  background-color: #fff;
  padding-left: 1%;
  flex-grow: 1;
}

.Craft_note dd a {
  text-decoration: none;
  color: blue;
}

/* マウスオーバー */
.Craft_note dd a:hover {color: rgb(71, 1, 92);}
  
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}
  h1 {text-align: center;}
  .Craft {padding-bottom: 16px;}
  .Craft_img {text-align: center;}

  .Craft_img img {
    width: 345px;
    height: auto;
  }

  .Craft_img p {margin: 0;}
  .Craft_note {margin-top: 16px;}
  .Craft_note h2 {margin: 8px auto;}
  .Craft_note dl {font-size: 16px;}
  .Craft_note dt {width: 24%;}

  .Craft_note dd {
    padding: 2%;
    font-size: 16px;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}

  .Craft {
    display: flex;
    padding-bottom: 24px;
  }

  .Craft_img {margin: auto;}

  .Craft_img img {
    width: 400px;
    height: auto;
  }

  .Craft_note {
    margin: auto;
    padding-left: 16px;
  }

  .Craft_note h2 {margin: 8px auto;}
  .Craft_note dl {font-size: 18px;}
  .Craft_note dt {width: 20%;}
  .Craft_note dd {width: 14cm;}
}
</style>

