<template>

<div>
  <TheHeader />
  
  <main>
    <h1>天璋院篤姫の年表</h1>
      <div class="box">
        <ul class="timeline">
          <li>
            <p class="timeline-date">1836年（0歳）</p>
            <div class="timeline-content">
              <h3>篤姫生まれる</h3>
            </div>
          </li>

          <li>
            <p class="timeline-date">1853年（17歳）</p>
            <div class="timeline-content">
              <h3>篤姫が島津斉彬なりあきらの養女となる</h3>
            </div>
          </li>

          <li>
            <p class="timeline-date">1856年（20歳）</p>
            <div class="timeline-content">
              <h3>篤姫が徳川家定の御台所（みだいどころ。正妻）となる</h3>
            </div>
          </li>

          <li>
            <p class="timeline-date">1858年（22歳）</p>
            <div class="timeline-content">
              <h3>徳川家定、島津斉彬、あいついで亡くなる</h3>
            </div>
          </li>

          <li>
            <p class="timeline-date">1867年（31歳）</p>
            <div class="timeline-content">
              <h3>大政奉還。江戸城無血開城</h3>
            </div>
          </li>

          <li>
            <p class="timeline-date">1883年（47歳）</p>
            <div class="timeline-content">
              <h3>篤姫亡くなる</h3>
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