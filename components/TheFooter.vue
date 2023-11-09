<template>
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
</template>

<style scoped>
  .footer {
    display: flex;
    justify-content: space-between;
    padding: 2rem;
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
  }

  .md-flex li + li {
    margin-left: 16px;
  }

  /* 検索フォーム */
  #form {
    position: relative; 
    margin-bottom: 20px;	
  }
</style>