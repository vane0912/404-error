<template>
    <div class="text-direction">
        <h1>I have bad news for you</h1>
        <p>The page you are looking for might be removed or is temporarily unavailable </p>
        <button>BACK TO HOMEPAGE</button>
    </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&display=swap');
@mixin fontStyle($weigth: 700, $size: 50px, $color: #333333){
    font-family: 'Space Mono', monospace;
    font-weight: $weigth;
    font-size: $size;
    color: $color;
}
    h1{
        @include fontStyle();
    }
    p{
        @include fontStyle(400, 20px);
    }
    button{
        @include fontStyle(700, 14px, #FFFFFF);
        height: 15%;
        width: 40%;
        background-color: #333333;
        border: none;
        cursor: pointer;
    }
    .text-direction{
        height: 70%;
        width: 40%;
    }
    @media screen and (max-width: 916px) {
    h1{
      font-size: 30px;
    }
    p{
      font-size: 15px;
    }
    button{
        width: 80%;
        height: 15%;
    }
    .text-direction{
        width: 80%;
    }
  }
</style>
