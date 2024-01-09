<template>

  <div>
    <TheHeader />

    <main>
      <h1>「偉人」</h1>
      <h2 class = history_headline>島津斉彬（しまづなりあきら）（1809-1858）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/shimadu.jpg" alt="島津斉彬">
        </div>

        <div class = explanation>
          <p>
            幕末の鹿児島藩主。<br>号は惟敬・麟洲、謚号を順聖院。斉興の子。
            藩政改革・富国強兵策を推進。<br>反射炉や機械制工業を他藩にさきがけて経営し、それらを一括して集成館を設立した。<br>
            また開国の意見を抱き西郷隆盛・大久保利通等の英才を抜擢し、明治維新の先駆をなした。<br>
            その卓越した識見は、松平春嶽より「英明近世の第一人者」と称された。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/History/pages/ShimazuNariakira" target="_blank"><b>年表はこちら</b></a>
        </div>
      </div>

      <h2 class = history_headline>西郷隆盛（さいごうたかもり）（1827-1877）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/segodon.jpeg" alt="西郷隆盛">
        </div>
        
        <div class = explanation>
          <p>
            西郷隆盛は幕末期の薩摩藩の武士。<br>
            故郷鹿児島の盟友・大久保利通と共に薩摩藩をリードして王政復古を実現させ、<br>徳川幕府を倒し、明治政府の成立に大きな貢献をした。<br>
            維新後、封建制度下の特権を失った不平士族（旧武士）の首領となって西南戦争を起こしたが政府軍に敗れ自刃した。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/History/pages/SaigoTakamori" target="_blank"><b>年表はこちら</b></a>
        </div> 
      </div>

      <h2 class = history_headline>大久保利通（おおくぼとしみち）（1830-1878）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/ookubo.jpg" alt="大久保利通">
        </div>

        <div class = explanation>
          <p>
            明治維新の指導者。
            島津久光のもとで公武合体運動を推進。
            やがて討幕へと転じ、薩長連合を成立させる一方、岩倉具視らと結んで慶応3(1867)年12月、王政復古のクーデターを敢行。<br>
            版籍奉還や廃藩置県を推進し、新政府の基礎を固める。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/History/pages/OkuboToshimichi" target="_blank"><b>年表はこちら</b></a>
        </div>
      </div>

      <h2 class = history_headline>小松帯刀（こまつたてわき）（1835-1870）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/komatsu.jpg" alt="小松帯刀">
        </div>

        <div class = explanation>
          <p>
            島津久光の側近として大久保利通らの藩内下級武士を多く要職につかせ，
            家老に進んだ後は<br>大久保・西郷隆盛らとともに討幕派公卿・諸藩の間を奔走。
            大政奉還に尽力。<br>
            明治政府に重用され外国官（外務省の前身）副知事になったが病死。
          </p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/History/pages/KomatsuTatewaki" target="_blank"><b>年表はこちら</b></a>
        </div>
      </div>

      <h2 class = history_headline_last>天璋院篤姫（てんしょういんあつひめ）（1836-1883）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/Atsuhime.jpg" alt="天璋院篤姫">
        </div>

        <div class = explanation>
          <p>幕府の消滅に立会い、徳川本家廃絶・江戸城武力攻略の回避に力を尽くし、明治期には<br>徳川本家の家格・家名の維持を目ざした。</p>
        </div>
        <div class="link-space">
          <a class ="explanation-link" href="http://localhost:3000/History/pages/TenshoinAtsuhime" target="_blank"><b>年表はこちら</b></a>
        </div>
      </div>
    
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
h1 {font-family: 'New Tegomin', serif;}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {margin: 0 auto;}

  h1 {
    margin: 8px;
    text-align: center;
    margin-bottom: 0;
  }

  br {display: none;}

  .history {text-align: center;}

  h2.history_headline {
    margin: 0;
    text-align: center;
    font-size: 28px;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  h2.history_headline_last {
    margin: 0;
    text-align: center;
    font-size: 25px;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  .link-space {margin: 8px 0;}

  .explanation p {
    font-size: 15px;
    text-align: left; /* 左寄せ */
    margin-top: 16px;
    margin-bottom: 0;
  }
  
  .explanation-link {
    text-decoration: none;
    color: blue;
  }
  
/* 工芸品画像 */
  .history_img img {
    width: 8cm;
    height: auto;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }
  
  h1 {margin-bottom: 0;}
  
/* 工芸品一覧説明 */
  .history {
    display: flex;
    margin-bottom: 16px;
  }

  .history p {
    margin: 0;
    font-size: 15px;
  }

  h2.history_headline {
    margin: 0;
    padding: 8px 0;
    border-top: 2px solid #d5d4c3;
  }

  h2.history_headline_last {
    margin: 0;
    padding-top: 8px;
    border-top: 2px solid #d5d4c3;
  }

  .explanation {
    margin: auto;
    width: 17cm;
  }

  .link-space {align-self: end;}

  .link-space a {
    margin: 0;
    font-size: 14px;
  }
  
  .explanation-link {
    text-decoration: none;
    color: blue;
    display: flex;
    align-items: flex-end;
  }

  a:hover.explanation-link {color: rgb(71, 1, 92);}

/* 工芸品画像 */
  .history_img img{
    width: 5cm;
    height: auto;
  }

/* 提供 */
  .teikyou p {font-size: 13px;}
}
</style>