<template>

<div>
  <TheHeader />
  
  <main>
    <h1>小松帯刀の年表</h1>
    <div class = "box">
      <ul class="timeline">
        <li>
          <p class="timeline-date">1835年（1歳）</p>
          <div class="timeline-content">
            <h3>薩摩国鹿児島城下山下町（現・鹿児島市山下町）にて、喜入きいれ領主・肝付兼善きもつきかねよしの三男として生まれる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1848年（13歳）</p>
          <div class="timeline-content">
            <h3>（～1855年（21歳）まで）藩校・造士館にて学んだほか、漢学者・横山安容よこやまあんようから儒学、国学者・八田知紀（はったともき）から歌道を学ぶ。西郷隆盛・大久保利通らからなる精忠組とも交流。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1855年（21歳）</p>
          <div class="timeline-content">
            <h3>奥小姓おくごしょう・近習番勤きんじゅばんづとめとして薩摩藩・江戸藩邸に出仕。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1856年（22歳）</p>
          <div class="timeline-content">
            <h3>吉利よしとし領主・小松清猷きよなおが急死。小松家存続のため清猷の妹・千賀ちかの婿となり、吉利領主となる</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1858年（24歳）</p>
          <div class="timeline-content">
            <h3>薩摩藩の当番頭・奏者番そうじゃばんとして藩主・島津忠義に仕える。造船などを行う集成館の管理・貨幣鍛造などを職務とした。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1861年（27歳）</p>
          <div class="timeline-content">
            <h3>長崎出張を命じられ、オランダ軍艦にて軍艦操作・電気・水雷などの研修を受ける。その実演にて手腕を認められ、藩の実験を握っていた島津久光の側近となる。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1862年（28歳）</p>
          <div class="timeline-content">
            <h3>久光の上洛に随行し、朝廷との交渉役を務める。帰国後、薩摩藩家老に就任。薩英戦争にて指揮を執り、イギリス艦隊を退ける。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1864年（30歳）</p>
          <div class="timeline-content">
            <h3>「禁門の変」にて、西郷隆盛らと共に御所の守備を務め、朝廷からの信頼を得る。第一次長州征討に出兵。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1866年（32歳）</p>
          <div class="timeline-content">
            <h3>坂本龍馬、中岡慎太郎らの仲介にて、長州藩の木戸孝允たかよし、井上馨かおるらと交渉。京都の小松邸にて薩長同盟が成立する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1867年（33歳）</p>
          <div class="timeline-content">
            <h3>土佐藩と薩土同盟を成立させる。大和交易株式会社の設立、イギリス留学生の送り出しなど、外交にも力を注いだ。薩摩藩代表として将軍・徳川慶喜の大政奉還に立ち会う。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1868年（34歳）</p>
          <div class="timeline-content">
            <h3>明治政府が成立。以降、総裁局顧問・参与・外国事務掛などの要職を歴任する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1969年（35歳）</p>
          <div class="timeline-content">
            <h3>大久保利通らと版籍奉還を画策。反発を招くも自ら自領を返還し、島津久光を説得する。</h3>
          </div>
        </li>

        <li>
          <p class="timeline-date">1970年（36歳）</p>
          <div class="timeline-content">
            <h3>肺病や下腹部の腫瘍などを患い、オランダ人医師アントニウス・ボードウィンの治療を受ける。7月20日、大阪の借家にて病没。</h3>
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