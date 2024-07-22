<script setup>
  defineProps({
    iconPath: {
      type: String,
      required: true
    },
    url: {
      type: String,
      required: true
    },
    altText: {
      type: String,
      default: ""
    },
    widgetHeight: {
      type: String,
      default: "56px"
    },
    widgetWidth: {
      type: String,
      default: "76px"
    },
    iconHeight: {
      type: String,
      default: "52px"
    },
    transitionDuration: {
      type: String,
      default: "0.1s"
    }
  })
</script>
<!-- ####################################################################### -->
<template>
  <div class="widget">
    <a :href="url" target="_blank"><img :src="iconPath" class="icon" :title="altText"/></a>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .widget {
    padding: 0 10px 0 10px;
    height: v-bind(widgetHeight);
    width: v-bind(widgetWidth);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
  .icon {
    height: v-bind(iconHeight);
    transition: height v-bind(transitionDuration);
    transition-timing-function: ease-in-out;
  }
  .icon:hover {
    height: v-bind(widgetHeight);
  }
</style>