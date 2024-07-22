<script setup>
  defineProps({
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
  <div class="section-box">
    <slot></slot>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .section-box {
    padding: 80px 10dvw;
    width: 100dvw;
    min-width: 1280px;
    height: 100dvh;
    background-color: v-bind(bgcolor);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: v-bind(textColor);
  }
</style>