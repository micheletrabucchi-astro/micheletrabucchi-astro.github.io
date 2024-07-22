<script setup>
  defineProps({
    authors: {
      type: String,
      required: true
    },
    bibinfo: {
      type: String,
      required: true
    },
    adsurl: {
      type: String,
      required: true
    },
    imagePath: {
      type: String,
      required: true
    },
    flexDir: {
      type: String,
      default: "row"
    },
    pdfPath: {
      type: String,
      default: ""
    }
  })
</script>
<!-- ####################################################################### -->
<template>
  <div class="box">
    <div class="text-box">
      <div class="pdf-header-box">
        <a v-if="pdfPath === ''"></a>
        <a v-else :href="pdfPath" download><img src="../../public/icons/file-pdf-solid-salmon.svg" class="pdf-icon"/></a>
        <div class="header-box">
          <h3 class="authors">{{ authors }}</h3>
          <a :href="adsurl" target="_blank"><h4 class="bibinfo">{{ bibinfo }}</h4></a>
        </div>
      </div>
      <hr class="hline">
      <p class="abstract">
        <slot></slot>
      </p>
    </div>
    <div class="image-box">
      <img class="image" :src="imagePath" alt="" />
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
    max-height: 512px;
  }
  .authors {
    font-size: 16pt;
    font-family: 'Times New Roman';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 10px;
  }
  .bibinfo {
    font-size: 13pt;
    font-family: 'Times New Roman';
    font-style: normal;
    font-weight: 400;
    color: #414141;
    margin-bottom: 10px;
  }
  .bibinfo:hover{
    color: #000;
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
    font-family: 'Times';
    font-style: normal;
    font-weight: 300;
    color: #414141;
    margin-bottom: 10px;
    text-align: justify;
  }
</style>