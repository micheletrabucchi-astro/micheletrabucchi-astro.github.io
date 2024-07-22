<script setup>
  import Widget from './Widget.vue';
</script>
<!-- ####################################################################### -->
<template>
  <div class="widgets-block">
    <Widget iconPath="/icons/envelope-solid.svg"
            url="mailto:michele.trabucchi@unipd.it"
            altText="contact me"/>
    <Widget iconPath="/icons/orcid.svg"
            url="https://orcid.org/0000-0002-1429-2388"
            altText="ORCID"/>
    <Widget iconPath="/icons/ads.svg"
            url="https://ui.adsabs.harvard.edu/search/fq=%7B!type%3Daqp%20v%3D%24fq_database%7D&fq_database=(database%3Aastronomy%20OR%20database%3Aphysics)&q=author%3A%22trabucchi%2C%20michele%22%20collection%3Aastronomy%20orcid%3A0000-0002-1429-2388&sort=date%20desc%2C%20bibcode%20desc&p_=0"
            altText="NASA/ADS"/>
    <Widget iconPath="/icons/arxiv.svg"
            url="https://arxiv.org/search/advanced?advanced=1&terms-0-operator=AND&terms-0-term=0000-0002-1429-2388&terms-0-field=orcid&classification-physics_archives=all&classification-include_cross_list=include&date-filter_by=all_dates&date-year=&date-from_date=&date-to_date=&date-date_type=submitted_date&abstracts=show&size=50&order=-announced_date_first"
            altText="arXiv"/>
    <Widget iconPath="/icons/google-scholar.svg"
            url="https://scholar.google.com/citations?user=he03gFcAAAAJ&hl=en"
            altText="Google Scholar"/>
    <Widget iconPath="/icons/researchgate.svg"
            url="https://www.researchgate.net/profile/Michele_Trabucchi2"
            altText="ResearchGate"/>
    <Widget iconPath="/icons/scopus.svg"
            url="https://www.scopus.com/authid/detail.uri?authorId=57193167327"
            altText="Scopus"/>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .widgets-block {
    padding: 30px 0 0 0;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
</style>