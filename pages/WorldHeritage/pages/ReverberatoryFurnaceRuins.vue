<template>

  <div>
    <TheHeader />

    <main>
      <h1>旧集成館「反射炉跡」</h1>
      <div class="WorldHeritage">

        <div class = WorldHeritage_img>
          <img src="~/assets/img/Reverberatory furnace ruins.jpeg" alt="旧集成館「反射炉跡」">
        </div>
      
        <div class = WorldHeritage_note>    
        
          <dl>
            <dt>営業時間</dt>
            <dd>
              8:30～17:30（3/16～10/31）
              <br>
              8:30～17:20（11/1～3/15）
              </dd>
          </dl>

          <dl>
            <dt>休日</dt>
            <dd>年中無休</dd>
          </dl>

          <dl>
            <dt>料金</dt>
            <dd>
              大人:1,000円 
              <br>
              小人:500円（尚古集成館と共通）
              </dd>
          </dl>

          <dl>
            <dt>住所</dt>
            <dd>鹿児島県鹿児島市吉野町9700-1</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>
              【車】鹿児島中央駅から20分
              <br>
              【車】鹿児島空港から40分
              <br>
              【バス】鹿児島市周遊バスで仙巌園前（磯庭園前）下車徒歩1分。
            </dd>
          </dl>

          <dl>
          <dt>詳しくは</dt>
          <dd><a href="https://www.senganen.jp/" target="_blank">仙厳園 公式ホームページ</a></dd>
          </dl>

        </div>
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
  margin: 0;            /* 要素の外側余白 */
  padding: 8px 0;       /* 要素の内側余白 */
  font-family: 'New Tegomin', serif;  /* フォントの変更 */
}

.WorldHeritage_note dd a {
  text-decoration: none;
  color: blue;
}

/* マウスオーバー */
.WorldHeritage_note dd a:hover {color: rgb(71, 1, 92);}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}    /* 要素の外側上余白 */

  h1 {text-align: center;}   /* 左右の中央揃え */
  
  .WorldHeritage {padding-bottom: 16px;}

  .WorldHeritage_img {text-align: center;}

  .WorldHeritage_img img {width: 400px;}

  .WorldHeritage_note {margin-top: 16px;}

  .WorldHeritage_note h2 {margin: 8px auto;}

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
    margin: 0;
    padding: 2%;
    font-size: 16px;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;} /* 最大横幅 */
  
  .WorldHeritage {
    display: flex;
    padding-bottom: 24px;
  }

  .WorldHeritage_img {margin: auto;}

  .WorldHeritage_img img {width: 480px;}

  .WorldHeritage_note {
    margin: auto;
    padding-left: 16px;
  }

  .WorldHeritage_note h2 {margin: 8px auto;}

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
    margin: 0;
    display: flex;
    background-color: #fff;
    padding-left: 1%;
    flex-grow: 1;
  }
}
</style>