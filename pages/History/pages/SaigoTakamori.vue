<template>

<div>
  <TheHeader />
  
  <main>
    <h1>西郷隆盛の年表</h1>
    <div class = "box">
      <ul class="timeline">
        <li>
          <p class="timeline-date">1827年（1歳）</p>
          <div class="timeline-content">
            <h3>鹿児島城下・下鍛冶屋しもかじや町に生まれる。(幼名、小吉)</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1844年（18歳）</p>
          <div class="timeline-content">
            <h3>藩に出仕し、郡方書役助こおりかたかきやくすけとなる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1850年（24歳）</p>
          <div class="timeline-content">
            <h3>島津斉彬しまづなりあきらに農政に関する意見書を提出する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1854年（28歳）</p>
          <div class="timeline-content">
            <h3>斉彬のお供として江戸へ向かう。庭方役にわかたやくに昇進する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1859年（33歳）</p>
          <div class="timeline-content">
            <h3>奄美大島で潜居生活を始める。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1862年（36歳）</p>
          <div class="timeline-content">
            <h3>鹿児島に帰国するも、再び流刑に。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1864年（38歳）</p>
          <div class="timeline-content">
            <h3>禁門の変で薩摩軍を指揮する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1866年（40歳）</p>
          <div class="timeline-content">
            <h3>薩長同盟を結ぶ。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1868年（42歳）</p>
          <div class="timeline-content">
            <h3>鳥羽伏見の戦い。江戸無血開城。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1871年（45歳）</p>
          <div class="timeline-content">
            <h3>新政府の参議となる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1873年（47歳）</p>
          <div class="timeline-content">
            <h3>征韓論騒動が起こり、敗れて鹿児島へ帰国する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1874年（48歳）</p>
          <div class="timeline-content">
            <h3>私学校を作る。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1877年（51歳）</p>
          <div class="timeline-content">
            <h3>西南戦争・城山にて自決する。</h3>
          </div>
        </li>
      </ul>
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

/* 年表 */
.timeline {margin: 0;}  /* 要素の外側余白 */

.timeline > li {
  overflow: hidden;   /* 要素からはみ出た部分を非表示 */
  margin: 0;          /* 要素の外側余白 */
  position: relative; /* 現在位置を基準に相対位置を指定 */
}

.timeline-date {
  width: 135px;       /* 横幅 */
  float: left;        /* 左から順に横並び */
  margin-top: 20px;   /* 要素の外側上余白 */
}

.timeline-content {
  width: 75%;                       /* 横幅 */
  float: left;                      /* 左から順に横並び */
  border-left: 3px #e5e5d1 solid; /* 下線 */
  padding-left: 30px;               /* 要素の内側左余白 */
}

/* timeline-content要素の後ろ */
.timeline-content:before {
  content: '';            /* 中点*/
  width: 12px;            /* 横幅 */
  height: 12px;           /* 高さ */
  background: #6fc173;  /* 背景 */
  position: absolute;     /* 親要素を基準に絶対配置を指定 */
  left: 130px;            /* 位置調整 */
  top: 24px;              /* 位置調整 */
  border-radius: 100%;
}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */

  h1 {
    padding: 8px 0;     /* 要素の内側余白 */
    text-align: center; /* 中央揃え */
  }

  .timeline {list-style: none;} /* 点削除 */

  .timeline li {margin-bottom: 40px;} /* 要素の外側下余白 */
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
}
</style>