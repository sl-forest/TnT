<template>

  <footer id="footer02" class="outer-block">

    <div class="inner-block">
      <div class="wrap">
        
        <div class="logo">
          <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトロゴ"></a>
        </div>

        <h1>鹿児島紹介サイト</h1>

        <div class="cont">
          <ul class="nav">
            <li><a href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </div>
    </div><!-- /inner-block -->
    
    <div class="copyright"
      style="color: white; text-align: center; height: 32px;">
      © 2023 TnT Inc
    </div>
    
  </footer>

</template>

<style>

  .wrap h1 {
    color: white;
    margin: 0;
    margin-left: 16px;
  }

  #footer02 {
    background: #222;
  }
 
  #footer02 .nav li a {
    padding: 15px;
    color: #ccc;
  }
 
  #footer02 .c-btn {
    margin-left: 25px;
  }
 
@media screen and (min-width: 1024px) {
  #footer02 .logo {
    padding: 10px 0;
  }
 
  #footer02 .wrap {
    display: flex;
    justify-content: center;
    align-items: center;
  }
 
  #footer02 .cont {
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
  }
 
  #footer02 .nav {
    display: inline-block;
    list-style: none;
  }
 
  #footer02 .nav li {
    display: inline-block;
  }

  #footer02 .nav li a {
    text-decoration: none;
  }

  #footer02 .nav li a:hover {
    color: #22e5ff;
  }
}

@media only screen and (max-width: 480px) {
  #footer02 {
    padding: 20px 0 0;
  }
 
  #footer02 .inner-block {
    padding: 0;
  }
 
  .ie #footer02 .logo img,
  #footer02 .logo {
    text-align: center;
    display: block;
  }

  #footer02 .inner-block h1 {
    text-align: center;
  }

  #footer02 .nav {
    list-style: none;
  }

  #footer02 .nav li {
    border-top: 1px solid #555;
  }
 
  #footer02 .nav li a {
    text-decoration: none;
    padding: 12px 20px;
    display: block;
    background-size: 5px auto;
  }
 
  #footer02 .nav li:last-child {
    border-bottom: 1px solid #555;
  }
}
</style>