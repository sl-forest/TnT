<template>
  
  <div>
    <TheHeader />

    <main>
      <div class="top_img">
        <img src="~/assets/img/Top_img1.png" alt="トップ画像">
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
.Kagoshima_about h1 {font-family: 'New Tegomin', serif;}

.headline h2 {font-family: 'New Tegomin', serif;}

.Kagoshima_about {text-align: center;}

.Kagoshima_about p {font-family: serif;}

html {font-family: sans-serif;}

a.text_area {
  font-size: 32px;
  font-family: serif;
  text-align: center;
  display: inline-block;
  width: 300px;
  margin: 0 auto;
  color: rgb(0, 0, 0);
  text-decoration: none;
}

/* スマホ（ 画面サイズが480px ） */
@media screen and (max-width:480px) {
  * {
	  float: none;
	  position: static;
  }

  .pc {display: none;}

  .Kagoshima_about h1 {
    margin: 0;
    font-size: 32px;
  }

  .Kagoshima_about p {
    font-size: 16px;
    margin: 0;
  }

  .top_img img {
    max-width: 100%;
    margin: 0;
  }

  /* 紹介 */
  .headline h2 {
    font-size: 40px;
    text-align: center;
    margin-bottom: 16px;
  }

  figure.image_area01 img,
  figure.image_area03 img,
  figure.image_area05 img,
  figure.image_area07 img,
  figure.image_area09 img {
    display: none;
  }

  figure.image_area02 img,
  figure.image_area04 img,
  figure.image_area06 img,
  figure.image_area08 img,
  figure.image_area10 img {
    height: 16em;
  }

  .introduction {
    margin: auto;
    text-align: center;
    align-items: center;
    justify-content: space-around;
    border-top: 2px solid #d5d4c3;
  }
}

/* PC（ 画面サイズが1024px以上 ）*/
@media screen and (min-width: 1024px) {
  .Kagoshima_about h1 {
    font-size: 40px;
    margin-bottom: 8px;
  }

  .Kagoshima_about p {
    font-size: 25px;
    margin: 0;
  }

  .top_img img {
    max-width: 100%;
  }

  /* 紹介 */
  .headline h2 {
    font-size: 40px;
    text-align: center;
    margin-bottom: 16px;
  }

  figure.image_area {
    margin: auto;
    margin-top: 0;
    display: inline-block;
  }

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
    margin: auto;
    width: 1000px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    border-top: 2px solid #d5d4c3;
  }
}
</style>