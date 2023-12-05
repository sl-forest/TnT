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
  
  .timeline {
    list-style: none;
  }
  
  .timeline > li {
    margin-bottom: 40px;
  }
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