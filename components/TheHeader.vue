<template>

    <header>
        <div class="logo-space">
            
            <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>

            <div class="site-name">
                <h1>鹿児島紹介サイト</h1>
            </div>

        </div>

        <!--The hamburger appears, when the screen resolution becomes 760px-->
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
</template>

<style lang="scss" scoped>
// PC
@media screen and (min-width: 1024px) {
    a:hover.menu_item {
        color: #4eeaff;
    }
}

// 共通
@mixin burgerSpan {
    display: inline-block;
    position: absolute;
    width: 100%;
    height: 3px;
    background-color: #ffffff;
}

body {
    margin: 0;
    padding: 0;
}

header {
    display: flex;
    align-items: center;
    padding: 1.4em;
    background: #2d303a;
    border-bottom: 2px solid #3c4356;
    justify-content: space-evenly;
}

.logo-space {
    margin: 0;
    display: flex;
}

.logo-space a img {
    width: 64px;      /*ロゴ画像の幅調整*/
    height: 64px;     /*ロゴ画像の高さ調整*/
    padding-top: 6px; /*ロゴの位置調整*/
}

.logo-space .site-name h1 {
  font-family: sans-serif;
  color: #fff;  /*サイトの名前の色*/
  margin-top: 13px;
  margin-left: 16px;
  margin-bottom: 0;
  font-size: 35px;
}

nav {
  display: flex;
  align-items: center;
  
// スマホ
  @media screen and (max-width: 480px) {
    nav {display: inline;}
  }
  
}

.menu_box {
  display: flex;
  flex-direction: row;
  list-style-type: none;
  
// スマホ
  @media screen and (max-width: 480px) {
    flex-direction: column;
    position: fixed;
    visibility: hidden;
    top: 0;
    left: 0;
    width: 100%;
    height: 15em;
    margin: -600px 0 0 0;
    padding: 0.6em 0;
    text-align: center;
    background-color: #2d303a;
    box-shadow: 1px 0 6px rgba(0, 0, 0, .2);
    z-index: 1;
    transition-duration: 0.5s;
  }

}

.menu_item {
    display: flex;
    flex-direction: column;
    padding: 0 1em 0 1.9em;
    color: #ffffff;
    font-family: sans-serif;
    font-size: 14px;
    font-weight: 400;
    text-decoration: none;
    text-transform: uppercase;

// スマホ
    @media screen and (max-width: 480px) {
        display: block;
        padding: 12px 24px;
        color: #ffffff;
        font-size: 18px;
        transition-duration: 0.5s;

        &:hover {background-color: #4f5464;}

    }

}

#menu_toggle {
    opacity: 0;
  
    &:checked ~ .menu_btn > span {
        transform: rotate(45deg);
    }

    &:checked ~ .menu_btn > span::before {
        top: 0;
        transform: rotate(0);
        background: #f06c64;
    }

    &:checked ~ .menu_btn > span::after {
        top: 0;
        transform: rotate(90deg);
        background: #f06c64;
    }

    &:checked ~ .menu_box {
        visibility: visible;
        left: 0;
        margin: 0;
    }

}

.menu_btn {
    transition-duration: 0.25s;
    box-sizing: border-box;
    display: flex;
    align-items: center;
    position: relative;
    bottom: 2px;
    width: 26px;
    height: 26px;
    cursor: pointer;
    z-index: 2;

    span {
    @include burgerSpan;

    &::before {
        @include burgerSpan;
        content: '';
        top: -8px;
        transition-duration: 0.25s;
    }

    &::after {
        @include burgerSpan;
        content: '';
        top: 8px;
        transition-duration: 0.25s;
    }

}

// PC
@media screen and (min-width: 1024px) {display: none;}

}
</style>