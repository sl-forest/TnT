<template>

  <footer id="footer" class="outer-block">

    <div class="inner-block">
      <div class="wrap">
        
        <div class="logo">
          <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo-min.png" alt="サイトロゴ"></a>
        </div>

        <h1>鹿児島紹介サイト</h1>

        <div class="serach-sm">
          <form method="get" action="http://www.google.co.jp/search" class="search-form" target="_blank">
          <label>  
            <input type="text" name="q" placeholder="Google検索">
          </label>
            <button type="submit" name="btng" value="検索"></button>
          </form>
        </div>

        <div class="cont">
          <ul class="nav">
            <li><a href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>

        <div class="serach-pc">
          <form method="get" action="http://www.google.co.jp/search" class="search-form" target="_blank">
          <label>  
            <input type="text" name="q" placeholder="Google検索">
          </label>
            <button type="submit" name="btng" value="検索"></button>
          </form>
        </div>

      </div>
    </div><!-- /inner-block -->
    
    <div class="copyright">
      © 2023 TnT.
    </div>
    
  </footer>

</template>

<style>
/* 共通 */
  #footer {background: #242428;}      /* 背景 */

  .wrap h1 {
    font-family: 'New Tegomin', serif;  /* フォント変更 */
    color: white;                     /* 文字の色 */
    margin: 0;                          /* 要素の外側余白 */
    padding: 0;                         /* 要素の内側余白 */
    padding-top: 21px;                  /* 要素の内側上余白 */
    padding-left: 16px;                 /* 要素の内側下余白 */
  }
 
  #footer .nav li a {
    font-family: 'New Tegomin', serif;  /* フォントの変更 */
    color: #ffffff;                   /* 文字の色 */
    padding: 15px;                      /* 要素の内側余白 */
  }
 
  #footer .c-btn {margin-left: 25px;}   /* 要素の外側左余白 */

  /* 検索 */
  #footer form {margin: auto;}  /* 要素の外側余白 */

  #footer .search-form {
    display: flex;        /* 親要素に対して子要素を横並びにする */
    align-items: center;  /* 中央揃え */
    overflow: hidden;     /* 要素からはみ出た部分を非表示 */
    border-radius: 3px;   /* 角を丸める */
    margin: 0;            /* 要素の外側余白 */
  }

  #footer .search-form input {
    width: 250px;                 /* 横幅 */
    height: 45px;                 /* 高さ */
    padding: 5px 15px;            /* 要素の内側余白 */
    border: none;                 /* 枠線削除 */
    border-radius: 3px 0 0 3px;   /* 角を丸める */
    box-sizing: border-box;       /* ボックスサイズの指定 */
    background-color: #e6edf3;  /* 背景 */
    font-size: 1em;               /* 文字の大きさ */
    outline: none;                /* 輪郭削除 */
  }

  #footer .search-form input::placeholder {color: #767d83;} /* 文字の色 */

  #footer .search-form button {
    display: flex;                /* 親要素に対して子要素を横並びにする */
    justify-content: center;      /* 横並び要素の左右中央揃え */
    align-items: center;          /* 中央揃え */
    width: 50px;                  /* 横幅 */
    height: 45px;                 /* 高さ */
    border: none;                 /* 枠線削除 */
    border-radius: 0 3px 3px 0;   /* 角を丸める */
    background-color: #2589d0;  /* 背景 */
    cursor: pointer;              /* カーソルを指さし表示 */
  }

  #footer .search-form button::after {
    width: 20px;    /* 横幅 */
    height: 20px;   /* 高さ */
    background-image: url('data:image/svg+xml;charset=utf8,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2024%2024%22%3E%20%3Cpath%20d%3D%22M23.7%2020.8%2019%2016.1c-.2-.2-.5-.3-.8-.3h-.8c1.3-1.7%202-3.7%202-6C19.5%204.4%2015.1%200%209.7%200S0%204.4%200%209.7s4.4%209.7%209.7%209.7c2.3%200%204.3-.8%206-2v.8c0%20.3.1.6.3.8l4.7%204.7c.4.4%201.2.4%201.6%200l1.3-1.3c.5-.5.5-1.2.1-1.6zm-14-5.1c-3.3%200-6-2.7-6-6s2.7-6%206-6%206%202.7%206%206-2.6%206-6%206z%22%20fill%3D%22%23fff%22%3E%3C%2Fpath%3E%20%3C%2Fsvg%3E'); /* 虫眼鏡画像 */ 
    background-repeat: no-repeat; /* 画像を繰り返さない */
    content: '';                  /* 画像を表示 */
  }

/* コピーライト */
  #footer .copyright {
    text-align: center; /* 中央揃え */
    height: 32px;       /* 高さ */
    color: white;     /* 文字の色 */
  }

/* PC */
@media screen and (min-width: 1024px) {
  #footer .wrap {
    display: flex;            /* 親要素に対して子要素を横並びにする */
    justify-content: center;  /* 横並び要素の中央揃え */
    align-items: center;      /* 中央揃え */
  }

  #footer .logo img {
    padding: 0;       /* 要素の内側余白 */
    margin-top: 24px; /* 要素の外側上余白 */
    height: 80px;     /* 高さ */
  }

  #footer .serach-sm {display: none;} /* 表示しない */

  #footer .serach-pc {
    margin-top: 28px;   /* 要素の外側上余白 */
    margin-left: 24px;  /* 要素の外側左余白 */
    margin-bottom: 0;   /* 要素の外側下余白 */
  }
 
  #footer .nav {
    display: inline-block;  /* インラインブロック要素へ変更 */
    margin-top: 30px;       /* 要素の外側上余白 */
    margin-bottom: 0;       /* 要素の外側下余白 */
  }
 
  #footer .nav li {display: inline-block;}    /* インラインブロック要素へ変更 */
  #footer .nav li a {text-decoration: none;}  /* 下線無効 */
/* マウスオーバー */
  #footer .nav li a:hover {color: #ffd700;} /* 文字の色 */
}

/* スマホ */
@media only screen and (max-width: 480px) {
  #footer {padding: 8px 0;}           /* 要素の内側余白 */
  .wrap h1 {padding: 8px 0;}          /* 要素の内側余白 */
  #footer .inner-block {padding: 0;}  /* 要素の内側余白 */

   #footer .logo img {
    padding: 0;       /* 要素の内側余白 */
    margin-top: 16px; /* 要素の外側上余白 */
    width: 25%;       /* 横幅 */
  }
 
  .ie #footer .logo img,
  #footer .logo {
    text-align: center; /* 中央揃え */
    display: block;     /* ブロック要素へ変更 */
  }

  #footer .inner-block h1 {text-align: center;} /* 中央揃え */
  #footer .serach-pc {display: none;}           /* 表示しない */

  #footer .serach-sm {
    margin-left: 88px;    /* 要素の外側左余白 */
    margin-top: 12px;     /* 要素の外側上余白 */
    margin-bottom: 32px;  /* 要素の外側下余白 */
  }

  #footer .nav {
    padding: 0 40px;    /* 要素の内側余白 */
    list-style: none;   /* 中点削除 */
  }

  #footer .nav li {border-top: 1px solid #555;} 
 
  #footer .nav li a {
    text-decoration: none;  /* 下線無効 */
    padding: 12px 20px;     /* 要素の内側余白 */
    display: block;         /* ブロック要素へ変更 */
  }
 
  #footer .nav li:last-child {border-bottom: 1px solid #555;} /* 下線 */
  #footer .copyright {padding: 8px 0}                           /* 要素の内側余白 */
}
</style>