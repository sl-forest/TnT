<template>
    <div class="loading">
      <img class="loading_logo" src="~/assets/img/Kagoshima_logo-min.png" alt="ロード画面">
    </div>
</template>

<style>
/* ロード画面 */
.loading {
  position: fixed;            /* 要素の固定 */
  top: 0;                     /* 位置調整 */
  left: 0;                    /* 位置調整 */
  width: 100vw;               /* 横幅 */
  height: 100vh;              /* 高さ */
  z-index: 100;               /* 要素を重ねる順序の指定 */
  background-color: #fff;   /* 背景 */
  display: flex;              /* 親要素に対して子要素を横並び */
  align-items: center;        /* 中央揃え */
  justify-content: center;    /* 横並び要素の中央揃え */
  animation: fadeOut 1.6s 3.2s forwards;  /* アニメーション */
}

@keyframes fadeOut {
  0% {
    opacity: 1;         /* 不透明度 */
  }

  100% {
    opacity: 0;         /* 不透明度 */
    visibility: hidden; /* 要素はあるが見えない */
  }
}

.loading_logo {
  opacity: 0;                             /* 不透明度 */
  animation: logo_fade 2s 0.5s forwards;  /* アニメーション */
  width: 175px;                           /* 横幅 */
}

@keyframes logo_fade {
  0% {
    opacity: 0;                   /* 不透明度 */
    transform: translateY(20px);  /* 要素の上下左右の位置 */
  }

  60% {
    opacity: 1;                   /* 不透明度 */
    transform: translateY(0);     /* 要素の上下左右の位置 */
  }

  100% {
    opacity: 0;                   /* 不透明度 */
  }
}
</style>