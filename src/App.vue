<template>
  <div id="app" class="all">
    <header>
      <header-comp/>
    </header>

    <main>
      <main-comp/>
    </main>

    <footer>
      <footer-comp/>
    </footer>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  }
}
</script>

<style lang="scss">
  *{
    padding: 0;
    margin:0%;
    box-sizing: border-box;
  }

  .all{
    height: 100vh;
  }

  ul{
    list-style: none
  }
</style>
