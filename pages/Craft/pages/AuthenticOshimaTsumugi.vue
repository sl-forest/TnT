<template>

   <div>
    <TheHeader />

    <main>
      <h1>本場大島紬</h1>
        <div class="WorldHeritage">
            
            <div class = WorldHeritage_img>
                <img src="~/assets/img/OshimaTsumugi.jpg" alt="本場大島紬">
            </div>

            <div class = WorldHeritage_note>

              <dl>
                <dt>読み</dt>
                <dd>ほんばおおしまつむぎ</dd>
              </dl>
              
              <dl>
                <dt>工芸品の分類</dt>
                <dd>織物</dd>
              </dl>

              <dl>
                <dt>定義</dt>
                <dd>・絹100%
                    <br>
                    ・先染め手織り
                    <br>
                    ・平織り
                    <br>
                    ・締機しめばたで手作業により、経緯絣たてよこかすりおよび緯絣よこかすりを加工したもの
                    <br>
                    ・手機てばたで、経緯絣および緯絣を絣合わせをして織上げたもの
                </dd>
              </dl>

              <dl>
                <dt>指定年月日</dt>
                <dd>昭和50年（1975年）2月17日</dd>
              </dl>

              <dl>
                <dt>詳しくは</dt>
                <dd><a href="https://oshimatsumugi.com/tsumugi/" target=”_blank”>本場大島紬織物協同組合</a></dd>
              </dl>

              <dl>
                <dt>大島紬体験について</dt>
                <dd><a href="https://www.tumugi.co.jp/" target=”_blank”>大島紬村 公式ホームページ</a></dd>
              </dl>

            </div>

        </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
    /* スマホ向けスタイル */
    @media screen and (max-width: 767px) {
      .WorldHeritage_note > dd {
        border: 1px solid #ddd;
        border-top: none;
      }

      .WorldHeritage_note > dt,
      .WorldHeritage_note > dd {
        text-align: center;
      }

      .WorldHeritage_note > dd > ul {
        text-align: left;
      }
}
    /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
      main {
        max-width: 1024px;
        margin: 0 auto;
      }

      .WorldHeritage {
        display: flex;
        padding-bottom: 24px;
      }

      .WorldHeritage h1 {
        margin: 1.6px auto;
      }

      .WorldHeritage_img img {
        height: 9.5cm;
      }

      .WorldHeritage_img p {
        margin: 0;
      }

      .WorldHeritage_note {
        margin-top: 0.6cm;
        padding-left: 16px;
      }

      .WorldHeritage_note h2 {
        margin: 8px auto;
      }

      .WorldHeritage_note dl {
        font-size: 16px;
        margin: 3px 0;
        overflow: hidden;
        display: flex;
        align-items: center;
        background-color: #e0e2e2;
      }

      .WorldHeritage_note dt {
        vertical-align: middle;
        flex-shrink: 0;
        text-align: center;
        width: 28%;
      }

      .WorldHeritage_note dd {
        width: 15cm;
        margin: 0px;
        display: flex;
        background-color: #fff;
        padding-left: 1%;
        flex-grow: 1;
      }

      .WorldHeritage_note dd a {
        text-decoration: none;
        color: blue;
      }

      .WorldHeritage_note dd a:hover {
        color: rgb(71, 1, 92);
      }
   
    /* ボタン */
      a.btn {
        display: block;
        text-align: center;
        vertical-align: middle;
        text-decoration: none;
        width: 320px;
        margin-top: 18px;
        margin-left: 65px;
        padding: 1rem 4rem;
        font-weight: bold;
        border: 2px solid #27acd9;
        background: #27acd9;
        color: #fff;
        border-radius: 100vh;
        transition: 0.5s;
      }
      
      a.btn:hover {
        color: #27acd9;
        background: #fff;
      }
}

</style>
