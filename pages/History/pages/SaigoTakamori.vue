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

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;} /* 要素の外側上余白 */

  h1 {
    padding: 8px 0px;     /* 要素の内側余白 */
    text-align: center;   /* 左右の中央揃え */
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
  
  .timeline {list-style: none;}

  .timeline > li {margin-bottom: 40px;}
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */

  h1 {padding-top: 16px;}   /* 要素の内側上余白 */
  
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
}
</style>