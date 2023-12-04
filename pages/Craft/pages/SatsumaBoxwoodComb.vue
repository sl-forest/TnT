<template>

   <div>
    <TheHeader />

    <main>
      <h1>薩摩つげ櫛</h1>
        <div class="Craft">
            
            <div class = Craft_img>
                <img src="~/assets/img/Tugegushi.jpg" alt="薩摩つげ櫛">
            </div>

            <div class = Craft_note>

              <dl>
                <dt>読み</dt>
                <dd>さつまつげくし
                </dd>
              </dl>
              
              <dl>
                <dt>工芸品の分類</dt>
                <dd>木工品</dd>
              </dl>

              <dl>
                <dt>主な製品</dt>
                <dd>櫛</dd>
              </dl>

              <dl>
                <dt>主要製造地域</dt>
                <dd>薩摩地方</dd>
              </dl>

              <dl>
                <dt>指定年月日</dt>
                <dd>平成6年（1994年）3月14日</dd>
              </dl>

              <dl>
                <dt>詳しくは</dt>
                <dd><a href="http://kushi.jp/" target="_blank">喜多つげ製作所</a></dd>
              </dl>

            </div>

        </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  h1 {
    text-align: center;
    margin: 12px 0;
  }

  .Craft_img {
    text-align: center;
    margin-bottom: 24px;
  }

  .Craft_img img {
    width: 72%;
  }

  .Craft_note {
    margin-bottom: 24px;
  }

  .Craft_note dl {
    font-size: 16px;
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
    width: 30%;
  }

  .Craft_note dd {
    width: 12cm;
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

  .Craft_img img {
    height: 9.5cm;
  }

  .Craft_img p {
    margin: 0;
  }

  .Craft_note {
    margin-top: 0.6cm;
    padding-left: 16px;
  }

  .Craft_note h2 {
    margin: 8px auto;
  }

  .Craft_note dl {
    font-size: 16px;
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
    width: 28%;
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
}
</style>
