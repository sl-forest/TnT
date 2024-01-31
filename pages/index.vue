<template>
  
  <div>
    <Loding />
    <TheHeader />

    <main>
      <div class="top_img">

        <img class="item1" src="~/assets/img/Top01.jpg" alt="トップ画像">
        <img class="item1" src="~/assets/img/Top02.jpg" alt="トップ画像">
        <img class="item1" src="~/assets/img/Top03.jpg" alt="トップ画像">

        <div class="img_font">
          鹿児島へ<br>
          &emsp; ようこそ
        </div>

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
          <strong>歴史</strong>
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
            <img src="~/assets/img/Buridaikon.jpg" alt="ぶり大根">
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
* {margin: 0;}  /* 要素の外側余白 */

/* トップ画像 */
.top_img {
  overflow: hidden;   /* 要素からはみ出た部分を非表示 */
  position: relative; /* 現在位置を基準に相対位置を指定 */
}

.item1 {
  opacity: 0;         /* 不透明度 */
  object-fit: cover;  /* 画像のトリミング */
  position: absolute; /* 親要素を基準に絶対配置を指定 */
  width: 100%;        /* 横幅 */
  height: 100%;       /* 高さ */
  -webkit-animation: anime 21s 0s infinite; /* 30秒間アニメーションを繰り返し再生 */
  animation: anime 21s 0s infinite;         /* 30秒間アニメーションを繰り返し再生 */
}

.item1:nth-of-type(2) {
  -webkit-animation-delay: 7s; /* アニメーション開始までの指定 */
  animation-delay: 7s;         /* アニメーション開始までの指定 */
}

.item1:nth-of-type(3) {
  -webkit-animation-delay: 14s; /* アニメーション開始までの指定 */
  animation-delay: 14s;         /* アニメーション開始までの指定 */
}

/* ふわっとアニメーション */
@keyframes anime {
  0% {opacity: 0;}  /* 不透明度 */
  30% {opacity: 1;} /* 不透明度 */
  35% {opacity: 1;} /* 不透明度 */
  
  50% {
    opacity: 0; /* 不透明度 */
    z-index: 9; /* 要素を重ねる順序の指定 */
  }

  100% {opacity: 0;}  /* 不透明度 */
}

@-webkit-keyframes anime {
  0% {opacity: 0;}  /* 不透明度 */
  30% {opacity: 1;} /* 不透明度 */
  35% {opacity: 1;} /* 不透明度 */

  50% {
    opacity: 0; /* 不透明度 */
    z-index: 9; /* 要素を重ねる順序の指定 */
  }

  100% {opacity: 0;} /* 不透明度 */
}

/* トップ画像の上の文字 */
.img_font {
  margin: 0;                        /* 要素の外側余白 */
  font-size: 64px;                  /* 文字の大きさ */
  text-shadow: 1px 1px 3px #444;  /* 背景 */
  font-family: 'New Tegomin';       /* フォント変更 */
  writing-mode: vertical-rl;        /* 縦書き */
  z-index: 11;                      /* 要素を重ねる順序の指定 */
  top: 16%;                         /* 位置調整 */
  left: 72%;                        /* 位置調整 */
  position: absolute;               /* 親要素を基準に絶対配置を指定 */
  color: rgb(255, 255, 255);      /* 文字の色 */
}

.Kagoshima_about h1 {
  margin: 8px 0;                      /* 要素の外側余白 */
  font-family: 'New Tegomin', serif;  /* フォント変更 */
}  

.headline h2 {
  margin: 8px 0;                      /* 要素の外側余白*/
  font-size: 40px;                    /* 文字の大きさ */
  font-family: 'New Tegomin', serif;  /* フォント変更 */
  text-align: center;                 /* 中央揃え */
}

.Kagoshima_about {text-align: center;}  /* 中央揃え */

.Kagoshima_about p {
  font-family: serif;  /* フォント変更 */
  font-weight: bold;   /* 文字の太さ */
}

a.text_area {
  font-size: 32px;        /* 文字の大きさ */
  font-family: serif;     /* フォント変更 */
  text-align: center;     /* 中央揃え */
  margin: 0 auto;         /* 要素の外側余白*/
  color: rgb(0, 0, 0);  /* 文字の色 */
  text-decoration: none;  /* 下線無効 */
}

/* スマホ（ 画面サイズが480px ） */
@media screen and (max-width:480px) {
  .pc {display: none;}  /* 表示しない */

/* トップ画像 */
  .top_img {
    margin-top: 90px;   /* 要素の外側の余白 */
    height: 16rem;      /* 高さ */
  }

  .img_font {font-size: 32px;}            /* 文字の大きさ */
  .Kagoshima_about h1 {font-size: 32px;}  /* 文字の大きさ */

  .Kagoshima_about p {
    margin: 0;            /* 要素の外側余白 */
    font-size: 16px;      /* 文字の大きさ */
  }

/* 画像 */
  figure.image_area02,
  figure.image_area04,
  figure.image_area06,
  figure.image_area08,
  figure.image_area10
  {margin: 8px 0;}  /* 要素の外側余白 */

  figure.image_area01 img,
  figure.image_area03 img,
  figure.image_area05 img,
  figure.image_area07 img,
  figure.image_area09 img
  {display: none;}  /* 表示しない */

  figure.image_area02 img,
  figure.image_area04 img,
  figure.image_area06 img,
  figure.image_area08 img,
  figure.image_area10 img {
    width: 320px; /* 横幅 */
  } 

  .introduction {
    margin: auto;           /* 要素の外側余白 */
    text-align: center;     /* 中央揃え */
    border-top: 2px solid #d5d4c3;  /* 下線表示 */
  }
}

/* PC（ 画面サイズが1024px以上 ）*/
@media screen and (min-width: 1024px) {
/* トップ画像 */
  .top_img {
    width: auto;    /* 横幅 */
    height: 36rem;  /* 高さ */
  }

  .fuchidori {font-size: 64px;}           /* 文字の大きさ */
  .Kagoshima_about h1 {font-size: 40px;}  /* 文字の大きさ */

  .Kagoshima_about p {
    font-size: 25px;  /* 文字の大きさ */
    margin: 0;        /* 要素の外側余白*/
  }

  figure.image_area {
    margin: auto;           /* 要素の外側余白 */
    margin-top: 0;          /* 要素の外側上余白 */
    display: inline-block;  /* インラインブロック要素へ変更 */ 
  }

/* 画像の横幅・高さの調整 */
  figure.image_area01 img,
  figure.image_area02 img,
  figure.image_area03 img,
  figure.image_area04 img,
  figure.image_area05 img,
  figure.image_area06 img,
  figure.image_area07 img,
  figure.image_area08 img,
  figure.image_area09 img,
  figure.image_area10 img {
    width: 224px;
    height: 200px;
  }

  .introduction {
    margin: auto;         /* 要素の外側余白 */
    padding: 8px 0;       /* 要素の内側余白 */
    width: 1000px;        /* 幅 */
    display: flex;        /* 親要素に対して子要素を横並びにする */
    align-items: center;  /* 中央揃え */
    border-top: 2px solid #d5d4c3;  /* 上線 */
  }
}
</style>