<template>
    <!-- ヘッダー高さ分の余白   -->
    <div class="header-box">
    <header>
        <div class="logo-space">
  
            <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>

            <div class="site-name">
                <h1>鹿児島紹介サイト</h1>
            </div>

        </div>

        <nav>
            <input id="menu_toggle" type="checkbox" />
            <label class="menu_btn" for="menu_toggle">
            <span></span>
            </label>

            <ul class="menu_box">
                <li><a class="menu_item" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
                <li><a class="menu_item" href="http://localhost:3000/History/pages/1">歴史</a></li>
                <li><a class="menu_item" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
                <li><a class="menu_item" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
                <li><a class="menu_item" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
            </ul>
        </nav>
    </header>
    </div>
</template>

<style lang="scss" scoped>
// PC
@media screen and (min-width: 1024px) {
    a:hover.menu_item {color: #ffd700;} /* 文字の色 */

    .header-box {height: 80px;} /* 高さ */
}

// 共通
@mixin burgerSpan {
    display: inline-block;        /* インラインブロック要素へ変更 */
    position: absolute;
    width: 100%;                  /* 横幅 */
    height: 3px;                  /* 高さ */
    background-color: #ffffff;  /* 背景 */
}

body {
    margin: 0;   /* 要素の外側余白*/
    padding: 0;  /* 要素の内側余白 */
}

header {
    position: fixed;
    padding: 1.6px 0;       /* 要素の内側余白 */
    left: 0;                /* 位置調整 */
    width: 100%;            /* 横幅 */
    background: #242428;  /* 背景 */
    z-index: 12;            /* 要素を重ねる順序の指定 */
    display: flex;          /* 親要素に対して子要素を横並びにする */ 
    justify-content: space-evenly;  

// スマホ
    @media screen and (max-width: 480px) {
        padding: 6.4px 0;   /* 要素の内側余白 */
        top: 0;             /* 位置調整 */
    }
  
}

.logo-space {
    margin: 0;      /* 要素の外側余白 */
    display: flex;  /* 親要素に対して子要素を横並びにする */
}

.logo-space a img {
    width: 64px;      /* 横幅 */
    height: 64px;     /* 高さ */
    padding-top: 6px; /* 要素の内側余白 */
}

.logo-space .site-name h1 {
    font-family: 'New Tegomin', serif;
    color: #fff;      /* サイトの名前の色 */
    margin: 0;          /* 要素の外側余白 */
    padding-top: 13px;  /* 要素の内側上余白 */
    padding-left: 16px; /* 要素の内側左余白 */
    font-size: 35px;    /* 文字の大きさ */
}

nav {
  display: flex;        /* 親要素に対して子要素を横並びにする */
  align-items: center;  /* 上下の中央揃え */
  margin-top: 8px;      /* 要素の外側余白 */
  
// スマホ
  @media screen and (max-width: 480px) {display: inline;}   /* インライン要素へ変更 */
}

.menu_box {
  display: flex;        /* 親要素に対して子要素を横並びにする */
  flex-direction: row;
  list-style-type: none;
  
// スマホ
  @media screen and (max-width: 480px) {
    flex-direction: column;
    position: fixed;
    visibility: hidden;
    top: 0;                                     /* 位置調整 */
    left: 0;                                    /* 位置調整 */
    width: 100%;                                /* 横幅 */
    height: 15em;                               /* 高さ */
    margin: -600px 0 0 0;                       /* 要素の外側余白 */
    padding: 0.6em 0;                           /* 要素の内側余白 */
    text-align: center;                         /* 左右の中央揃え */
    background-color: #2d303a;                /* 背景 */
    box-shadow: 1px 0 6px rgba(0, 0, 0, .2);  /* 影 */
    z-index: 1;                                 /* 要素を重ねる順序の指定 */
    transition-duration: 0.5s;                  /* アニメーションが完了するまでの時間 */
  }

}

.menu_item {
    display: flex;             /* 親要素に対して子要素を横並びにする */
    flex-direction: column;
    padding: 0 1em 0 1.9em;
    color: #ffffff;
    font-family: 'New Tegomin', serif;  /* フォント変更 */
    font-size: 15px;                    /* 文字の大きさ */
    font-weight: 400;                   /* 文字の太さ */
    text-decoration: none;              /* 下線無効 */
    text-transform: uppercase;

// スマホ
    @media screen and (max-width: 480px) {
        display: block;     /* ブロック要素へ変更 */
        padding: 12px 24px; /* 要素の内側余白 */
        color: #ffffff;   /* 文字の色 */
        font-size: 18px;    /* 文字の大きさ */
        transition-duration: 0.5s;  /* アニメーションが完了するまでの時間 */

        &:hover {background-color: #4f5464;}

    }

}

#menu_toggle {
    opacity: 0; /* 不透明度 */
  
    &:checked ~ .menu_btn > span {
        transform: rotate(45deg);
    }

    &:checked ~ .menu_btn > span::before {
        top: 0;                 /* 位置調整 */
        transform: rotate(0);
        background: #f06c64;
    }

    &:checked ~ .menu_btn > span::after {
        top: 0;                     /* 位置調整 */
        transform: rotate(90deg);
        background: #f06c64;
    }

    &:checked ~ .menu_box {
        visibility: visible;
        margin: 0;           /* 要素の外側余白 */
        left: 0;             /* 位置調整 */
    }

}

.menu_btn {
    transition-duration: 0.25s; /* アニメーションが完了するまでの時間 */
    box-sizing: border-box;
    display: flex;              /* 親要素に対して子要素を横並びにする */
    align-items: center;
    position: relative;
    bottom: 2px;                /* 位置調整 */
    width: 26px;                /* 横幅 */
    height: 26px;               /* 高さ */
    cursor: pointer;
    z-index: 2;                /* 要素を重ねる順序の指定 */

    span {
    @include burgerSpan;

    &::before {
        @include burgerSpan;
        content: '';
        top: -8px;                  /* 位置調整 */
        transition-duration: 0.25s; /* アニメーションが完了するまでの時間 */
    }

    &::after {
        @include burgerSpan;
        content: '';
        top: 8px;                   /* 位置調整 */
        transition-duration: 0.25s; /* アニメーションが完了するまでの時間 */
    }

}

// PC
@media screen and (min-width: 1024px) {display: none;}

}
</style>