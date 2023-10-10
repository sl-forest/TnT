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
        <h1>「偉人」</h1>
        <h2 class = history_headline>島津斉彬（しまづなりあきら）（1809-1858）</h2>
        <div class="history">
            <div class = history01_img>
                <img src="~/assets/img/shimadu.jpg" alt="島津斉彬">
            </div>

            <div class = explanation>
                <div>
                  幕末の鹿児島藩主。号は惟敬・麟洲、謚号を順聖院。斉興の子。
                  藩政改革・富国強兵策を推進。反射炉や機械制工業を他藩にさきがけて経営し、それらを一括して集成館を設立した。
                  また開国の意見を抱き西郷隆盛・大久保利通等の英才を抜擢し、明治維新の先駆をなした。
                  その卓越した識見は、松平春嶽より「英明近世の第一人者」と称された。
                </div>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = history_headline>西郷隆盛（さいごうたかもり）（1827-1877）</h2>
        <div class="history">
            <div class = history01_img>
                <img src="~/assets/img/segodon.jpeg" alt="西郷隆盛">
            </div>
            
            <div class = explanation>
                <p>西郷隆盛は幕末期の薩摩藩の武士。</p>
                <p>故郷鹿児島の盟友・大久保利通と共に薩摩藩をリードして王政復古を実現させ、徳川幕府を倒し、明治政府の成立に大きな貢献をした。</p>
                <p>維新後、封建制度下の特権を失った不平士族（旧武士）の首領となって西南戦争を起こしたが政府軍に敗れ自刃した。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = history_headline>大久保利通（おおくぼとしみち）（1830-1878）</h2>
        <div class="history">
            <div class = history01_img>
                <img src="~/assets/img/ookubo.jpg" alt="大久保利通">
            </div>

            <div class = explanation>
                <p>明治維新の指導者。</p> 
                <p>島津久光のもとで公武合体運動を推進。</p>
                <p>やがて討幕へと転じ、薩長連合を成立させる一方、岩倉具視らと結んで慶応3(1867)年12月、王政復古のクーデターを敢行。</p>
                <p>版籍奉還や廃藩置県を推進し、新政府の基礎を固める。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = history_headline>小松帯刀（こまつたてわき）（1835-1870）</h2>
        <div class="history">
            <div class = history01_img>
                <img src="~/assets/img/komatsu.jpg" alt="小松帯刀">
            </div>

            <div class = explanation>
                <p>島津久光の側近として大久保利通らの藩内下級武士を多く要職につかせ，</p>
                <p>家老に進んだ後は大久保・西郷隆盛らとともに討幕派公卿・諸藩の間を奔走。</p>
                <p>大政奉還に尽力。明治政府に重用され外国官（外務省の前身）副知事になったが病死。</p>
            </div>
            <a class ="explanation-link" href="#">詳細はこちら</a>
        </div>

        <h2 class = history_headline>天璋院篤姫</h2>
        <div class="history">
            <div class = history01_img>
                <img src="~/assets/img/Atsuhime.jpg" alt="天璋院篤姫">
            </div>

            <div class = explanation>
                <p>幕府の消滅に立会い、徳川本家廃絶・江戸城武力攻略の回避に力を尽くし、明治期には徳川本家の家格・家名の維持を目ざした。</p>
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
            <a class="Pagination-Item-Link" href="http://localhost:3000//History/pages/1">
            <svg xmlns="http://www.w3.org/2000/svg" class="Pagination-Item-Link-Icon" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M11 19l-7-7 7-7m8 14l-7-7 7-7" />
            </svg>
            </a>
            </li>

              <li class="Pagination-Item">
                <a class="Pagination-Item-Link isActive" href="http://localhost:3000/History/pages/1"><span>1</span></a>
              </li>
              
              <li class="Pagination-Item">
                <a class="Pagination-Item-Link" href="http://localhost:3000/History/pages/2"><span>2</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/History/pages/3"><span>3</span></a>
              </li>

              <li class="Pagination-Item">
                  <a class="Pagination-Item-Link" href="http://localhost:3000/History/pages/3">
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

      h2.history_headline {
        margin: 0;
        padding-top: 8px;
        border-top: 2px solid #d5d4c3;
      }
      
      /* 歴史一覧説明 */
      .history {
        display: flex;
      }

      .history p {
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
      .history01_img img{
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