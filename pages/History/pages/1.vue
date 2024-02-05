<template>

  <div>
    <TheHeader />

    <main>
      <h1>「偉人」</h1>
      <h2 class = history_headline>島津斉彬（しまづなりあきら）（1809-1858）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/shimadu-min.jpg" alt="島津斉彬">
        </div>

        <div class = explanation>
          <p>
            幕末の鹿児島藩主。<br>
            富国強兵策を推進。反射炉や機械制工業を他藩にさきがけて経営し、それらを一括して集成館を設立した。<br>
            また開国の意見を抱き西郷隆盛・大久保利通等の英才を抜擢し、明治維新の先駆をなした。<br>
            その卓越した識見は、松平春嶽より「英明近世の第一人者」と称された。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/History/pages/ShimazuNariakira">島津斉彬の年表はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = history_headline>西郷隆盛（さいごうたかもり）（1827-1877）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/segodon-min.jpeg" alt="西郷隆盛">
        </div>
        
        <div class = explanation>
          <p>
            西郷隆盛は幕末期の薩摩藩の武士。<br>
            故郷鹿児島の盟友・大久保利通と共に薩摩藩をリードして王政復古を実現させ、<br>
            徳川幕府を倒し、明治政府の成立に大きな貢献をした。<br>
            維新後、封建制度下の特権を失った不平士族（旧武士）の首領となって西南戦争を起こしたが政府軍に敗れ自刃した。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/History/pages/SaigoTakamori">西郷隆盛の年表はこちら</a>
          </div> 
        </div>
      </div>

      <h2 class = history_headline>大久保利通（おおくぼとしみち）（1830-1878）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/ookubo-min.jpg" alt="大久保利通">
        </div>

        <div class = explanation>
          <p>
            明治維新の指導者。島津久光のもとで公武合体運動を推進。<br>
            やがて討幕へと転じ、薩長連合を成立させる一方、岩倉具視らと結んで<br>
            慶応3(1867)年12月、王政復古のクーデターを敢行。<br>
            版籍奉還や廃藩置県を推進し、新政府の基礎を固める。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/History/pages/OkuboToshimichi">大久保利通の年表はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = history_headline>小松帯刀（こまつたてわき）（1835-1870）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/komatsu-min.jpg" alt="小松帯刀">
        </div>

        <div class = explanation>
          <p>
            島津久光の側近として大久保利通らの藩内下級武士を多く要職につかせ，<br>
            家老に進んだ後は大久保・西郷隆盛らとともに討幕派公卿・諸藩の間を奔走。<br>
            大政奉還に尽力。明治政府に重用され外国官（外務省の前身）副知事になったが病死。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/History/pages/KomatsuTatewaki">小松帯刀の年表はこちら</a>
          </div>
        </div>
      </div>

      <h2 class = history_headline_last>天璋院篤姫（てんしょういんあつひめ）（1836-1883）</h2>
      <div class="history">
        <div class = history_img>
          <img src="~/assets/img/Atsuhime-min.jpg" alt="天璋院篤姫">
        </div>

        <div class = explanation>
          <p>
            幕府の消滅に立会い、徳川本家廃絶・江戸城武力攻略の回避に力を尽くし、<br>
            明治期には徳川本家の家格・家名の維持を目ざした。
          </p>
          <div class="link-space">
            <a class ="btn" href="http://localhost:3000/History/pages/TenshoinAtsuhime">天璋院篤姫の年表はこちら</a>
          </div>
        </div>
      </div>
    
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}       /* 要素の外側余白 */
main {margin: 0 auto;}  /* 要素の外側余白 */

h1 {
  margin: 0;                          /* 要素の外側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

h2.history_headline {
  margin: 0;                       /* 要素の外側余白 */
  padding: 8px 0;                  /* 要素の内側余白 */
  border-top: 2px solid #d5d4c3; /* 上線 */
}

h2.history_headline_last {
  margin: 0;                       /* 要素の外側余白 */
  padding: 8px 0;                  /* 要素の内側余白 */
  border-top: 2px solid #d5d4c3; /* 上線 */
}

.explanation p {
  margin: 0;            /* 要素の外側余白 */
  font-family: serif;   /* フォントの変更 */
  font-weight: bold;    /* 文字の太さ */
  font-size: 15px;      /* 文字の大きさ */
}

/* ボタン */
.btn {
  display: inline-block;      /* インラインブロック要素へ変更 */
  padding: 0.3em 0.6em;       /* 要素の内側余白 */
  text-decoration: none;      /* 下線無効 */
  color: black;             /* 文字の色 */
  border: solid 2px black;  /* 枠線 */
  border-radius: 3px;         /* 要素の境界の外側の角を丸める */
  transition: .4s;            /* 要素の2つの状態間の変化を定義する */
}

/* マウスオーバー */
.btn:hover {
  background: black;  /* 背景 */
  color: white;       /* 文字の色 */
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */

  h1 {
    padding: 8px 0;     /* 要素の内側余白 */
    text-align: center; /* 中央揃え */
  }

  br {display: none;}             /* 表示しない */
  .history {text-align: center;} /* 中央揃え */

  h2.history_headline {
    text-align: center; /* 中央揃え */
    font-size: 28px;    /* 文字の大きさ */
  }

  h2.history_headline_last {
    text-align: center; /* 中央揃え */
    font-size: 25px;    /* 文字の大きさ */
  }

  .link-space {margin: 16px 0;} /* 要素の外側余白 */

  .explanation p {
    text-align: left; /* 左寄せ */
    margin-top: 16px; /* 要素の外側上余白 */
  }
  
/* 画像 */
  .history_img img {
    width: 320px; /* 横幅 */
    height: auto; /* 高さ */
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
/* 一覧説明 */
  .history {
    display: flex;        /* 親要素に対して子要素を横並び */
    margin-bottom: 16px;  /* 要素の外側下余白 */
    column-gap: 1rem;     /* 行や列の間のすき間を定義 */
  }

  .explanation {align-self: center;}  /* 中央揃え */
  .link-space {margin-top: 0.5rem;}   /* 要素の外側上余白 */

/* 画像 */
  .history_img img {
    width: 200px; /* 横幅 */
    height: auto; /* 高さ */
  }
}
</style>