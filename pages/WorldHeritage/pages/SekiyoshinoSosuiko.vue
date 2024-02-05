<template>

  <div>
    <TheHeader />

    <main>
      <h1>関吉の疎水溝</h1>
      <div class="WorldHeritage">

        <div class = WorldHeritage_img>
          <img src="~/assets/img/Sekiyoshi-min.jpg" alt="関吉の疎水溝">
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
            <dd>鹿児島県鹿児島市下田町</dd>
          </dl>

          <dl>
            <dt>移動方法</dt>
            <dd>【車】鹿児島中央駅から30分
                <br>
                【バス】鹿児島中央駅から30分（バス下車後徒歩8分）
            </dd>
          </dl>

          <dl>
            <dt>詳しくは</dt>
            <dd><a href="https://www.kagoshima-kankou.com/industrial-heritage/52606" target="_blank">鹿児島の旅 関吉の疎水溝</a></dd>
          </dl>

        </div>

      </div>
    </main>
    <TheFooter />
  </div>

</template>

<style>
/* 共通 */
body {margin: 0;}
main {margin: 0 auto;}

h1 {
  margin: 0;
  padding: 8px 0;
  font-family: 'New Tegomin', serif;
}

.WorldHeritage_note dl {
  margin: 3px 0;
  overflow: hidden;
  display: flex;
  align-items: center;
  background-color: #e0e2e2;
}

.WorldHeritage_note dt {
  flex-shrink: 0;
  text-align: center;
}

.WorldHeritage_note dd {
  margin: 0;
  display: flex;
  background-color: #fff;
  padding-left: 1%;
  flex-grow: 1;
}

.WorldHeritage_note dd a {
  text-decoration: none;
  color: blue;
}

/* マウスオーバー */
.WorldHeritage_note dd a:hover {color: rgb(71, 1, 92);}

/* スマホ向けスタイル */
@media screen and (max-width: 480px) {
  body {margin-top: 18%;}

  h1 {
    text-align: center;
    font-size: 30px;
  }
  
  .WorldHeritage {padding-bottom: 16px;}
  .WorldHeritage_img {text-align: center;}

  .WorldHeritage_img img {
    width: 400px;
    height: auto;
  }

  .WorldHeritage_note {margin-top: 16px;}
  .WorldHeritage_note h2 {margin: 8px auto;}
  .WorldHeritage_note dl {font-size: 16px;}
  .WorldHeritage_note dt {width: 24%;}

  .WorldHeritage_note dd {
    padding: 2%;
    font-size: 16px;
  }
}

/* PC向けスタイル */
@media screen and (min-width: 1024px) {
  main {max-width: 1024px;}
  
  .WorldHeritage {
    display: flex;
    padding-bottom: 24px;
  }

  .WorldHeritage_img {margin: auto;}

  .WorldHeritage_img img {
    width: auto;
    height: 340px;
  }

  .WorldHeritage_note {
    margin: auto;
    padding-left: 16px;
  }

  .WorldHeritage_note h2 {margin: 8px auto;}
  .WorldHeritage_note dl {font-size: 18px;}
  .WorldHeritage_note dt {width: 18%;}
  .WorldHeritage_note dd {width: 14.5cm;}
}
</style>
