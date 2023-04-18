<template>
  <MainHeader></MainHeader>
  <div id="game">
    <health-bar :health="monsterHealth" title="Monster Health"></health-bar>
    <health-bar :health="playerHealth" title="Your Health"></health-bar>
  
    <section id="controls">
      <button>ATTACK</button>
      <button>SPECIAL ATTACK</button>
      <button>HEAL</button>
      <button>SURRENDER</button>
    </section>
    <section id="log" class="container">
      <h2>Battle Log</h2>
      <ul></ul>
    </section>
  </div>
</template>

<script>
import HealthBar from './components/HealthBar.vue';
import MainHeader from './components/MainHeader.vue';

export default {
  components: {
    MainHeader,
    HealthBar
  },
  data() {
    return {
      monsterHealth: 100,
      playerHealth: 60,
    };
  }
}
</script>

<style>

</style>
