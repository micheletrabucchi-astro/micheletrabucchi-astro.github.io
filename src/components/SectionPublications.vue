<script setup>
  import AccordionPanel from './AccordionPanel.vue';
  import Paper from './Paper.vue';  
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
      aria-title="trabucchi_2024"
      handle="(2024)"
      title="Long-Period Variables as distance and age indicators in the era of Gaia and LSST">
      <Paper
        authors="Trabucchi, M."
        bibinfo="2024 •​​ Proceedings of the IAU, S376, 306T"
        adsurl="https://ui.adsabs.harvard.edu/abs/2024IAUS..376..306T/abstract"
        imagePath="/images/trabucchi_2024.png"
        pdfPath="/files/Trabucchi_2024_ProceedingsIAU_S376_306T.pdf"
        flexDir="row-reverse"
        >
        Long-period variables are bright, evolved red giant stars showing periodic photometric changes due to stellar pulsation. They follow one or more period-luminosity and period-age relations, which make them highly promising distance indicators and tracers of young and intermediate-age stellar populations. Such a potential is especially interesting in view of the massive amount of data delivered by modern large-scale variability surveys. Crucially, these applications require a clear theoretical understanding of pulsation physics in connection with stellar evolution. Here, I describe an ongoing effort from our collaboration dedicated to the modelling of stellar pulsation in evolved stars, and how this work is impacting our capability of investigating long-period variables and exploiting them for other astrophysical studies. Furthermore, I present our ongoing work aimed at assessing the potential of semi-regular variables, an often neglected sub-type of long-period variables, to be distance indicators complementary to their better-known, more evolved counterparts, the Mira variables.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="pawlak_trabucchi_eyer_mowlavi_2024"
      handle="(2024)"
      title="Investigating the long secondary period phenomenon with the ASAS-SN and Gaia data">
      <Paper
        authors="Palwak, M.; Trabucchi, M.; Eyer, L. & Mowlavi, N."
        bibinfo="2024 •​​ A&A, 682:A88"
        adsurl="https://ui.adsabs.harvard.edu/abs/2024A%26A...682A..88P/abstract"
        imagePath="/images/pawlak_trabucchi_eyer_mowlavi_2024.png"
        pdfPath="/files/Pawlak_Trabucchi_Eyer_Mowlavi_2024_A&A_682_A88.pdf"
        >
        Period–luminosity (PL) sequences of long-period variables (LPVs) are commonly interpreted as different pulsation modes, but there is disagreement on the modal assignment. Here, we re-examine the observed PL sequences in the Large Magellanic Cloud, including the sequence of long secondary periods (LSPs), and their associated pulsation modes. First, we theoretically model the sequences using linear, radial, nonadiabatic pulsation models and a population synthesis model of the LMC red giants. Then, we use a semi-empirical approach to assign modes to the pulsation sequences by exploiting observed multi-mode pulsators. As a result of the combined approaches, we consistently ﬁnd that sequences B and C′ both correspond to ﬁrst overtone pulsation, although there are some fundamental mode pulsators at low luminosities on both sequences. The masses of these fundamental mode pulsators are larger at a given luminosity than the mass of the ﬁrst overtone pulsators. These two sequences, B and C′, are separated by a small period interval in which large amplitude pulsation in a long secondary period (sequence D variability) occurs, meaning that the ﬁrst overtone pulsation is not seen as the primary mode of pulsation. Observationally, this leads to the splitting of the ﬁrst overtone pulsation sequence into the two observed sequences, B and C′. Our two independent examinations also show that sequences A′, A, and C correspond to third overtone, second overtone, and fundamental mode pulsation, respectively.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="gaia_fpr_2023"
      handle="(2023)"
      title="Gaia Focused Product Release: Radial velocity time series of long-period variables">
      <Paper
        authors="Gaia Collaboration: Trabucchi, M.; Mowlavi, N.; Lebzelter, T.; Lecoeur-Taïbi, I. et al."
        bibinfo="2023 •​​ A&A, 680:A36"
        adsurl="https://ui.adsabs.harvard.edu/abs/2023A%26A...680A..36G/abstract"
        imagePath="/images/gaia_fpr_2023.png"
        pdfPath="/files/GaiaCollaboration_Trabucchi_Mowlavi_Lebzelter_etal_2023_A&A_680_A36.pdf"
        flexDir="row-reverse"
        >
        Period–luminosity (PL) sequences of long-period variables (LPVs) are commonly interpreted as different pulsation modes, but there is disagreement on the modal assignment. Here, we re-examine the observed PL sequences in the Large Magellanic Cloud, including the sequence of long secondary periods (LSPs), and their associated pulsation modes. First, we theoretically model the sequences using linear, radial, nonadiabatic pulsation models and a population synthesis model of the LMC red giants. Then, we use a semi-empirical approach to assign modes to the pulsation sequences by exploiting observed multi-mode pulsators. As a result of the combined approaches, we consistently ﬁnd that sequences B and C′ both correspond to ﬁrst overtone pulsation, although there are some fundamental mode pulsators at low luminosities on both sequences. The masses of these fundamental mode pulsators are larger at a given luminosity than the mass of the ﬁrst overtone pulsators. These two sequences, B and C′, are separated by a small period interval in which large amplitude pulsation in a long secondary period (sequence D variability) occurs, meaning that the ﬁrst overtone pulsation is not seen as the primary mode of pulsation. Observationally, this leads to the splitting of the ﬁrst overtone pulsation sequence into the two observed sequences, B and C′. Our two independent examinations also show that sequences A′, A, and C correspond to third overtone, second overtone, and fundamental mode pulsation, respectively.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="gaia_dr3_2023"
      handle="(2023)"
      title="Gaia Data Release 3. The second Gaia catalogue of long-period variable candidates">
      <Paper
        authors="Lebzelter, T.; Mowlavi, N.; Lecoeur-Taïbi, I.; Trabucchi, M. et al."
        bibinfo="2023 •​​ A&A, 674:A15"
        adsurl="https://ui.adsabs.harvard.edu/abs/2023A%26A...674A..15L/abstract"
        imagePath="/images/gaia_dr3_2023.png"
        pdfPath="/files/Lebzelter_Mowlavi_LecoeurTaibi_Trabucchi_etal_2023_A&A_674_A15.pdf"
        >
        Context. The third Gaia Data Release covers 34 months of data and includes the second Gaia catalogue of long-period variables (LPVs), with G variability amplitudes larger than 0.1 mag (5-95% quantile range).
        Aims: The paper describes the production and content of the second Gaia catalogue of LPVs and the methods we used to compute the published variability parameters and identify C-star candidates.
        Methods: We applied various filtering criteria to minimise contamination from variable star types other than LPVs. The period and amplitude of the detected variability were derived from model fits to the G-band light curve wherever possible. C stars were identified using their molecular signature in the low-resolution RP spectra.
        Results: The catalogue contains 1 720 558 LPV candidates, including 392 240 stars with published periods (ranging from 35 to ∼1000 days) and 546 468 stars classified as C-star candidates. Comparison with literature data (OGLE and ASAS-SN) leads to an estimated completeness of 80%. The recovery rate is about 90% for the most regular stars (typically miras) and 60% for SRVs and irregular stars. At the same time, the number of known LPVs is increased by a factor of 6 with respect to literature data for amplitudes larger than 0.1 mag in G, and the contamination is estimated to be below 2%. Our C-star classification, based on solid theoretical arguments, is consistent with spectroscopically identified C stars in the literature. Caution must be taken in crowded regions, however, where the signal-ro-noise ratio of the RP spectra can become very low, or if the source is reddened by some kind of extinction. The quality and potential of the catalogue are illustrated by presenting and discussing LPVs in the solar neighbourhood, in globular clusters, and in galaxies of the Local Group.
        Conclusions: This is the largest all-sky LPVs catalogue to date. The photometric depth reaches G = 20 mag. This is a unique dataset for research into the late stages of stellar evolution.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="trabucchi_mowlavi_2022"
      handle="(2022)"
      title="The period-age relation of long-period variables">
      <Paper
        authors="Trabucchi, M. & Mowlavi, N."
        bibinfo="2022 •​​ A&A, 658:A1"
        adsurl="https://ui.adsabs.harvard.edu/abs/2022A%26A...658L...1T/abstract"
        imagePath="/images/trabucchi_mowlavi_2022.png"
        pdfPath="/files/Trabucchi_Mowlavi_2022_A&A_658_L1.pdf"
        flexDir="row-reverse"
        >
        Context. Pieces of empirical evidence suggest the existence of a period-age relation for long-period variables (LPVs). Yet, this property has hardly been studied on theoretical grounds thus far.
        Aims: We aim to examine the period-age relation using the results from recent nonlinear pulsation calculations.
        Methods: We combined isochrone models with theoretical periods to simulate the distribution of fundamental mode LPV pulsators, which include Miras, in the period-age plane, and we compared it with observations of LPVs in Galactic and Magellanic Clouds' clusters.
        Results: In agreement with observations, models predict that the fundamental mode period decreases with increasing age because of the dominant role of mass in shaping stellar structure and evolution. At a given age, the period distribution shows a non-negligible width and is skewed toward short periods, except for young C-rich stars. As a result, the period-age relations of O-rich and C-rich models are predicted to have different slopes. We derived best-fit relations describing age and initial mass as a function of the fundamental mode period for both O- and C-rich models.
        Conclusions: The study confirms the power of the period-age relations to study populations of LPVs of specific types, either O-rich or C-rich, on statistical grounds. In doing so, it is recommended not to limit a study to Miras, which would make it prone to selection biases, but rather to include semi-regular variables that pulsate predominantly in the fundamental mode. The use of the relations to study individual LPVs, on the other hand, requires more care given the scatter in the period distribution predicted at any given age.
        </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="trabucchi_mowlavi_lebzelter_2021"
      handle="(2021)"
      title="Semi-regular red giants as distance indicators. I. The period-luminosity relations of semi-regular variables revisited">
      <Paper
        authors="Trabucchi, M; Mowlavi, N. & Lebzelter, T."
        bibinfo="2021 •​​ A&A, 656:A66"
        adsurl="https://ui.adsabs.harvard.edu/abs/2021A%26A...656A..66T/abstract"
        imagePath="/images/trabucchi_mowlavi_lebzelter_2021.png"
        pdfPath="/files/Trabucchi_Mowlavi_Lebzelter_2021_A&A_656_A66.pdf"
        >
        Context. Semi-regular variables (SRVs) are similar to Miras in brightness, and they also follow one or more period-luminosity relations (PLRs), though not necessarily the same one as Miras. As potential standard candles they are more challenging than Miras because of their smaller variability amplitudes and less regular light curves, but they are substantially more numerous and especially promising for probing old stellar populations.
        Aims: We aim to characterise the variability of SRVs, specifically focusing on their connection with Miras, in order to prepare the ground for investigating their potential as distance indicators.
        Methods: We examine SRVs and Miras in the Magellanic Clouds from OGLE-III observations, with data from Gaia and 2MASS. After cleaning the sample of variability periods unrelated to pulsation, we classify each source by chemical type and combination of pulsation modes. We examine the results in terms of global photometric and pulsation properties.
        Results: We identify four SRV groups that fit the general evolutionary scenario predicted by theory. SRVs dominated by fundamental-mode pulsation are very similar to Miras, especially if mono-periodic. They further split into two subgroups, one of which follows the same sequence as Miras in the period-luminosity and period-amplitude diagrams, without discontinuity.
        Conclusions: The similarities between Miras and SRVs suggest that the latter can be adopted as distance indicators in a way that is complementary to the use of the former, thereby at least doubling the available number of long-period variables (LPVs) suitable for use as distance indicators. The traditional amplitude-based separation between Miras and SRVs is not necessarily appropriate, and a more physically sound criterion should also involve pulsation periods. While this would require comparatively longer time-series, they are expected to become accessible in the coming years even for weak sources thanks to current and future large-scale surveys. The table of reclassified LPVs is made public.
        </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="trabucchi_etal_2021"
      handle="(2021)"
      title="Modelling long-period variables - II. Fundamental mode pulsation in the non-linear regime">
      <Paper
        authors="Trabucchi, M; Wood, P. R.; Mowlavi, N.; Pastorelli, G.; Marigo, P.; Girardi, L. & Lebzelter, T."
        bibinfo="2021 •​​ MNRAS, 500:1575"
        adsurl="https://ui.adsabs.harvard.edu/abs/2021MNRAS.500.1575T/abstract"
        imagePath="/images/trabucchi_etal_2021.png"
        pdfPath="/files/Trabucchi_etal_2021_MNRAS_500_1575.pdf"
        flexDir="row-reverse"
        >
        Context. Semi-regular variables (SRVs) are similar to Miras in brightness, and they also follow one or more period-luminosity relations (PLRs), though not necessarily the same one as Miras. As potential standard candles they are more challenging than Miras because of their smaller variability amplitudes and less regular light curves, but they are substantially more numerous and especially promising for probing old stellar populations.
        Aims: We aim to characterise the variability of SRVs, specifically focusing on their connection with Miras, in order to prepare the ground for investigating their potential as distance indicators.
        Methods: We examine SRVs and Miras in the Magellanic Clouds from OGLE-III observations, with data from Gaia and 2MASS. After cleaning the sample of variability periods unrelated to pulsation, we classify each source by chemical type and combination of pulsation modes. We examine the results in terms of global photometric and pulsation properties.
        Results: We identify four SRV groups that fit the general evolutionary scenario predicted by theory. SRVs dominated by fundamental-mode pulsation are very similar to Miras, especially if mono-periodic. They further split into two subgroups, one of which follows the same sequence as Miras in the period-luminosity and period-amplitude diagrams, without discontinuity.
        Conclusions: The similarities between Miras and SRVs suggest that the latter can be adopted as distance indicators in a way that is complementary to the use of the former, thereby at least doubling the available number of long-period variables (LPVs) suitable for use as distance indicators. The traditional amplitude-based separation between Miras and SRVs is not necessarily appropriate, and a more physically sound criterion should also involve pulsation periods. While this would require comparatively longer time-series, they are expected to become accessible in the coming years even for weak sources thanks to current and future large-scale surveys. The table of reclassified LPVs is made public.
        </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="lebzelter_trabucchi_mowlavi_etal_2019"
      handle="(2019)"
      title="Period-luminosity diagram of long period variables in the Magellanic Clouds. New aspects revealed from Gaia Data Release 2">
      <Paper
        authors="Lebzelter, T.; Trabucchi, M; Mowlavi, N.; Wood, P. R.; Marigo, P.; Pastorelli, G. & Lecoeur-Taïbi, I."
        bibinfo="2019 •​​ A&A, 631:A24"
        adsurl="https://ui.adsabs.harvard.edu/abs/2019A%26A...631A..24L/abstract"
        imagePath="/images/lebzelter_trabucchi_mowlavi_etal_2019.png"
        pdfPath="/files/Lebzelter_Trabucchi_Mowlavi_etal_2019_A&A_631_A24.pdf"
        >
        Context. The period-luminosity diagram (PLD) has proven to be a powerful tool for studying populations of pulsating red giants. Gaia Data Release 2 (DR2) provides a large data set including many long-period variables (LPVs) on which this tool can be applied.
        Aims: We investigate the location of LPVs from the Large and Small Magellanic Clouds in the PLD using various optical and infrared luminosity indicators from Gaia and 2MASS, respectively. We thereby distinguish between stars of different masses and surface chemistry.
        Methods: The data set taken from the Gaia DR2 catalogue of LPVs allows for a homogeneous study from low- to high-mass LPVs. These sources are divided into sub-populations of asymptotic giant branch (AGB) stars according to their mass and their O- or C-rich nature using the Gaia-2MASS diagram developed by our group. This diagram uses a Wesenheit index WBP, RP based on Wesenheit functions in the Gaia and 2MASS photometric bands. Four different luminosity indicators are used to study the period-luminosity (P-L) relations.
        Results: We provide the first observational evidence of a P-L relation offset for both fundamental and 1O pulsators between low- and intermediate-mass O-rich stars, in agreement with published pulsation predictions. Among the luminosity indicators explored, sequence C' is the narrowest in the P-WBP, RP diagram, and is thus to be preferred over the other PLDs for the determination of distances using LPVs. The majority of massive AGB stars and red supergiants form a smooth extension of sequence C of low- and intermediate-mass AGB stars in the P-WBP, RP diagram, suggesting that they pulsate in the fundamental mode. All results are similar in the two Magellanic Clouds.
        </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="mcdonald_trabucchi_2019"
      handle="(2019)"
      title="The onset of the AGB wind tied to a transition between sequences in the period-luminosity diagram">
      <Paper
        authors="McDonald, I. & Trabucchi, M."
        bibinfo="2019 •​​ MNRAS — 484:4678"
        adsurl="https://ui.adsabs.harvard.edu/abs/2019MNRAS.484.4678M/abstract"
        imagePath="/images/mcdonald_trabucchi_2019.png"
        pdfPath="/files/McDonald_Trabucchi_2019_MNRAS_484_4678.pdf"
        flexDir="row-reverse"
        >
        We link the onset of pulsation-enhanced, dust-driven winds from asymptotic giant branch (AGB) stars in the Magellanic Clouds to the star's transition between period-luminosity sequences (from B to C'). This transition occurs at ∼60 d for solar-mass stars, which represent the bulk of the AGB population: this is the same period at which copious dust production starts in solar-neighbourhood AGB stars. It is contemporaneous with the onset of long secondary period (LSP) variability on sequence D. The combined amplitude of the first-overtone (B + C') and fundamental (C) modes and (perhaps) long-secondary period (D; LSP) variability appears to drive a sudden increase in mass-loss rate to a stable plateau, previously identified to be a few ×10-7 M⊙ yr-1. We cite this as evidence that pulsations are necessary to initiate mass-loss from AGB stars and that these pulsations are significant in controlling stars' mass-loss rates. We also show evidence that LSPs may evolve from long to short periods as the star evolves, counter to the other period-luminosity sequences.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="trabucchi_etal_2019"
      handle="(2019)"
      title="Modelling long-period variables – I. A new grid of O-rich and C-rich pulsation models">
      <Paper
        authors="Trabucchi, M.; Wood, P. R.; Montalbán, J.; Marigo P.; Pastorelli G. & Girardi, L."
        bibinfo="2019 •​​ MNRAS — 482:929"
        adsurl="https://ui.adsabs.harvard.edu/abs/2019MNRAS.482..929T/abstract"
        imagePath="/images/trabucchi_etal_2019.png"
        pdfPath="/files/Trabucchi_etal_2019_MNRAS_482_929.pdf"
        >
        We present a new grid of non-adiabatic, linear pulsation models of long-period variables (LPVs), including periods and growth rates for radial modes from the fundamental to the fourth overtone. The models span a wide range in mass, luminosity, metallicity, C/O ratio, and helium abundance, effectively covering the whole thermally pulsing asymptotic giant branch (TP-AGB) evolution, and representing a significant update with respect to previous works. The main improvement is the inclusion of detailed atomic and molecular opacities, consistent with the models chemical mixture, that makes the present set of models the first to systematically account for variability in C-stars. We examine periods and growth rates in the models, and find that, while the fundamental mode is affected by the structure of the envelope, overtones are less sensitive to the interior and largely determined by the global properties. In the models, the frequency of the overtone with the largest degree of excitation is found to scale with the acoustic cut-off frequency at the stellar surface, a behaviour similar to that observed for the frequency of maximum oscillation power for solar-like oscillations in less evolved red giants. This allows us to provide a simple analytic prescription to predict the most-likely dominant mode as a function of stellar parameters. Best-fitting relations for periods are also provided. By applying results of pulsation models to evolutionary tracks, we present a general picture of the evolution of long-period variability during the TP-AGB, that we find consistent with observations. Models are made public through a dedicated web interface.
      </Paper>
    </AccordionPanel>
    <!--  -->
    <AccordionPanel
      aria-title="trabucchi_etal_2017"
      handle="(2017)"
      title="A New Interpretation of the Period–Luminosity Sequences of Long-period Variables">
      <Paper
        authors="Trabucchi, M.; Wood, P. R.; Montalbán, J.; Marigo P.; Pastorelli G. & Girardi, L."
        bibinfo="2017 •​​ ApJ — 847:139"
        adsurl="https://ui.adsabs.harvard.edu/abs/2017ApJ...847..139T/abstract"
        imagePath="/images/trabucchi_etal_2017.png"
        pdfPath="/files/Trabucchi_etal_2017_ApJ_847_139.pdf"
        flexDir="row-reverse"
        >
        Period–luminosity (PL) sequences of long-period variables (LPVs) are commonly interpreted as different pulsation modes, but there is disagreement on the modal assignment. Here, we re-examine the observed PL sequences in the Large Magellanic Cloud, including the sequence of long secondary periods (LSPs), and their associated pulsation modes. First, we theoretically model the sequences using linear, radial, nonadiabatic pulsation models and a population synthesis model of the LMC red giants. Then, we use a semi-empirical approach to assign modes to the pulsation sequences by exploiting observed multi-mode pulsators. As a result of the combined approaches, we consistently ﬁnd that sequences B and C′ both correspond to ﬁrst overtone pulsation, although there are some fundamental mode pulsators at low luminosities on both sequences. The masses of these fundamental mode pulsators are larger at a given luminosity than the mass of the ﬁrst overtone pulsators. These two sequences, B and C′, are separated by a small period interval in which large amplitude pulsation in a long secondary period (sequence D variability) occurs, meaning that the ﬁrst overtone pulsation is not seen as the primary mode of pulsation. Observationally, this leads to the splitting of the ﬁrst overtone pulsation sequence into the two observed sequences, B and C′. Our two independent examinations also show that sequences A′, A, and C correspond to third overtone, second overtone, and fundamental mode pulsation, respectively.
      </Paper>
    </AccordionPanel>
  </div>
</template>
<!-- ####################################################################### -->
<style scoped>
  .link {
    text-decoration: underline;
    /* text-decoration-thickness: 1px; */
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
    /* background-color: rgba(255, 255, 255, 1); */
    background-color: v-bind(bgcolor);
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }
</style>