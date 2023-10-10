<template>

  <div>
    <header>
      <!-- ロゴ -->
      <div class="logo">
        <a href="http://localhost:3000"><img src="~/assets/img/Kagoshima_logo.png" alt="サイトのロゴ"></a>
      </div>

      <!--  サイトの名前 -->
      <div class="site-name">
        <a href="http://localhost:3000"><h1>鹿児島紹介サイト</h1></a>
      </div>

      <!-- メニュー -->
      <nav>
        <div class="menu">
          <ul class="item">
            <li><a class="item-link" href="http://localhost:3000/Craft/pages/1">工芸品</a></li>
            <li><a class="item-link" href="http://localhost:3000/History/pages/1">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000/LocalCuisine/pages/1">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000/TraditionalCulture/pages/1">伝統芸能</a></li>
            <li><a class="item-link" href="http://localhost:3000">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
      <h1>豚骨</h1>
        <div class="LocalCuisine">
            <div class = LocalCuisine_img>
                <img src="~/assets/img/Tonkotsu.jpg" alt="豚骨">
            </div>
            
            <div class = LocalCuisine_note>
                <h2>伝承地域</h2>
                <p>鹿児島県全域</p>
                <h2>食材</h2>
                <p>豚骨（スペアリブ）、こんにゃく、大根、ごぼう、焼酎、味噌、砂糖</p>
                <h2>歴史</h2>
                <p>薩摩武士たちが狩場や戦場などでつくった野外料理がはじまりで、かの西郷隆盛も好物であったといわれている。</p>
                <p>「豚骨」には、豚肉と麦味噌、黒砂糖、そして芋焼酎という、鹿児島県ならではの食材がふんだんに盛り込まれているため、今日にいたるまで鹿児島県を代表する郷土料理として親しまれている。</p>
            </div>
        </div>

        <div class = "recipe">
          <h3>材料（3～4人分）</h3>
          <ul class = "LocalCuisine_memu">

            <li>
              <ul class = "list">
                <li>豚骨（スペアリブ）</li>
                <li>400g</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>大根</li>
                <li>8cm</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>人参</li>
                <li>1本</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>こんにゃく</li>
                <li>1袋（200g）</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>油</li>
                <li>適量</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>焼酎</li>
                <li>1/4cup</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>しょうが</li>
                <li>1片</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>だし汁</li>
                <li>3cup</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>砂糖（おすすめは黒砂糖）</li>
                <li>大さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>合わせ味噌</li>
                <li>大さじ5</li>
              </ul>
            </li>

            <li>
              <ul class = "list">
                <li>酒</li>
                <li>大さじ2</li>
              </ul>
            </li>

            <li>
              <ul class = "list_last">
                <li>醤油</li>
                <li>大さじ2</li>
              </ul>
            </li>

          </ul>

              <h3>作り方</h3>

              <ul class = "LocalCuisine_make">
                
                <li>
                  <div class = "num">1</div>
                  <div class = "text">
                    大根は2cm幅の半月切りに、人参も程よい大きさにカットしておく。
                  </div>
                </li>

                <li>
                  <div class = "num">2</div>
                  <div class = "text">
                    こんにゃくは味が染みやすいよう切り込みを入れて食べやすい大きさに切り、熱湯で下湯でしておく。
                  </div>
                </li>

                <li>
                  <div class = "num">3</div>
                  <div class = "text">
                    	フライパンに油を入れて熱し、豚骨を焼き付けて、焼酎を加え水気が無くなるまで煮絡める。（臭みが取れる）
                  </div>
                </li>

                <li>
                  <div class = "num">4</div>
                  <div class = "text">
                    圧力鍋に豚骨と☆を加え（味噌は味噌漉しで溶く）１０分加圧する。
                  </div>
                </li>

                <li>
                  <div class = "num">5</div>
                  <div class = "text">
                    自然に圧が抜けたら大根・人参・こんにゃくと醤油を入れ、再度5分加圧する。
                  </div>
                </li>

                <li>
                  <div class = "num">6</div>
                  <div class = "text">
                    圧が抜けたら落し蓋（クシャクシャにしたアルミホイル使用）をし、味を見ながら煮汁が半量位になるまで煮詰める。
                  </div>
                </li>

                <li>
                  <div class = "num">7</div>
                  <div class = "text">
                    前日に仕込んで味を染み込ませまる。表面に脂肪が浮いて来るので丁寧に取り除くことでカロリーダウンになる。
                  </div>
                </li>

                <li>
                  <div class = "num">8</div>
                  <div class = "text">
                    温めて器に盛り、お好みで塩茹でしたいんげん等添えると彩りが良い。
                  </div>
                </li>

              </ul>
        </div>
    </main>

  <fotter>

  </fotter>
  
  </div>

</template>

<style>
    /* スマホ向けスタイル */

    /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
      main {
        max-width: 1024px;
        margin: 0 auto;
      }
      
      header {
        flex-wrap: wrap; /*折り返し */
        display: flex;  /*ヘッダーの下の要素を並列に*/
        padding: 0; /*ヘッダーの位置調整*/
        background: #333; /*ヘッダーの背景色*/
      }
      
      .site-name h1 {
        color: #fff;  /*サイトの名前の色*/
      }

      .site-name a {
        text-decoration: none;
      }

      .logo {
        margin: 5px 15px;
      }

      .logo a img {
        width: 65px;  /*ロゴ画像の幅調整*/
        height: 65px; /*ロゴ画像の高さ調整*/
        padding-top: 1.5px; /*ロゴの位置調整*/
      }
      
      nav ul {
      padding-left: 24px;
    }

      .item ul {
        display: inline-block;
        margin-top: 25px;
    }

      ul {
        list-style: none;
        padding: 0;
      }
      
      .item li {
        display: inline-block;
        list-style: none;
        margin-right: 16px;
        padding: 10px;
        border-bottom: 2px solid #2ac5b3;
    }

      .item li a {
        color: #fff;  /*メニューの色*/
        text-decoration: none;  /*メニューの下線を消す*/
      }

    /*郷土料理説明*/
      .LocalCuisine {
        display: flex;
        padding-bottom: 24px;
      }

      .LocalCuisine h1 {
        margin: 1.6px auto;
      }

      .LocalCuisine_img img {
        height: 10cm;
      }

      .LocalCuisine_img p {
        margin: 0;
      }

    /*材料*/
      .LocalCuisine_note {
        margin-top: 0.6cm;
        margin-left: 16px;
      }

      .LocalCuisine_note h2 {
        margin: 8px auto;
      }

      .LocalCuisine_note p {
        margin: 8px auto;
      }

      .recipe {
        background: #d2e7f3;
        padding: 24px;
      }

      .recipe h3 {
        margin: 0;
        padding: 0;
        border-bottom: 1px solid #1b1b1b;
      }

      .list {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 6px;
        border-bottom: 1px solid #9e9595;
      }

      .list_last {
        display: flex;
        flex-flow: row wrap;
        justify-content: space-between;
        padding: 8px 0 64px;
      }

    /*作り方*/
      .LocalCuisine_make {
        list-style: none;
        margin: 0;
        font-size: 1em;
        padding: 0;
      }

      .LocalCuisine_make li {
        display: table;
        padding: 16px 0;
        border-bottom: 1px solid #9e9595;
      }

      .num {
        display: inline-block;
        font-size: 1.714em;
        width: 40px;
        margin-top: -5px;
        padding-right: 10px;
      }

      .text {
        display: table-cell;
        vertical-align: top;
        width: 100%;
      }
    }
</style>