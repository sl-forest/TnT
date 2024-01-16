<template>
  
  <div>
    <TheHeader />

    <main>
      <div class="top_img">
        <img class="item1" src="~/assets/img/Top01.jpg" alt="トップ画像">
        <img class="item1" src="~/assets/img/Top02.jpg" alt="トップ画像">
        <img class="item1" src="~/assets/img/Top03.jpg" alt="トップ画像">
      </div>


      <div class="Kagoshima_about">
          <h1>～鹿児島について～</h1>
          <p>
            多くの観光名所や豊かな自然があり、その土地に根付いた伝統と人の温もり溢れる地方。<br class="pc">
            時代の流れに揉まれ戦乱の歴史をその身に刻みながらも発展してきた鹿児島。<br class="pc">
            そんな魅力溢れる鹿児島を体験してみてください。
          </p>
      </div>

      <div class="headline"><h2>紹介一覧</h2></div>
      <div class = "introduction">
        <figure class="image_area01">
          <a href="http://localhost:3000/Craft/pages/1">
            <img src="~/assets/img/SatumaKiriko.jpg" alt="薩摩切子">
          </a>
        </figure>
        
        <a href="http://localhost:3000/Craft/pages/1" class="text_area">
          <strong>工芸品</strong>
        </a>
        
        <figure class="image_area02">
          <a href="http://localhost:3000/Craft/pages/1">
            <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
          </a>
        </figure>
      </div>

      <div class = "introduction">
        <figure class="image_area03">
          <a href="http://localhost:3000/History/pages/1">
            <img src="~/assets/img/segodon.jpeg" alt="西郷隆盛">
          </a>
        </figure>
        
        <a href="http://localhost:3000/History/pages/1" class="text_area">
          <strong>歴史（偉人）</strong>
        </a>
        
        <figure class="image_area04">
          <a href="http://localhost:3000/History/pages/1">
            <img src="~/assets/img/ookubo.jpg" alt="大久保利通">
          </a>
        </figure>
      </div>
      
      <div class = "introduction">
        <figure class="image_area05">
          <a href="http://localhost:3000/LocalCuisine/pages/1">
            <img src="~/assets/img/Keihan.jpg" alt="鶏飯">
          </a>
        </figure>

        <a href="http://localhost:3000/LocalCuisine/pages/1" class="text_area">
          <strong>郷土料理</strong>
        </a>
        
        <figure class="image_area06">
          <a href="http://localhost:3000/LocalCuisine/pages/1">
            <img src="~/assets/img/Torisashi.jpeg" alt="馬刺し">
          </a>
        </figure>
      </div>

      <div class = "introduction">
        <figure class="image_area07">
          <a href="http://localhost:3000/TouristSpot/pages/1">
            <img src="~/assets/img/Jingu.jpg" alt="霧島神宮">
          </a>
        </figure>
        
        <a href="http://localhost:3000/TouristSpot/pages/1" class="text_area">
          <strong>観光地</strong>
        </a>
        
        <figure class="image_area08">
          <a href="http://localhost:3000/TouristSpot/pages/1">
            <img src="~/assets/img/Senganen.jpg" alt="仙厳園">
          </a>
        </figure>
      </div>

      <div class = "introduction">
        <figure class="image_area09">
          <a href="http://localhost:3000/WorldHeritage/pages/1">
            <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
          </a>
        </figure>
        
        <a href="http://localhost:3000/WorldHeritage/pages/1" class="text_area">
          <strong>世界遺産</strong>
        </a>
        
        <figure class="image_area10">
          <a href="http://localhost:3000/WorldHeritage/pages/1">
            <img src="~/assets/img/Ijinkan.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
          </a>
        </figure>
      </div>
    </main>
    <TheFooter />
  </div>
  
</template>

<style>
/* 共通 */
/* トップ画像 */
.top_img {
  overflow: hidden;
  position: relative;
}

/* imgのみ */
.item1 {
  opacity: 0;
  object-fit: cover;
  position: absolute;
  -webkit-animation: anime 30s 0s infinite;
  animation: anime 30s 0s infinite;
}

.item1:nth-of-type(2) {
  -webkit-animation-delay: 10s;
  animation-delay: 10s;
}

.item1:nth-of-type(3) {
  -webkit-animation-delay: 20s;
  animation-delay: 20s;
}

