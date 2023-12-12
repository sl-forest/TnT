<template>

  <div>
    <TheHeader />

    <main>
      <h1>寺山炭窯跡</h1>
      <div class="WorldHeritage">

        <div class = WorldHeritage_img>
          <img src="~/assets/img/Sumigamaato.jpg" alt="寺山炭窯跡">
        </div>
        
        <div class = WorldHeritage_note>    
          
          <dl>
            <dt>営業時間</dt>
            <dd>見学自由</dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>無料</dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市吉野町10716-68</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>
                【車】鹿児島中央駅から45分
                <br>
                【バス】鹿児島中央駅から中別府団地線にて約40分
                <br>
                少年自然の家入口バス停下車徒歩約20分
            </dd>
          </dl>

          <dl>
            <dt>詳しくは</dt>
            <dd><a href="http://www.japansmeijiindustrialrevolution.com/site/kagoshima/component02.html" target="_blank">寺山炭窯後 ホームページ</a></dd>
          </dl>

        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
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
    text-decoration: none;
    width: 320px;
    margin: 24px auto;
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
/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  main {
    margin: 0 auto;
  }

  h1 {
    margin: 16px 0;
    text-align: center;
  }
  
  .WorldHeritage {
    padding-bottom: 16px;
  }

  .WorldHeritage h1 {
    margin: 1.6px auto;
  }

  .WorldHeritage_img {
    text-align: center;
  }

  .WorldHeritage_img img {
    height: 6cm;
  }

  .WorldHeritage_img p {
    margin: 0;
  }

  .WorldHeritage_note {
    margin-top: 16px;
  }

  .WorldHeritage_note h2 {
    margin: 8px auto;
  }

  .WorldHeritage_note dl {
    display: table;
    width: 100%;
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
    width: 20%;
  }

  .WorldHeritage_note dd {
    margin: 0px;
    padding: 2%;
    font-size: 15px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
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
    height: 8cm;
  }

  .WorldHeritage_img p {
    margin: 0;
  }

  .WorldHeritage_note {
    margin: auto;
    padding-left: 16px;
  }

  .WorldHeritage_note h2 {
    margin: 8px auto;
  }

  .WorldHeritage_note dl {
    font-size: 18px;
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
    width: 20%;
  }

  .WorldHeritage_note dd {
    width: 14cm;
    margin: 0px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>