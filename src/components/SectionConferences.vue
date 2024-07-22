<script setup>
  import AccordionPanel from './AccordionPanel.vue';
  import Talk from './Talk.vue';
  //
  defineProps({
    title: {
      type: String,
      default: ""
    },
    bgcolor: {
      type: String,
      default: "rgba(255, 255, 255, 1)"
    }
  })
</script>
<!-- ####################################################################### -->
<template>
  <div class="section-box">
    <h2 class="title">{{ title }}</h2>
    <div class="content">
      <slot></slot>
    </div>
    <!--  -->
    <AccordionPanel
      aria-title="lssteu6"
      handle="(2024)"
      title="La Palma — LSST@Europe 6">
      <Talk
        eventTitle="European Astronomical Society Annual Meeting"
        eventSubtitle=""
        eventLocation="La Palma, Canary Islands (Spain)"
        eventUrl="https://meetings.iac.es/LSSTEurope6/"
        talkTitle="Modeling long-period variability in evolved stars for Rubin-LSST"
        talkType="Contributed Talk"
        eventImagePath="/images/lsst-europe-6.jpg"
        talkPdfPath=""
        >
        Low- to intermediate-mass stars evolve to the asymptotic giant branch (AGB) phase during which they display pulsation over months- to years-long time scales as long-period variables (LPVs). This process is crucial to understanding the late evolution and death of these stars, their stellar winds and the resulting pollution of the interstellar medium, as well as their compact remnants and the initial-final mass relation. Our knowledge of LPVs and related phenomena, as well as their astrophysical applications such as measuring stellar distances and ages, will benefit enormously from the LSST program thanks to its long planned duration. The full exploitation of such observations requires solid theoretical grounds. During this talk I will cover a number of recent developments in our work involving the modeling of pulsation in evolved stars and the simulation of variability properties of populations of LPVs, part of our in-kind contribution to Rubin-LSST. I will also discuss a number of parallel projects, related to this topic, that are being carried out among our group and are expected to be of interest for the Rubin community.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="eas_2024"
      handle="(2024)"
      title="Padova — EAS 2024">
      <Talk
        eventTitle="European Astronomical Society Annual Meeting"
        eventSubtitle="Gaia: The (TWO) Billion Star Galaxy Census: from the Solar System to our Milky Way and beyond"
        eventLocation="Centro Congressi PadovaFiere, Padova (Italy)"
        eventUrl="https://eas.unige.ch/EAS2024/session.jsp?id=S4"
        talkTitle="The Gaia Focused Product Release Catalog of Long-Period Variable candidates"
        talkType="Contributed Talk"
        eventImagePath="/images/eas-padova-2024.png"
        talkPdfPath="/files/talk_trabucchi_padova2024.pdf"
        flexDir="row-reverse"
        >
        Long-period variables (LPVs) represent the late evolutionary stages of low- to intermediate-mass stars (on the Asymptotic Giant Branch, AGB) or massive stars (Red Supergiants, RSGs). They display periodic variability attributed primarily to stellar pulsation in several low-order modes, possibly at the same time. They also exhibit long-term periodic changes, dubbed “long secondary periods” (LSPs), whose nature is still unclear. Understanding these variability processes is crucial to study the evolution of these stars and the mass-loss process that leads to their death, as well as to the enrichment of the interstellar medium by their nucleosynthesis products. In 2016, the second Gaia Data Release (Gaia DR2) delivered photometric time series for over 150'000 LPV candidates based on 22 months of observations. With Gaia DR3 (2022), this number increased to more than 2.3 millions, extending the span of the time series up to 34 months. Among them, 10’000 sources brighter than G=14mag were selected and published with their radial velocity time series as part of the Gaia Focused Product Release (FPR) of October 2023. While measuring the mean radial velocity of a star is a key ingredient to understanding the dynamics of the Galaxy's stellar content, Gaia's multi-epoch observations allow us to monitor radial velocity variability - in parallel to photometric variability. I will present the purpose, construction and content of the FPR catalog of LPVs, focusing on the potential provided by the combination of epoch photometry and radial velocity data distinguishing between different types of variability such as pulsation, LSPs, and ellipsoidal variations. The LPV catalogue published in the FPR is an appealing teaser for what is expected for DR4. It has already substantially expanded the availability of epoch radial velocity data for long-period variables, and is of unprecedented value for investigating the variability of evolved red giants.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="seminar_heidelberg"
      handle="(2024)"
      title="[Virtual] — Seminar @ MPA Stellar Group">
      <Talk
        eventTitle="Invited Seminar"
        eventSubtitle="Max-Planck-Institut für Astronomie"
        eventLocation="Heidelberg (Germany)"
        eventUrl=""
        talkTitle="Long-Period Variables: Recent Developments in the Modelling and Interpretation"
        talkType=""
        eventImagePath="/images/talk-bg.jpg"
        talkPdfPath="/files/seminar_trabucchi_heidelberg2024.pdf"
        flexDir="row"
        >
        During their late evolution, low-/intermediate-mass stars become very luminous, mass-losing, pulsating red giants called "long-period variables". Characterizing their pulsation physics is crucial to understand their evolution and impact on the circumstellar environment, as well as to exploit their potential as distance and age indicators. I will present an overview of the main results in this context achieved by our research group in recent years, their impact on our understanding of the observed properties of these stars, and the next development planned for the future.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="lssteu5"
      handle="(2023)"
      title="Poreč — LSST@Europe 5">
      <Talk
        eventTitle="LSST@Europe 5"
        eventSubtitle="Towards LSST science, together!"
        eventLocation="Poreč (Croatia)"
        eventUrl="https://www.lssteu5.eu/"
        talkTitle="Simulating the pulsation of long-period variables for LSST"
        talkType="Contributed Talk"
        eventImagePath="/images/lsst-europe-5-logo.png"
        talkPdfPath="/files/talk_trabucchi_porec2023.pdf"
        flexDir="row-reverse"
        >
        Long-period variables (LPVs) represent the final stages in the evolution of low- and intermediate-mass stars. As they evolve on the Asymptotic Giant Branch (AGB) they become unstable to pulsation in multiple modes, with periods of orders of months up to years, and amplitudes from a milli-magnitude level up to several magnitudes in visual bands. With its high cadence and multi-year observational baseline, LSST is expected to provide exceptional data to study these stars and to exploit their potential for several applications of high astrophysical interest, including distance measurements and age estimates, constraining stellar evolution models, and investigating stellar mass-loss and the chemical evolution of galaxies. Such studies will have to rely on solid theoretical grounds in terms of the description of stellar pulsation in red giant stars, and its connection with stellar structure and evolution. I report on the ongoing effort to compute an updated grid of 1D hydrodynamic models to accurately describe the pulsation of the envelope of evolved stars, with the purpose of enabling the continuous analysis of LPVs observed by LSST throughout the survey. The new grid will fully cover the space of AGB stellar parameters with special attention to chemical composition, so to be able to describe both O-rich and C-rich chemical types, as well as multiple astrophysical environments with different metallicities (the Galactic halo, disk and bulge, dwarf galaxies, and so on). The models will allow for the derivation of an accurate connection between variability observables (multiple pulsation periods) and underlying physical properties (mass, radius, metallicity). The grid will also give access to optimized template light curves and cycle variations of relevant physical quantities, enabling a detailed characterization of LSST observations as well as a deeper understanding of the physics of evolved stars.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="30_cu7"
      handle="(2023)"
      title="Napoli — 30th Gaia DPAC CU7 Meeting">
      <Talk
        eventTitle="30th Meeting of the Gaia DPAC Coordination Unit 7"
        eventSubtitle=""
        eventLocation="INAF - Osservatorio Astronomico di Capodimonte, Napoli (Italy)"
        eventUrl="https://sites.google.com/inaf.it/cu7-meeting-n-30/home"
        talkTitle="Focused Product Release: Radial Velocities Time Series of Long-Period Variables"
        talkType="Invited Report"
        eventImagePath="/images/oacn.jpg"
        talkPdfPath=""
        flexDir="row"
        >
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="iaus376"
      handle="(2023)"
      title="[Virtual] — IAU Symposium 376">
      <Talk
        eventTitle="International Astronomical Union Symposium 376"
        eventSubtitle="At the cross-roads of astrophysics and cosmology: Period-luminosity relations in the 2020s"
        eventLocation="Budapest (Hungary)"
        eventUrl="https://iaus376.org/"
        talkTitle="Long-Period Variables as Distance and Age Indicators in the Era of Gaia and LSST"
        talkType="Invited Talk"
        eventImagePath="/images/iaus-376.jpg"
        talkPdfPath="/files/talk_trabucchi_budapest2023.pdf"
        flexDir="row-reverse"
        >
        Low- and intermediate-mass stars terminate their evolution on the Asymptotic Giant Branch (AGB) as Long-Period Variables (LPVs): bright red giants pulsating on timescales between about a month and a few years. Their variability is known as a powerful diagnostic for constraining stellar physics (most importantly dust formation and mass loss, key to galaxy evolution) and estimating elusive stellar properties (masses, radii, …). LPVs obey period-age and period-luminosity relations enabling their use as distance indicators and for mapping young- and intermediate-age stellar populations. Miras, a class of highly luminous LPVs characterized by large visual amplitudes, are especially promising for reaching further distances than those accessible to Classical Cepheids. In this talk I will provide an overview of our recent research in this active field, with focus on two main subjects. I will discuss the current status and prospects of the theoretical machinery developed by the Padova stellar research group. This highly integrated framework of evolutionary tracks, pulsation models, and stellar population synthesis tools was crucial to attain a self-consistent interpretation of the global properties of LPVs observed by OGLE and Gaia in the Magellanic Clouds, and will be foundational to analyze the massive amount of data from upcoming large-scale variability surveys such as Rubin-LSST. At the same time, the understanding obtained from these models is instrumental for the extraction of a substantial wealth of information still buried in existing observational catalogs. This is especially true for the Semi-Regular Variables (SRVs), the somewhat neglected progenitors of Miras, that have the potential to complement the latter as distance indicators. Compared to Miras, SRVs are more numerous in any given stellar population, follow the same period-luminosity relation as well as an additional one and suffer from shallower circumstellar extinction. Moreover, they are found in older stellar populations, often probed with RR Lyrae variables, compared to which the SRVs are substantially brighter. These arguments motivated a project aimed at assessing their potential as standard candles, the results of which I will present in the second part of this talk.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="dpac_6"
      handle="(2023)"
      title="[Virtual] — Gaia DPAC 2023">
      <Talk
        eventTitle="6th Meeting of the Gaia Data Processing and Analysis Consortium"
        eventSubtitle=""
        eventLocation="Neue Universität, Heidelberg (Germany)"
        eventUrl="https://zah.uni-heidelberg.de/talks-seminars-events/gaia-dpac-2021-153-1932021"
        talkTitle="Gaia Focused Product Release - Epoch Radial Velocities for Long-Period Variables"
        talkType="Invited Report"
        eventImagePath="/images/dpac-2023.jpg"
        talkPdfPath=""
        flexDir="row"
        >
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="lssteu4"
      handle="(2022)"
      title="Roma — LSST@Europe 4">
      <Talk
        eventTitle="LSST@Europe 4"
        eventSubtitle="Shaping the European Contribution to LSST"
        eventLocation="Accademia dei Lincei, Roma (Italy)"
        eventUrl="https://sites.google.com/inaf.it/lssteurope4"
        talkTitle="Simulating Miras & Long-Period Variables in LSST"
        talkType="Contributed Talk"
        eventImagePath="/images/lsst-europe-4-logo.png"
        talkPdfPath="/files/talk_trabucchi_roma2022.pdf"
        flexDir="row-reverse"
        >
        Long-period variables (LPVs) are pulsating stars approaching the tip of the red giant branch or the end of their evolution on the asymptotic giant branch (AGB). They obey one ore more period-luminosity relations and can reach high intrinsic luminosities, which make them promising distance indicators. Moreover, they have distinctively red colors and can reach very large photometric amplitudes of variability in the Mira-like phase, thus being easily detectable and identifiable. Pulsation in the AGB is a crucial part in the processes of mass-loss, dust formation and the enrichment of the interstellar medium, and is a powerful diagnostic to constrain global stellar parameters and improve stellar evolutionary models. I will present the results of recent pulsation models of LPVs, that will be implemented in the simulations of the LSST stellar content.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="lsst_regional_2"
      handle="(2022)"
      title="Plitviče — The 2nd LSST Regional Workshop">
      <Talk
        eventTitle="The 2nd LSST Regional Workshop"
        eventSubtitle=""
        eventLocation="Plitviče (Croatia)"
        eventUrl="http://faculty.washington.edu/ivezic/lsst/LOI2022Plitvice/"
        talkTitle="Long-Period Variables as Distance and Age Indicators"
        talkType="Contributed Talk"
        eventImagePath="/images/plitvice.jpg"
        talkPdfPath=""
        flexDir="row"
        >
        The end-point of stellar evolution on the Asymptotic Giant Branch (AGB) is represented by Mira variables, large-amplitude fundamental-mode pulsators whose NIR period-luminosity relation (PLR) is a promising standard candle. Semi-regular variables (SRVs), the direct progenitors of Miras, are traditionally considered as a distinct variability type than Miras, and rarely considered as potential distance indicators. A systematic analysis of OGLE-III data for Miras and SRVs in the Magellanic Clouds shows that SRVs can actually be very similar to Miras, and that a revision of the traditional distinction between the two could lead to considerable benefits in terms of the performance of their PLR as a distance indicator. Because of this relation, such stars can also be used as age indicators. This has been known for several decades because of the relation between their periods and average kinematics, which connect longer-period Miras with younger stellar populations. Using a new prescription I derived from hydrodynamic models for accurately computing the pulsation periods of Miras as a function of physical parameters, I present the first theory-based analysis of the period-age relation of LPVs, and discuss its implications.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="delve"
      handle="(2021)"
      title="[Virtual] — DELVE">
      <Talk
        eventTitle="DELVE: The Death-Throes of Evolved Stars"
        eventSubtitle="A Virtual Encounter"
        eventLocation="KU Leuven Institute of Astronomy (Belgium)"
        eventUrl="https://fys.kuleuven.be/ster/events/conferences/2021/delve"
        talkTitle="Advancements in the Modelling and Interpretation of Long-Period Variables"
        talkType="Contributed Talk"
        eventImagePath="/images/delve.jpg"
        talkPdfPath="/files/talk_trabucchi_delve2021.pdf"
        flexDir="row-reverse"
        >
        AGB stars display long-period variability (of order of hundreds of days) due to stellar pulsation, which is crucial in the mass-loss process that leads to the death of these stars. It is also a valuable investigation tool as, once backed by accurate models, it provides a way to estimate global stellar parameters. Moreover, AGB stars follow several distinct period-luminosity relations, and being intrinsically bright have thus the potential of being powerful distance indicators. The frequent multi-periodic nature of long-period variables adds a degree of complexity to their observed light curves that often makes their analysis more difficult, but at the same time carries additional physical information on their nature. In this talk I will present the most recent results concerning the nonlinear modelling of pulsation in AGB stars, and the first accurate prescription for the fundamental mode pulsation of Miras and related long-period variables, in agreement with observations of evolved red giants in the Magellanic Clouds. I will also present the preliminary results of the ongoing efforts to analyze multi-periodicity in long-period variables and apply it to the characterization of evolved stellar populations and their use as standard candles.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="brite_2019"
      handle="(2019)"
      title="Wien — Stars and their Variability Observed from Space">
      <Talk
        eventTitle="Stars and their Variability Observed from Space"
        eventSubtitle="Celebrating the Birthday of BRITE-Constellation"
        eventLocation="Universität Wien (Austria)"
        eventUrl="https://starsandspace.univie.ac.at/home/"
        talkTitle="Modelling Long-Period Variables in the Gaia Era"
        talkType="Contributed Talk"
        eventImagePath="/images/brite-2019.jpg"
        talkPdfPath="/files/talk_trabucchi_wien2019.pdf"
        flexDir="row"
        >
        Long-period variables (LPVs) are asymptotic giant branch (AGB) and upper red giant branch (RGB) stars that exhibit variability due to stellar oscillations in one or more modes of low radial order. Owing to the strong link between pulsation and stellar properties, their observed periods and amplitudes provide a powerful tool to estimate stellar masses and radii. Being deeply entwined with highly uncertain processes such as convection, mass-loss, and dust-formation, the variability of these evolved stars represents a promising channel to better understand stellar physics. Finally, LPVs follow several distinct period-luminosity relations that hold a high potential as distance indicators. Large-scale microlensing surveys (EROS, MACHO, OGLE) carried on during the last few decades turned the Magellanic Clouds into ideal laboratories to study the ensemble properties of LPVs. Today, the Gaia mission is providing new insight into these objects, as well as new possibilities to apply them to the characterization of stellar populations. I will present here some of these recent results, as well as a novel approach to their interpretation based on the combination of new pulsation models with state-of-the-art synthetic stellar population models. I will cover the main shortcomings of the theory that are becoming evident from the emerging picture of LPVs in the Magellanic Clouds, as well as the constraints offered by variability observations to improve theoretical models.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="seminar_uppsala"
      handle="(2019)"
      title="Uppsala — Seminar @ Uppsala Universitet">
      <Talk
        eventTitle="Invited Seminar"
        eventSubtitle="Department of Physics and Astronomy, Uppsala University"
        eventLocation="Uppsala (Sweden)"
        eventUrl=""
        talkTitle="Long-Period Variables - Pulsating AGB Stars in the Gaia Era"
        talkType=""
        eventImagePath="/images/talk-bg.jpg"
        talkPdfPath="/files/seminar_trabucchi_uppsala2019.pdf"
        flexDir="row-reverse"
        >
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="iauga_30"
      handle="(2018)"
      title="Wien — IAU Symposium 343">
      <Talk
        eventTitle="30th General Assembly of the International Astronomical Union"
        eventSubtitle="Symposium 343 – Why Galaxies Care About AGB Stars - A Continuing Challenge Through Cosmic Time"
        eventLocation="Austria Center, Wien (Austria)"
        eventUrl="https://astronomy2018.univie.ac.at/symposia/symposium343/index.htm"
        talkTitle="Characterization of Long-Period Variables in the Magellanic Clouds"
        talkType="Contributed Talk"
        eventImagePath="/images/iauga-30.jpg"
        talkPdfPath=""
        flexDir="row"
        >
        Asymptotic Giant Branch (AGB) stars often exhibit pulsation in modes of low radial order and periods between a few days and a few thousand days. The observed periods and variability amplitudes of such Long-Period Variables (LVPs) provide an additional constraint to be matched by stellar evolution and population models, as well as a powerful tool to infer stellar parameters. LPVs are known to follow several well defined period-luminosity (PL) relations at infrared wavelengths, representing promising distance indicators, especially in the case of the bright, large-amplitude Mira variables. In order to fully exploit the potential of LPVs in the study of stellar evolution and stellar populations, it is necessary to understand and characterise their observed variability features, both in relation to their photometric properties and the predictions from evolutionary and pulsation models. Of crucial importance is the correct identification of the actual pulsation modes involved in the observed PL sequences, a long debated topic. We present here a characterisation of the population of LPVs in the Magellanic Clouds. To do so, we make use of a large and improved grid of pulsation models, computed including updated opacity data for the specific composition of O- and C-rich stars. Pulsation models are combined with a population synthesis tool to simulate a population of evolved red giant variables. Models are compared with observational data from the OGLE-III Catalogue of Variable Stars, allowing us to provide a consistent interpretation of the observed PL sequences. We discuss some of the possibilities related to the use of pulsation models and observed pulsation properties to assist the calibration of stellar evolutionary models. Some of the issues involved in the theoretical modelling of pulsation in evolved red giants are also discussed.
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="seminar_geneve"
      handle="(2018)"
      title="Genève — Seminar @ Observatoire Astronomique">
      <Talk
        eventTitle="Invited Seminar"
        eventSubtitle="Astronomical Observatory - Department of Astronomy, Geneva University"
        eventLocation="Genève (Switzerland)"
        eventUrl=""
        talkTitle="New Pulsation Models of AGB Stars - Exploiting the Potential of Long-Period Variables"
        talkType=""
        eventImagePath="/images/talk-bg.jpg"
        talkPdfPath=""
        flexDir="row-reverse"
        >
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="lssteu3"
      handle="(2018)"
      title="Lyon — LSST@Europe 3">
      <Talk
        eventTitle="LSST@Europe 3"
        eventSubtitle="Large Synoptic Survey Telescope - Building Science Collaborations"
        eventLocation="Maison Internationale des Langues et des Cultures, Lyon (France)"
        eventUrl="https://indico.in2p3.fr/event/16341/"
        talkTitle="Long-Period Variables as Seen by LSST"
        talkType="Contributed Talk"
        eventImagePath="/images/lsst-europe-3.jpg"
        talkPdfPath="/files/talk_trabucchi_lyon2018.pdf"
        flexDir="row"
        >
      </Talk>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="beijing_2017"
      handle="(2017)"
      title="Beijing — Stellar Populations and the Distance Scale">
      <Talk
        eventTitle="Stellar Populations and the Distance Scale"
        eventSubtitle="A Conference in Honour of Jeremy Mould"
        eventLocation="Kavli Institute for Astronomy and Astrophysics, Peking University, Beijing (China)"
        eventUrl="http://kiaa.pku.edu.cn/info/1026/5177.htm"
        talkTitle="Characterization of Long-Period Variables in the Magellanic Clouds"
        talkType="Contributed Talk"
        eventImagePath="/images/beijing-2017.jpg"
        talkPdfPath="/files/talk_trabucchi_beijing2017.pdf"
        flexDir="row-reverse"
        >
      </Talk>
    </AccordionPanel>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .link {
    text-decoration: underline;
    text-decoration-style: dotted;
    color: inherit;
  }
  .title {
    padding: 30px 0 0 0;
    font-size: 32pt;
    font-family: 'Ubuntu';
    font-style: normal;
    font-weight: 400;
    color: #df7366;
    margin-bottom: 30px;
  }
  .content {
    padding: 0 0 30px 0;
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
  }
  .section-box {
    padding: 80px 10dvw;
    width: 100dvw;
    min-height: 100dvh;
    background-color: v-bind(bgcolor);
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }
</style>