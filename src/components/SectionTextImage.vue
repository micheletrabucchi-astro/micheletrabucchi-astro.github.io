<script setup>
  import Section from './Section.vue'
  defineProps({
    imagePath: {
      type: String,
      required: true
    },
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
    <div class="text-image-box">
      <div class="text-box">
        <h2 class="title">{{ title }}</h2>
        <div class="content">
          <slot />
        </div>
      </div>
      <div class="image-box">
        <img :src="imagePath" class="image"/>
      </div>
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
    font-size: 16pt;
    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 300;
    color: #414141;
    line-height: 2;
    text-align: center;
    color: v-bind(textColor);
  }
  .text-image-box {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
  .text-box {
    padding: 0 2vw;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .image-box {
    padding: 0 2vw;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .image {
    max-width: 90%;
    max-height: 90%;
  }
</style>