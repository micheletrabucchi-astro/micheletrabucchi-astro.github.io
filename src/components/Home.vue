<script setup>
  import Widget from './Widget.vue';
  import WidgetsBlock from './WidgetsBlock.vue';
</script>
<!-- ####################################################################### -->
<template>
  <div class="home-box">
    <img src="/images/portrait.png" class="portrait" alt="Portrait of the scientist as a young man..." />
    <h1 class="maintitle">Michele Trabucchi</h1>
    <div class="affiliation-box">
      <Widget iconPath="/icons/unipd-logo-text.svg"
              url="https://www.unipd.it/en/" widgetHeight="100px" widgetWidth="200px" transitionDuration="0.5s"/>
      <h2 class="subtitle">Research Fellow @ <a href="https://www.unipd.it/en/">UniPd</a><br><a href="http://www.dfa.unipd.it/en/">Department of Physics & Astronomy</a></h2>
      <Widget iconPath="/icons/dfa-logo-text.svg"
              url="http://www.dfa.unipd.it/en/" widgetHeight="100px" widgetWidth="200px" transitionDuration="0.5s"/>
    </div>
    <hr class="hline"/>
    <WidgetsBlock/>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .home-box {
    height: 100dvh;
    width: 100dvw;
    min-width: 1280px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .portrait {
    height: 180px;
    padding: 0 0 0 0;
  }
  .maintitle {
    padding: 60px 0 10px 0;
    font-size: 60pt;
    font-family: Ubuntu, sans-serif;
    font-weight: 400;
    text-align: center;
    color: white;
    text-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  .affiliation-box {
    padding: 10px 0 10px 0;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
  .subtitle {
    padding: 0 50px 10px 50px;
    font-size: 24pt;
    font-family: Ubuntu, sans-serif;
    font-weight: 300;
    text-align: center;
    color: white;
    text-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  .hline {
    padding: 0 0 0 0;
    width: 55%;
    border: 0;
    height: 6px;
    border-top: 3px solid rgba(255, 255, 255, 0.5);
  }
</style>