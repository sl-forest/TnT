<template>

   <div>
    <TheHeader />

    <main>
      <h1>薩摩焼</h1>
        <div class="Craft">
            
            <div class = Craft_img>
                <img src="~/assets/img/SatsumaYaki.jpg" alt="薩摩焼">
            </div>

            <div class = Craft_note>

              <dl>
                <dt>読み</dt>
                <dd>さつまやき</dd>
              </dl>
              
              <dl>
                <dt>工芸品の分類</dt>
                <dd>陶磁器</dd>
              </dl>

              <dl>
                <dt>主な製品</dt>
                <dd>食器、茶器、花器、酒器、装飾品</dd>
              </dl>

              <dl>
                <dt>主要製造地域</dt>
                <dd>鹿児島市、指宿市、日置市</dd>
              </dl>

              <dl>
                <dt>系統</dt>
                <dd>
                    ・苗代川なおしろがわ系
                    <br>
                    ・竪野たての系
                    <br>
                    ・龍門司りゅうもんじ系
                    <br>
                    ・西餅田にしもちだ系
                    <br>
                    ・平佐ひらさ系
                </dd>
              </dl>

              <dl>
                <dt>指定年月日</dt>
                <dd>平成14年（2002年）1月30日</dd>
              </dl>

              <dl>
                <dt>詳しくは</dt>
                <dd><a href="https://www.kawanabe-butudan.or.jp/" target=”_blank”>鹿児島県川辺仏壇協同組合</a></dd>
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
      .Craft_note > dd {
        border: 1px solid #ddd;
        border-top: none;
      }

      .Craft_note > dt,
      .Craft_note > dd {
        text-align: center;
      }

      .Craft_note > dd > ul {
        text-align: left;
      }
}
    /* PC向けスタイル */
    @media screen and (min-width: 1024px) {
      main {
        max-width: 1024px;
        margin: 0 auto;
      }

      .Craft {
        display: flex;
        padding-bottom: 24px;
      }

      .Craft h1 {
        margin: 1.6px auto;
      }

      .Craft_img img {
        height: 9.5cm;
      }

      .Craft_img p {
        margin: 0;
      }

      .Craft_note {
        margin-top: 0.5cm;
        padding-left: 16px;
      }

      .Craft_note h2 {
        margin: 8px auto;
      }

      .Craft_note dl {
        font-size: 18px;
        margin: 3px 0;
        overflow: hidden;
        display: flex;
        align-items: center;
        background-color: #e0e2e2;
      }

      .Craft_note dt {
        vertical-align: middle;
        flex-shrink: 0;
        text-align: center;
        width: 25%;
      }

      .Craft_note dd {
        width: 15cm;
        margin: 0px;
        display: flex;
        background-color: #fff;
        padding-left: 1%;
        flex-grow: 1;
      }

      .Craft_note dd a {
        text-decoration: none;
        color: blue;
      }

      .Craft_note dd a:hover {
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
