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
        
        <h1>年表</h1>

        <div class = "box">
          <ul class="timeline">
            <li>
              <p class="timeline-date">1835年（1歳）</p>
                <div class="timeline-content">
                  <h3>薩摩国鹿児島城下山下町（現・鹿児島市山下町）にて、喜入きいれ領主・肝付兼善きもつきかねよしの三男として生まれる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1848年（13歳）</p>
                <div class="timeline-content">
                  <h3>（～1855年（21歳）まで）藩校・造士館にて学んだほか、漢学者・横山安容よこやまあんようから儒学、国学者・八田知紀はったともきから歌道を学ぶ。西郷隆盛・大久保利通らからなる精忠組とも交流。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1855年（21歳）</p>
                <div class="timeline-content">
                  <h3>奥小姓おくごしょう・近習番勤きんじゅばんづとめとして薩摩藩・江戸藩邸に出仕。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1856年（22歳）</p>
                <div class="timeline-content">
                  <h3>吉利よしとし領主・小松清猷きよなおが急死。小松家存続のため清猷の妹・千賀ちかの婿となり、吉利領主となる</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1858年（24歳）</p>
                <div class="timeline-content">
                  <h3>薩摩藩の当番頭・奏者番そうじゃばんとして藩主・島津忠義に仕える。造船などを行う集成館の管理・貨幣鍛造などを職務とした。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1861年（27歳）</p>
                <div class="timeline-content">
                  <h3>長崎出張を命じられ、オランダ軍艦にて軍艦操作・電気・水雷などの研修を受ける。その実演にて手腕を認められ、藩の実験を握っていた島津久光の側近となる。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1862年（28歳）</p>
                <div class="timeline-content">
                  <h3>久光の上洛に随行し、朝廷との交渉役を務める。帰国後、薩摩藩家老に就任。薩英戦争にて指揮を執り、イギリス艦隊を退ける。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1864年（30歳）</p>
                <div class="timeline-content">
                  <h3>「禁門の変」にて、西郷隆盛らと共に御所の守備を務め、朝廷からの信頼を得る。第一次長州征討に出兵。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1866年（32歳）</p>
                <div class="timeline-content">
                  <h3>坂本龍馬、中岡慎太郎らの仲介にて、長州藩の木戸孝允たかよし、井上馨かおるらと交渉。京都の小松邸にて薩長同盟が成立する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1867年（33歳）</p>
                <div class="timeline-content">
                  <h3>土佐藩と薩土同盟を成立させる。大和交易株式会社の設立、イギリス留学生の送り出しなど、外交にも力を注いだ。薩摩藩代表として将軍・徳川慶喜の大政奉還に立ち会う。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1868年（34歳）</p>
                <div class="timeline-content">
                  <h3>明治政府が成立。以降、総裁局顧問・参与・外国事務掛などの要職を歴任する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1969年（35歳）</p>
                <div class="timeline-content">
                  <h3>大久保利通らと版籍奉還を画策。反発を招くも自ら自領を返還し、島津久光を説得する。</h3>
                </div>
            </li>

            <li>
                <p class="timeline-date">1970年（36歳）</p>
                <div class="timeline-content">
                  <h3>肺病や下腹部の腫瘍などを患い、オランダ人医師アントニウス・ボードウィンの治療を受ける。7月20日、大阪の借家にて病没。</h3>
                </div>
            </li>
          </ul>
        </div>

        <!-- 検索ボックス -->
        <form id="form1" action="http://localhost:3000/">
        <input id="sbox" name="s" type="text" placeholder="キーワードを入力" />
        <input id="sbtn" type="submit" value="検索" />
        </form>

    </main>
</div>

</template>

<style>
    /* スマホ向けスタイル */
    .timeline {
        list-style: none;
      }
      
      .timeline > li {
        margin-bottom: 60px;
      }

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
      
    /* 年表 */
      .timeline > li {
        overflow: hidden;
        margin: 0;
        position: relative;
      }
      
      .timeline-date {
        width: 135px;
        float: left;
        margin-top: 20px;
      }
      
      .timeline-content {
        width: 75%;
        float: left;
        border-left: 3px #e5e5d1 solid;
        padding-left: 30px;
      }
      
      .timeline-content:before {
        content: '';
        width: 12px;
        height: 12px;
        background: #6fc173;
        position: absolute;
        left: 130px;
        top: 24px;
        border-radius: 100%;
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
    }

</style>