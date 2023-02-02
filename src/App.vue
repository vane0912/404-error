<template>
  <nav>
    <h2>404 NOT FOUND</h2>
  </nav>
  <main class="style-components">
    <ScareCrowComponent/>
    <ErrorTextAndButton />
  </main>
  <footer>
    <p>created by vane09 - devChallenges.io</p>
  </footer>
</template>
<script setup>
  import ErrorTextAndButton from './components/Error-text-and-button.vue';
  import ScareCrowComponent from './components/ScareCrowComponent.vue';
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Inconsolata:wght@700&display=swap');
@mixin heightAndWidth(){
    height: 100%;
    width: 100%;
    margin: 0;
    background-color: #FFFF;
}
  h2{
    font-family: 'Inconsolata', monospace;
    margin: 0;
  }
  nav{
    padding: 3% 5%;
  }
  #app{
    @include heightAndWidth();
  }
  body{
    @include heightAndWidth();
  }
  html{
    @include heightAndWidth();
  }
  .style-components{
    display: flex;
    justify-content: space-evenly;
    height: 70%;
    align-items: center;
  }
  footer{
    position: fixed;
    bottom: 0;
    width: 100%;
    display: flex;
    justify-content: center;
  }
  footer p{
    color: #BDBDBD;
    font-size: 10px;
  }
  @media screen and (max-width: 916px) {
    .style-components{
      flex-direction: column;
      height: 90%;
      padding: 10%;
    }
    h2{
      font-size: 20px;
    }
  }
</style>