/* ふわっとアニメーション */
@keyframes anime {
  0% {
    opacity: 0;
  }
  30% {
    opacity: 1;
  }
  35% {
    opacity: 1;
  }
  50% {
    opacity: 0;
    z-index: 9;
  }
  100% {
    opacity: 0;
  }
}

@-webkit-keyframes anime {
  0% {
    opacity: 0;
  }
  30% {
    opacity: 1;
  }
  35% {
    opacity: 1;
  }
  50% {
    opacity: 0;
    z-index: 9;
  }
  100% {
    opacity: 0;
  }
}

.top_img p {
  margin: 0;                    /* 全余白の指定 */
  font-family: 'New Tegomin';   /* フォントの変更 */
  writing-mode: vertical-rl;    /* 縦書き */
  position: absolute;
  color: #fff;                /* 色変更 */
  transform: translate(-50%,-50%);  
}

.Kagoshima_about h1 {
  margin: 8px 0px;                    /* 全余白の指定 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}  

.headline h2 {
  margin: 8px 0px;                    /* 全余白の指定 */
  font-size: 40px;                    /* 文字の大きさ */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
  text-align: center;                 /* 左右の中央揃え */
}

.Kagoshima_about {text-align: center;}  /* 左右の中央揃え */

.Kagoshima_about p {
  font-family: serif;  /* フォントの変更 */
  font-weight: bold;   /* 文字の太さ */
}

a.text_area {
  font-size: 32px;      /* 文字の大きさ */
  font-family: serif;   /* フォントの変更 */
  text-align: center;   /* 左右の中央揃え */
  margin: 0 auto;       /* 全余白の指定 */
  color: rgb(0, 0, 0);  /* 文字の色指定 */
  text-decoration: none;  /* 下線の削除 */
}

/* スマホ（ 画面サイズが480px ） */
@media screen and (max-width:480px) {
  * {
	  float: none;
	  position: static;
    max-width: 100%;
  }

  .pc {display: none;}    /* 表示しない */

  .top_img {
    height: 240px;
    width: 480px;
  }

  .top_img img {
    height: 240px;
    width: 480px;
  }

  .Kagoshima_about h1 {font-size: 32px;}

  .Kagoshima_about p {
    margin: 0;            /* 全余白の指定 */
    font-size: 16px;      /* 文字の大きさ */
  }

/* 画像 */
  figure.image_area01 img,
  figure.image_area03 img,
  figure.image_area05 img,
  figure.image_area07 img,
  figure.image_area09 img {
    display: none;          /* 表示しない */
  }

  figure.image_area02 img,
  figure.image_area04 img,
  figure.image_area06 img,
  figure.image_area08 img,
  figure.image_area10 img {
    height: 16em;           /* 高さの指定 */
  }

  .introduction {
    margin: auto;           /* 全余白の指定 */
    text-align: center;     /* 左右の中央揃え */
    border-top: 2px solid #d5d4c3;  /* 下線表示 */
  }
}

/* PC（ 画面サイズが1024px以上 ）*/
@media screen and (min-width: 1024px) {
  .top_img {
    height: 550px;
    width: 1324px;
  }

  .top_img img {
    height: 550px;
    width: 1324px;
  } 

  .Kagoshima_about h1 {font-size: 40px;}  /* 文字の大きさ */

  .Kagoshima_about p {
    font-size: 25px;      /* 文字の大きさ */
    margin: 0;            /* 全余白の指定 */
  }

  figure.image_area {
    margin: auto;         /* 全余白の指定 */
    margin-top: 0;        /* 上余白の指定 */
    display: inline-block;  
  }

/* 画像の高さ・幅の調整 */
  figure.image_area01 img {
    height: 16em;
    width: 15em;
  }

  figure.image_area02 img {
    height: 16em;
    width: 15em;
  }

  figure.image_area03 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area04 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area05 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area06 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area07 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area08 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area09 img {
    height: 13em;
    width: 15em;
  }

  figure.image_area10 img {
    height: 13em;
    width: 15em;
  }

  .introduction {
    margin: auto;          /*全余白の指定 */
    padding: 8px 0px;      /*全余白の指定 */
    width: 1000px;         /* 幅の指定 */
    display: flex;         /* 横並び */
    align-items: center;   /* 上下の中央揃え */
    border-top: 2px solid #d5d4c3;    /* 上線 */
  }
}
</style>