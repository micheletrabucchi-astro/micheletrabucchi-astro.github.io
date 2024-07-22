<script setup>
  defineProps({
    eventTitle: {
      type: String,
      required: true
    },
    eventSubtitle: {
      type: String,
      default: ""
    },
    eventLocation: {
      type: String,
      default: ""
    },
    eventUrl: {
      type: String,
      default: ""
    },
    talkType: {
      type: String,
      default: "Contributed Talk"
    },
    talkTitle: {
      type: String,
      required: true
    },
    talkPdfPath: {
      type: String,
      default: ""
    },
    eventImagePath: {
      type: String,
      default: ""
    },
    flexDir: {
      type: String,
      default: "row"
    }
  })
</script>
<!-- ####################################################################### -->
<template>
  <div class="box">
    <div class="text-box">
      <div class="pdf-header-box">
        <a v-if="talkPdfPath === ''"></a>
        <a v-else :href="talkPdfPath" download><img src="../../public/icons/file-pdf-solid-salmon.svg" class="pdf-icon"/></a>
        <div class="header-box">
          <a :href="eventUrl" target="_blank">
            <h2 class="event-title">{{ eventTitle }}</h2>
            <h3 class="event-subtitle">{{ eventSubtitle }}</h3>
            <h3 class="event-subtitle">{{ eventLocation }}</h3>
          </a>
        </div>
      </div>
      <hr class="hline">
      <h2 class="talk-title">{{ talkTitle }}</h2>
      <h3 class="talk-type">{{ talkType }}</h3>
      <p class="abstract">
        <slot></slot>
      </p>
    </div>
    <div class="image-box">
      <img class="image" :src="eventImagePath" alt="" />
    </div>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .box{
    display: flex;
    flex-direction: v-bind(flexDir);
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 100%;
    padding: 10px 5dvw 30px 5dvw;
  }
  .text-box {
    width: 60%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .pdf-header-box {
    width: 100%;
    display: flex;
    flex-direction: v-bind(flexDir);
    justify-content: center;
    align-items: center;
  }
  .header-box {
    width: 90%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .pdf-icon {
    height: 30px;
    width: 30px;
    margin-right: 10px;
    cursor: pointer;
  }
  .image-box {
    padding: 10px 10px 10px 10px;
    width: 40%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .image {
    max-height: 400px;
  }
  .hline {
    padding: 0 0 0 0;
    width: 75%;
    border: 0;
    height: 6px;
    border-top: 1px solid rgba(0, 0, 0, 0.5);
  }
  .abstract {
    padding: 10px 30px 10px 30px;
    font-size: 14pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 300;
    color: #414141;
    margin-bottom: 10px;
    text-align: justify;
  }
  .event-title {
    font-size: 16pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 10px;
    text-align: center;
  }
  .event-title:hover{
    color: #000;
  }
  .event-subtitle {
    font-size: 11pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 4px;
    text-align: center;
  }
  .event-subtitle:hover{
    color: #000;
  }
  .talk-title {
    font-size: 16pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 6px;
    text-align: center;
  }
  .talk-type {
    font-size: 13pt;
    font-family: 'Roboto';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 6px;
    text-align: center;
  }
</style>