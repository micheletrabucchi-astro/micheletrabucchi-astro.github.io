<!-- 
  Requires:
    npm install @vueuse/core
-->
<script setup>
  import { ref } from 'vue';
  import { useElementVisibility } from '@vueuse/core';
  //
  import Home from './components/Home.vue'
  import TopMenu from './components/TopMenu.vue'
  import Footer from './components/Footer.vue'
  import SectionText from './components/SectionText.vue'
  import SectionTextImage from './components/SectionTextImage.vue'
  import SectionPublications from './components/SectionPublications.vue'
  import SectionConferences from './components/SectionConferences.vue'
  //
  const projSect = ref(null);
  const projSectVisible = useElementVisibility(projSect);
  const collSect = ref(null);
  const collSectVisible = useElementVisibility(collSect);
  const bioSect = ref(null);
  const bioSectVisible = useElementVisibility(bioSect);
</script>
<!-- ####################################################################### -->
<template>
  <TopMenu/>
  <div class="wrapper">
    <img v-if="projSectVisible" src="/images/convergence.jpg" class="background"/>
    <img v-else-if="collSectVisible" src="/images/gaia-sky.jpg" class="background"/>
    <img v-else-if="bioSectVisible" src="/images/bio.jpg" class="background"/>
    <img v-else src="/images/background.jpg" class="background"/>
    <!--  -->
    <Home id="home"/>
    <!--  -->
    <SectionText id="research" title="Research" bgcolor="rgba(255, 255, 255, 1)">
      <div>
        My primary research interest is <b>stellar structure and evolution</b>, with
        a focus on <b>late evolutionary stages</b> and <b>stellar variability</b>.
        Since my PhD project I have been working on the computation and analysis of
        wide grids of non-adiabatic, radial <b>pulsation models of evolved red
        giants</b>, aimed at providing the community with up-to-date, easy-to-use
        prescriptions to predict the variability properties of <b>long-period
        variables</b>. In its most recent iteration, this reasearch led to the first
        accurate prescription for describing the variability periods of <b>Mira-like
        large-amplitude pulsators</b>. I am also interested in the analysis of
        observational data on stellar variability from large-scale surveys. I am a
        member of the Data Processing & Analysis Consortium of the ESA <b><em>Gaia
        </em> mission</b>, in which I have been working on the preparation of the
        most recent catalog of long-period variables, and I am a Junior Associate in
        the <b>Rubin-LSST</b> Italian Scientific Collaboration.
      </div>
    </SectionText>
    <!--  -->
    <SectionTextImage ref="projSect" id="projects" title="Projects" bgcolor="rgba(255, 255, 255, 0)" imagePath="/images/convergence-logo-text.png" textColor="#fff">
      <div>
        I am PI of the <b><em>CONVERGENCE</em></b> project, funded by the University of
        Padova through the
        <a href="https://www.unipd.it/bando-stars2023"><em>STARS@UniPd 2023</em></a> scheme.
        The project aims at developing a descriptive model of the <em>long secondary periods</em>
        observed together with pulsation in the light curves of evolved red giants.
        The origin of this phenomenon is still debated, and one of the main interpretations
        involves accretion on a substellar companion resulting in a dust cloud that
        periodically attenuates the stellar light. The final goal of <b><em>CONVERGENCE</em></b>
        is constrain stellar mass loss rates and characterize the population of accreting
        substellar companions in the Milky Way and in the Magellanic Clouds.
      </div>
    </SectionTextImage>
    <!--  -->
    <SectionPublications id="publications" title="Publications">
      <p>
        Below you can find a selection of my main scientific papers
        (click on the titles to show summary panels).
        <br>
        A complete list of my
        publications can be found at the
        <a class="link" href="https://ui.adsabs.harvard.edu/search/fq=%7B!type%3Daqp%20v%3D%24fq_database%7D&fq_database=(database%3Aastronomy%20OR%20database%3Aphysics)&q=author%3A%22trabucchi%2C%20michele%22%20collection%3Aastronomy%20orcid%3A0000-0002-1429-2388&sort=date%20desc%2C%20bibcode%20desc&p_=0">
        NASA Astrophysics Data System (ADS)
        </a>.
      </p>
    </SectionPublications>
    <!--  -->
    <SectionTextImage ref="collSect" id="collaborations" title="Main Collaborations" bgcolor="rgba(255, 255, 255, 0)" imagePath="/images/collab-logos.png" textColor="#fff">
      <div class="list-text">
        <li>
          <a href="https://ui.adsabs.harvard.edu/search/filter_database_fq_database=AND&filter_database_fq_database=((database%3Aastronomy%20OR%20database%3Aphysics))&filter_database_fq_database=database%3A%22astronomy%22&filter_property_fq_property=AND&filter_property_fq_property=property%3A%22refereed%22&fq=%7B!type%3Daqp%20v%3D%24fq_database%7D&fq=%7B!type%3Daqp%20v%3D%24fq_property%7D&fq_database=(((database%3Aastronomy%20OR%20database%3Aphysics))%20AND%20database%3A%22astronomy%22)&fq_property=(property%3A%22refereed%22)&q=abs%3A%22gaia%22%20orcid%3A0000-0002-1429-2388%20(author%3A%22Gaia%20Collaboration%22%20OR%20title%3A%22Gaia%20Data%20Release%22)%20year%3A2020-3020&sort=date%20desc%2C%20bibcode%20desc&p_=0" target="_blank">
          Member of the <b><em>Gaia</em> Data Processing & Analysis Consortium</b>,
          Coordination Unit 7 (Variability), part of the core team
          responsible for the <b>long-period variables Working Package</b>.
          </a>
        </li>
        <li>
          <a href="https://ui.adsabs.harvard.edu/search/fq=%7B!type%3Daqp%20v%3D%24fq_database%7D&fq_database=(database%3Aastronomy%20OR%20database%3Aphysics)&q=abs%3A%22lsst%22%20orcid%3A0000-0002-1429-2388&sort=date%20desc%2C%20bibcode%20desc&p_=0" target="_blank">
          Junior Associate in the <b>Rubin-LSST</b> Italian Scientific Collaboration,
          member of the <b>Stars, Milky Way, and Local Volume Science Collaboration</b>
          and of the <b>Transients and Variable Stars Science Collaboration</b>, active
          in the simulation of the LSST stellar population content.
          </a>
        </li>
        <br>
      </div>
      <h2>Past Collaborations</h2>
      <div class="list-text">
        <li>
          <a href="http://starkey.astro.unipd.it/index.html" target="_blank">
          The <b>STARKEY</b> project: core team member, responsible for the "Pulsation" Work Package
          </a>
        </li>
        <li>
          <a href="http://www.asterochronometry.eu/haydn/" target="_blank">
          The <b>HAYDN</b> ESA Voyage 2050 Proposal: responsible for the "Mass Loss" Working Group.
          </a>
        </li>
        <li>
          <a href="https://www.issibern.ch/teams/shot/" target="_blank">
          The <b>SHoT</b> ISSI Team: self-supporting expert on threotical pulsation models of evolved red giants.
          </a>
        </li>
      </div>
    </SectionTextImage>
    <!--  -->
    <SectionConferences id="conferences" title="Conferences, Seminars, Talks">
    </SectionConferences>
    <!--  -->
    <SectionText id="teaching" title="Teaching" bgcolor="rgba(255, 255, 255, 0)" textColor="#fff">
      <div>
        At the Department of Physics and Astronomy of the University of Padova
        I am involved in teaching and mentoring activities.
        Since 2023 I am responsible for the course unit
        <a class="link" href="https://en.didattica.unipd.it/off/2023/LM/SC/SC2490" target="_blank">
          <b>"Advanced Astrophysics"</b></a> for
        <a class="link" href="https://en.didattica.unipd.it/off/2023/LM/SC/SC2490/001PD/SCP9086382/N0" target="_blank">
          the Master's Degree in Astrophysics and Cosmology</a>
        at the University of Padova.
        <br>
        <br>
        <br>
        <br>
      </div>
      <h2>Past Teaching Experiences</h2>
      <div class="list-text">
        <br>
        <li>
          2024 ‣ Teacher in charge, course unit: "Astrofisica 2" — Bachelor's Degree in Astronomy, University of Padova
        </li>
        <li>
          2023 ‣ Lab Teacher, course unit: "Fisica" — Bachelor's Degrees in Biology, Biotechnologies, University of Padova
        </li>
        <li>
          2020-2022 ‣ Teaching Collaborator, course units "Astrophysics Lab I, II" — Master's Degreesin Astrophysics, University of Geneva
        </li>
        <li>
          2020-2022 ‣ Teaching Collaborator, course unit "Theoretical Physics III" — Bachelor's Degree in Physics, University of Geneva
        </li>
        <li>
          2019-2020 ‣ Teaching Assistant, course unit: "Advanced Astrophysics" — Master's Degree in Astrophysics & Cosmology, University of Padova
        </li>
        <li>
          2018-2019 ‣ Teaching Assistant, course unit: "Theoretical Astrophysics" — Master's Degree in Astronomy, University of Padova
        </li>
        <li>
          2015-2016 ‣ Computer Lab Teaching Assistant, course unit: "Theoretical Astrophysics" — Master's Degree in Astronomy, University of Padova
        </li>
      </div>
    </SectionText>
    <!--  -->
    <SectionTextImage id="outreach" title="Outreach" imagePath="/images/outreach.png">
      <div>
        Since 2018 I am engaged in outreach activities aimed at promoting the
        understanding of science and the scientific method among the general
        public. In particular, I have been involved in the organization of the
        European Researchers' Night in Padova, and later on in the
        <a class="link" href="https://science4all.it/" target="_blank">
          Science 4 All</a> activities of the University of Padova.
        <br>
        <br>
        As a <em>Gaia</em> DPAC member I take part in the outreach activities and
        events organized for the Data Release days. As main author of one of the
        <a class="link" href="https://ui.adsabs.harvard.edu/abs/2023A%26A...680A..36G/abstract" taget="_blank">
        <em>Gaia</em> Focused Product Release papers</a> I actively contributed to
        the organization of <a class="link" href="https://www.oapd.inaf.it/seminari-ed-eventi/aperitivo-con-gaia" target="_blank">
        local events in Padova</a>.
        </div>
    </SectionTextImage>
    <!--  -->
    <SectionText ref="bioSect" id="bio" title="" bgcolor="rgba(0, 0, 0, 0.4)" textColor="white">
      <div>
        <h1>Bio</h1>
        <br>
        I graduated in Astronomy at the University of Padova in 2014, with a
        thesis on the modelling of solar like oscillations in red giant branch
        stars.
        <br>
        <br>
        I then obtained a PhD in Astronomy at the same institution in 2018,
        working within the STARKEY project on the computation and analysis of
        non-adiabatic pulsation models of evolved red giants.
        <br>
        <br>
        From 2020 to 2022 I worked as a postdoc at the University of Geneva,
        studying the use of semi-regular red giant variables as standard candles
        and contributing to the preparation of the Gaia Data Release 3.
        <br>
        <br>
        I am currently a Research Fellow at the Department of Physics &
        Astronomy of the University of Padova.
        <br>
        <br>
        <a class="link" href="/files/MicheleTrabucchi_CV_2024.pdf" download>Download my CV</a>
      </div>
    </SectionText>
    <!--  -->
    <Footer></Footer>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .background{
    position: fixed;
    width: 100dvw;
    min-width: 1920px;
    min-height: 1080px;
    top: 0;
    left: 0;
    z-index: -1;
  }
  .list-text {
    font-size: 18pt;
    font-weight: 300;
    color: #fff;
    line-height: 1.5;
    text-align: left;
    list-style-type: square;
  }
  .link {
    text-decoration: underline;
    text-decoration-style: dotted;
    color: inherit;
  }
</style>