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
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {
    max-width: 1024px;
    margin: 0 auto;
  }

  h1 {
    text-align: center;
    margin-top: 16px;
    margin-bottom: 0;
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
  main {
    max-width: 1024px;
    margin: 0 auto;
  }

  h1 {
    margin-top: 16px;
    margin-bottom: 0;
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
}
</style>