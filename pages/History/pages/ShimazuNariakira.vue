<template>

<div>
  <TheHeader />

  <main>
    <h1>島津斉彬の年表</h1>
    <div class="box">
      <ul class="timeline">
        <li>
          <p class="timeline-date">1809年（1歳）</p>
          <div class="timeline-content">
            <h3>江戸の薩摩藩屋敷にて生まれる。（幼名 : 邦丸）</h3>
          </div>
        </li>
        
        <li>
          <p class="timeline-date">1825年（16歳）</p>
          <div class="timeline-content">
            <h3>初名であった忠方より斉彬と改名、「斉」は将軍「家斉」より一字を賜った。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1826年（17歳）</p>
          <div class="timeline-content">
            <h3>蘭癖大名として名高い曽祖父、島津重豪にシーボルトに引き合わされる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1849年（40歳）</p>
          <div class="timeline-content">
            <h3>薩摩藩主の父・斉興との対立が激化し、後継問題として「お油羅騒動」が起きる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1851年（42歳）</p>
          <div class="timeline-content">
            <h3>幕府の介入により斉興は隠居、島津斉彬が薩摩藩主となり、薩摩藩の近代化政策「集成館事業」を開始する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1853年（44歳）</p>
          <div class="timeline-content">
            <h3>ペリー来航、島津斉彬は幕府に大船建造の禁の解除を訴える。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1856年（47歳）</p>
          <div class="timeline-content">
            <h3>養女とした天璋院篤姫を江戸幕府13代将軍、徳川家定の正室に輿入れさせる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1858年（48歳）</p>
          <div class="timeline-content">
            <h3>将軍後継者問題で井伊直弼を中心とする幕府旧守派と対立する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1858年（48歳）</p>
          <div class="timeline-content">
            <h3>将軍後継問題で朝廷に圧力をかけるため京に兵を上げる直前8月24日に急死する。</h3>
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