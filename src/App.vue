<script setup>
import Ref_Example from './components/Ref_Example.vue'
import Reactive_Example from './components/Reactive_Example.vue';
import OptionsAPI from './components/OptionsAPI.vue';
// import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" /> -->
    <div class="wrapper">
      <Ref_Example />
    </div>
    <div class="wrapper">
      <Reactive_Example />
    </div>
    <div class="wrapper">
      <OptionsAPI />
    </div>
  </header>

  <main>
    <!-- <TheWelcome /> -->
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  display: flex;
  gap: 50px;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    /* padding-right: calc(var(--section-gap) / 2); */
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
