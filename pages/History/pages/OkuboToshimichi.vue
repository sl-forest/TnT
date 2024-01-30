<template>

<div>
  <TheHeader />
  
  <main>
    <h1>大久保利通の年表</h1>
    <div class = "box">
      <ul class="timeline">
        <li>
          <p class="timeline-date">1830年（1歳）</p>
          <div class="timeline-content">
            <h3>鹿児島城下の高麗町に生まれる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1846年（18歳）</p>
          <div class="timeline-content">
            <h3>薩摩藩の記録所書役となる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1850年（22歳）</p>
          <div class="timeline-content">
            <h3>お由羅騒動で免職・謹慎の処分を受ける。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1853年（25歳）</p>
          <div class="timeline-content">
            <h3>謹慎を解かれる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1866年（38歳）</p>
          <div class="timeline-content">
            <h3>第二次長州征討の出兵拒否。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1869年（41歳）</p>
          <div class="timeline-content">
            <h3>明治政府の参議に就任。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1871年（43歳）</p>
          <div class="timeline-content">
            <h3>岩倉使節団の一員として、欧米12カ国を歴訪。大蔵卿に就任。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1873年（45歳）</p>
          <div class="timeline-content">
            <h3>帰国。征韓論で西郷らと対立。内務卿に就任。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1877年（48歳）</p>
          <div class="timeline-content">
            <h3>西南戦争の指揮を執る。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1878年（49歳）</p>
          <div class="timeline-content">
            <h3>紀尾井坂で襲撃され、死亡。</h3>
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