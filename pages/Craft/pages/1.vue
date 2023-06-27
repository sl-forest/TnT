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
            <li><a class="item-link" href="http://localhost:3000">歴史</a></li>
            <li><a class="item-link" href="http://localhost:3000">郷土料理</a></li>
            <li><a class="item-link" href="http://localhost:3000">伝統芸能</a></li>
            <li><a class="item-link" href="http://localhost:3000">年間行事</a></li>
            <li><a class="item-link" href="http://localhost:3000">観光地</a></li>
            <li><a class="item-link" href="http://localhost:3000">世界遺産</a></li>
          </ul>
        </div>
      </nav>
    </header>

    <main>
        <h1>「伝統工芸品」</h1>
        <h2 class = craft_headline>本場大島紬</h2>
        <div class="craft">
            <div class = craft01_img>
                <img src="~/assets/img/OshimaTsumugi.jpg" alt="本場大島紬">
            </div>
            
            <div class = explanation>
                <p>1,300年の歴史を持ち、
                  絹織物の最高傑作といわれています。
                  30数工程もある緻密な手作業により、
                  図案から織り上がるまで半年から1年以上もかかります。
                  大島紬独自の技法「テーチ木泥染」は、
                  7世紀中頃から行われていた古代染色の技法を取り入れたものです。
                  緻密な絣模様や、軽くて暖かく、しなやかで着くずれしないなどの
                  優れた特徴があり、女性の着物として高い人気があります。
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>川辺仏壇</h2>
        <div class="craft">
            <div class = craft01_img>
                <img src="" alt="川辺仏壇">
            </div>

            <div class = explanation>
                <p>川辺仏壇（かわなべぶつだん）は、
                  鹿児島県南九州市川辺町周辺で作られている仏壇です。
                  川辺仏壇の特徴は、「ガマ戸」と呼ばれる川辺仏壇オリジナルの独特な仏壇があることです。
                  ”ガマ”とは、鹿児島県の方言で洞窟を表します。
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>薩摩焼</h2>
        <div class="craft">
            <div class = craft03_img>
                <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
            </div>

            <div class = explanation>
                <p>薩摩焼（さつまやき）は、鹿児島県内で焼かれる陶磁器です。</p>
                <p>主な窯場は姶良市の龍門司窯、日置市の苗代川窯、鹿児島市の長太郎窯などです。</p>
                <p>鉄分が多い土を高温で焼き締めるため、素朴で頑丈な仕上がりが特徴です。</p>
                <p>「白もん」と呼ばれる豪華絢爛な色絵錦手の陶器と「黒もん」と呼ばれる大衆向けの雑器に分かれるています。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>屋久杉</h2>
        <div class="craft">
            <div class = craft04_img>
                <img src="" alt="屋久杉">
            </div>

            <div class = explanation>
                <p>世界自然遺産に登録されている「屋久島」は1,000メートル以上の高峰が連なっており、
                  この大自然の中で育った樹齢1,000年以上のものを「屋久杉」と呼んでいます。
                  縄文の太古より風雨に耐え抜いてきた生命力あふれる屋久杉は、木目の美しさ、色、かおりの良さなど、
                  まさに銘木というにふさわしく、家具やインテリア用品などに幅広く活用されています。
                </p>
                <p>現在は自然保護のため、倒木や土埋木だけを工芸品として加工しています。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = craft_headline>薩摩つげ櫛</h2>
        <div class="craft">
            <div class = craft05_img>
                <img src="" alt="薩摩つげ櫛">
            </div>

            <div class = explanation>
                <p>薩摩つげ櫛は江戸時代から「櫛になりたや薩摩の櫛に、
                  諸国娘の手に渡ろ」とうたわれ、全国に名を馳せていました。
                  薩摩づけは材質が硬く、また、色艶が美しいのが特徴で、なによりも櫛の歯が折れにくく、
                  なめらかな櫛どおりで、静電気・抜け毛・切れ毛が少ないといわれています。
                </p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <!-- 検索ボックス -->
        <form id="form1" action="http://localhost:3000/">
        <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
        <input id="sbtn" type="submit" value="検索" />
        </form>
        
        <ul class="Pagination">
          <li class="Pagination-Item">
            <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/1">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
            </svg>
            </a>
            </li>

              <li class="Pagination-Item">
                <a class="Pagination-Item-Link isActive" href="http://localhost:3000/Craft/pages/1"><span>1</span></a>
              </li>
              
              <li class="Pagination-Item">
                <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/2"><span>2</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/3"><span>3</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/4"><span>4</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/5"><span>5</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/Craft/pages/5">
                      <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                          <path stroke-linecap="round" stroke-linejoin="round" d="M13 5l7 7-7 7M5 5l7 7-7 7" />
                      </svg>
                      </a>
                  </li>
              </ul>
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

      h2.craft_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 工芸品一覧説明 */
      .craft {
        display: flex;
      }

      .craft p {
        margin: 0;
      }

      .explanation {
        margin: auto;
        width: 40em;
      }
      
      .explanation-link {
        align-self: end;
      }

      /* 工芸品画像 */
      .craft01_img img{
        width: 5cm;
        height: auto;
      }

      .craft03_img img{
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