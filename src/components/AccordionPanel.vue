<script setup>
  import { ref } from 'vue';
  const props = defineProps({
    handle: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    ariaTitle: {
      type: String,
      required: true
    }
  });
  // 
  const showPanel = ref(false);
  const togglePanel = (event) => {
    showPanel.value = !showPanel.value;
  }
</script>
<!-- ####################################################################### -->
<template>
  <div class="panel">
    <button class="button" @click.prevent="togglePanel" :aria-controls="'accordion-content-' + ariaTitle" :id="'accordion-control-' + ariaTitle">
      <a class="handle">{{ handle }}</a>
      <span v-if="showPanel">
        <a ><img src="../../public/icons/expand-more-black.svg" class="icon"/></a>
      </span>
      <span v-else>
        <a ><img src="../../public/icons/chevron-right-black.svg" class="icon"/></a>
      </span>
      <a v-if="showPanel" class="title-highlight">{{ title }}</a>
      <a  v-else class="title">{{ title }}</a>
    </button>
    <div :aria-hidden="!showPanel" :id="'content-' + ariaTitle" v-if="showPanel">
      <slot></slot>
    </div>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .panel {
    width: 100dvw;
  }
  .button {
    width: 100dvw;
    min-height: 50px;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    border-radius: 0;
    border-style: none;
    cursor: pointer;
    background-color: rgba(255, 255, 255, 0);
    font-size: 20pt;
    padding: 0 0 0 0;
    color: #414141;
    font-weight: 300;
  }
  .handle {
    padding: 0 2dvw 0 5dvw;
    font-size: 20pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 300;
    color: #414141;
    margin-left: 10px;
  }
  .title {
    padding: 0 1dvw 0 1.5dvw;
    font-size: 20pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 300;
    color: #414141;
    margin-left: 10px;
  }
  .title-highlight {
    padding: 0 1dvw 0 1.5dvw;
    font-size: 20pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 300;
    color: #df7366;
    margin-left: 10px;
  }
</style>