<script setup>
  import Section from './Section.vue'
  defineProps({
    title: {
      type: String,
      default: ""
    },
    bgcolor: {
      type: String,
      default: "rgba(255, 255, 255, 1)"
    },
    textColor: {
      type: String,
      default: "#414141"
    }
  })
</script>
<!-- ####################################################################### -->
<template>
  <Section :bgcolor="bgcolor">
    <h2 class="title">{{ title }}</h2>
    <div class="content">
      <slot />
    </div>
  </Section>
</template>
<!-- ####################################################################### -->
<style scoped>
  .title {
    font-size: 32pt;
    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 400;
    color: #df7366;
    margin-bottom: 30px;
  }
  .content {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 18pt;
    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    line-height: 1.5;
    text-align: center;
    color: v-bind(textColor);
  }
</style>