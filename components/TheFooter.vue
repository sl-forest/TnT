<template>
  <div><head><head><meta name="viewport" content="width=device-width,initial-scale=1"></head></head>
    <footer class="footer">

      <p class="copyright">© 2023 TnT Inc.</p>

      <ul class="md-flex">
        <li><a href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
        <li><a href="http://localhost:3000/History/pages/1">歴史</a></li>
        <li><a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
        <li><a href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
        <li><a href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
      </ul>

    </footer>
  </div>
</template>

<style scoped>
/* スマホ */
@media screen and (max-width:480px) {

  * {
	  float: none;
	  position: static;
  }

  .footer {
    display: flex;
    justify-content: space-between;
    padding: 1.2rem;
    font-size: 15px;
    color: rgb(255, 255, 255);
    background: rgb(0, 0, 0);
    border-top: 1px solid #e5e7eb;
  }

  .footer a {
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  .footer a:hover {
    color: rgb(2, 243, 252);
  }

  .md-flex {
    display: flex;
    margin-right: 18px;
    padding: 0;
  }

  .md-flex li {
    font-size: 18px;
    font-weight: bold;
    float: left;
    writing-mode: tb-rl;
    writing-mode: vertical-rl; 
    -moz-writing-mode: vertical-rl;
    -o-writing-mode: vertical-rl;
    -webkit-writing-mode: vertical-rl;
  }

  .md-flex li + li {
    margin-left: 16px;
  }
}
/* PC */
@media screen and (min-width: 1024px) {
  .footer {
    display: flex;
    justify-content: space-between;
    padding: 1.2rem;
    font-size: 15px;
    color: rgb(255, 255, 255);
    background: rgb(0, 0, 0);
    border-top: 1px solid #e5e7eb;
  }

  .footer a {
    color: rgb(255, 255, 255);
    text-decoration: none;
  }

  .footer a:hover {
    color: rgb(2, 243, 252);
  }

  .copyright {
    margin: auto;
  }

  .md-flex {
    display: flex;
    margin-right: 3cm;
  }

  .md-flex li + li {
    margin-left: 16px;
  }
}
</style>