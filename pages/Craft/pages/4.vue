<template>

  <div>
    <TheHeader />

    <main>
      <h1>「県指定伝統工芸品」</h1>
      <h2 class = craft_headline>加世田鎌・加世田包丁</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Kaseda.jpg" alt="加世田鎌・加世田包丁">
        </div>
        
        <div class = explanation>
          <p>
            槌の打ち跡が生々しく、荒々しい鋼の黒光りを持つ加世田の刃物。<br>
            加世田包丁は日本刀と似た手法でつくられており、加世田鎌も両刃の丈夫さに刀鍛冶の技術がいかされている。
          </p>
        </div>
        <div class="link-space">
          <a class ="link" href="http://localhost:3000/Craft/pages/Kaseda">基本情報はこちら</a>
        </div>
      </div>

      <h2 class = craft_headline>甲冑</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/Kattyu.jpeg" alt="甲冑">        
          <div class="teikyou">
            <p>
              写真協力<br>
              公益社団法人 鹿児島県観光連盟
            </p>
          </div>
        </div>

        <div class = explanation>
          <p>
            昔ながらの製法を守りながら、映画・テレビなどの時代劇に使用される鎧やかぶとの<br>
            全国シェア９割以上の生産を誇り、全国各地のお祭りの武者行列などでも使用されている。
          </p>
        </div>
        <div class="link-space">
          <a class ="link" href="http://localhost:3000/Craft/pages/Armor">基本情報はこちら</a>
        </div>
      </div>        

      <h2 class = craft_headline>竹製品</h2>
      <div class="craft">
        <div class = craft_img>
          <img src="~/assets/img/bambooproducts.jpg" alt="竹製品">
        </div>

        <div class = explanation>
          <p>
            鹿児島は竹林面積日本一の「竹」のふるさと。<br>
            古くから竹を使って様々な生活道具が作られており、庶民生活には欠かせないもの。
          </p>
        </div>
        <div class="link-space">
          <a class ="link" href="http://localhost:3000/Craft/pages/BambooProducts">基本情報はこちら</a>
        </div>
      </div>
      
      <ul class="Pagination">
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1">
          <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
          </svg>
          </a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
        </li>
        
        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/4"><span>4</span></a>
        </li>

        <li class="Pagination-Item">
          <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13 5l7 7-7 7M5 5l7 7-7 7" />
            </svg>
          </a>
        </li>
      </ul>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
main {margin: 0 auto;}  /* 全余白の指定 */

h1 {font-family: 'New Tegomin', serif;} /* フォントの変更 */

h2.craft_headline {
  margin: 0px;                       /* 全余白の指定 */
  padding: 8px 0px;                  /* 全余白の指定 */
  border-top: 2px solid #d5d4c3;   /* 上線 */
}

/* 提供 */
.teikyou {font-weight: bold;} /* 文字の太さ */

.teikyou p {
  margin: 0px;        /* 全余白の指定 */
  font-size: 13px;    /* 文字の大きさ */
}

.explanation p {
  margin: 0px;          /* 全余白の指定 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

.link-space a {
  margin: 0;            /* 全余白の指定 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

.link {
  color: blue;          /* 文字の色 */
  text-decoration: none;  /* 下線の削除 */
}

/* ページネーション */
.Pagination {
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
}

.Pagination-Item-Link {
  width: 45px;
  height: 45px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  flex-wrap: wrap;
  overflow: hidden;
  background: #fff;
  border: solid 2px #111;
  font-size: 14px;
  color: #111;
  font-weight: bold;
  transition: all 0.15s linear;
}

.Pagination-Item-Link-Icon {width: 20px;}

.Pagination-Item-Link.isActive {
  background: #111;
  color: #fff;
  pointer-events: none;
}

.Pagination-Item-Link:not(.isActive):hover {
  background: #111;
  color: #fff;
}

.Pagination > * + * {margin-left: 8px;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  br {display: none;}

  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  .craft {text-align: center;}

  h2.craft_headline {text-align: center;}

  .link-space {margin: 8px 0;}

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px;
  }
  
/* 世界遺産画像 */
  .craft_img img{
    width: 8cm;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}

  h1 {margin-bottom: 0;}
  
/* 世界遺産一覧説明 */
  .craft {
    display: flex;
    margin-bottom: 16px;
  }
  
  .explanation {
    margin: auto;
    width: 40em;
  }

  .link-space {align-self: end;}

  a:hover.link {color: rgb(71, 1, 92);}

/* 世界遺産画像 */
  .craft_img img{
    width: 6cm;
    height: auto;
  }
}
</style>