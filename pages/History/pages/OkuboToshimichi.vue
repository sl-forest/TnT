<template>

<div>
  <TheHeader />
  
  <main>
    <h1>年表</h1>
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