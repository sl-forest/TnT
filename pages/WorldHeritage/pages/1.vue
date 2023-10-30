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
            <li><a class="item-link" href="http://localhost:3000/TouristSpot/pages/1">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000/WorldHeritage/pages/1">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
        <h1>「世界遺産」</h1>
        <h2 class = worldheritage_headline>関吉の疎水溝</h2>
        <div class="worldheritage">
            <div class = worldheritage_img>
                <img src="~/assets/img/Sekiyoshi.jpg" alt="関吉の疎水溝">
            </div>
            
            <div class = explanation>
                <p>集成館では高炉や鑽開台の動力源として水車を使用しており、水が必要だったため、新たな水路をこの場所に築いた。</p>
                <p>世界文化遺産「明治日本の産業革命遺産」の構成資産。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/SekiyoshinoSosuiko">スポット情報</a>
        </div>

        <h2 class = worldheritage_headline>寺山炭窯跡</h2>
        <div class="worldheritage">
            <div class = worldheritage_img>
                <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
            </div>

            <div class = explanation>
                <p>集成館事業で使用する白炭を増産するために建設した寺山炭窯の跡。</p>
                <p>炭窯は斜面を造成して凝灰岩を積み上げて建設、その大きさは国内最大級。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/TerayamaCharcoalKiln">スポット情報</a>
        </div>

        <h2 class = worldheritage_headline>旧集成館「反射炉跡」</h2>
        <div class="worldheritage">
            <div class = worldheritage_img>
                <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
                <p>写真協力：</p>
                <p>公益社団法人　鹿児島県観光連盟</p>
            </div>

            <div class = explanation>
                <p>1851年、薩摩藩主に就任した島津斉彬は、富国強兵・殖産興業を唱え、集成館事業を興した。</p>
                <p>集成館事業の中核となったのが、鹿児島市磯に築かれた工場群「集成館」。</p>
                <p>製鉄大砲鋳造、洋式艦船の建造、製鉄や紡績、ガラス製造、活版印刷などがおこなわれた。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ReverberatoryFurnaceRuins">スポット情報</a>
        </div>

        <h2 class = worldheritage_headline>旧集成館「旧鹿児島紡績所技師館」（異人館）</h2>
        <div class="worldheritage">
            <div class = worldheritage_img>
                <img src="~/assets/img/Ijinkan.jpeg" alt="旧集成館「旧鹿児島紡績所技師館」（異人館）">
                <p>写真協力：</p>
                <p>公益社団法人　鹿児島県観光連盟</p>
            </div>

            <div class = explanation>
                <p>日本で最初期の木造西洋建築。</p>
                <p>西欧人たちがアジアなどの植民地によく建設したコロニアル様式の建物。</p>
                <p></p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/Ijinkan">スポット情報</a>
        </div>

        <h2 class = worldheritage_headline>旧集成館機械工場（尚古集成館）</h2>
        <div class="worldheritage">
            <div class = worldheritage_img>
                <img src="~/assets/img/Shoko Shuseikan Museum.jpg" alt="旧集成館機械工場（尚古集成館）">
            </div>

            <div class = explanation>
                <p>洋式船や蒸気機関の修理、部品製造を行った集成館の機械工場。</p>
                <p>竹下清右衛門は長崎製鉄所などの西洋式の建物を参考に工場を建設。</p>
                <p>現在は博物館（尚古集成館）として島津家や集成館事業の歴史を学ぶことができる。</p>
            </div>
            <a class ="explanation-link" href="http://localhost:3000/WorldHeritage/pages/ShokoShuseikanMuseum">スポット情報</a>
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

    /*フォーム全体*/
      #form1{
        margin-left: auto; 
        margin-right: auto;
        position: relative;  /*フォームの相対位置*/	
        max-width: 270px;  /*フォームのサイズ*/
        margin-bottom: 15px; /*フォームの下に余白*/	 	
      }

    /*検索ボックス*/
      #sbox{
        left: 0;  /*検索ボタンの位置調整*/
        top: 13.5px; 	/*検索ボタンの位置調整*/
        outline: 0;  /*クリック時の青い枠線消す*/	
        height: 35px;  /*検索ボックスの高さ*/	
        padding: 0 10px; /*テキスト位置調整*/	 
        border-radius: 2px 0 0 2px;  /*検索ボックスの角を丸める*/		
        background:#eee;  /*検索ボックスの背景カラー*/		
      }

    /*検索ボタン*/
      #sbtn{
        width:70px; /*検索ボタンの横幅*/ 
        height:40px;  /*検索ボタンの縦幅*/ 
        border-radius:0 2px 2px 0;  /*検索ボタンの角を丸める*/ 
        background:#7fbfff; /*検索ボタンの背景カラー*/ 
        border:none;  /*検索ボタンの枠線を消す*/ 
        color:#fff; /*検索ボタンのテキストカラー*/ 
        font-weight:bold; /*検索ボタンのテキスト太字*/ 
        font-size:16px; /*検索ボタンのフォントサイズ*/ 
      }

    /*検索ボタンマウスオーバー時*/
      #sbtn:hover{
        color:#666; /*検索ボタンマウスオーバー時のフォントカラー*/ 
      }

      h1 {
        margin-bottom: 0;
      }

      h2.worldheritage_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 世界遺産一覧説明 */
      .worldheritage {
        display: flex;
      }

      .worldheritage p {
        margin: 0;
        font-size: 14px;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 世界遺産画像 */
      .worldheritage_img img{
        width: 5cm;
        height: auto;
      }
      
      /* ページネーション */
      .Pagination {
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .Pagination-Item-Link {
        width: 45px;
        height: 45px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: none;
        flex-wrap: wrap;
        overflow: hidden;
        background: #fff;
        border: solid 2px #111;
        font-size: 14px;
        color: #111;
        font-weight: bold;
        transition: all 0.15s linear;
      }

      .Pagination-Item-Link-Icon {
        width: 20px;
      }

      .Pagination-Item-Link.isActive {
        background: #111;
        color: #fff;
        pointer-events: none;
      }

      .Pagination-Item-Link:not(.isActive):hover {
        background: #111;
        color: #fff;
      }

      .Pagination > * + * {
        margin-left: 8px;
      }

    }

</style>