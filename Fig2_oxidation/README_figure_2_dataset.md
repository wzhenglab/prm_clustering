# Figure 2 Dataset

## Description

`figure_2_oxidation_assay.csv` contains the underlying experimental data
used to generate Figure 2 of the manuscript. The dataset reports
time-course measurements of dioxane, tetrahydrofuran (THF), and propane
during oxidation assays with E11 PRM-II and ENV421 PRM-III, together
with the corresponding abiotic blank and biotic empty-vector controls.

Each row represents an individual experimental measurement. Replicate
measurements are retained as separate rows.

## Column descriptions

  -----------------------------------------------------------------------
  Column                              Description
  ----------------------------------- -----------------------------------
  `prm`                               PRM treatment or control used in
                                      the oxidation assay. `e11` denotes
                                      E11 PRM-II; `env421` denotes ENV421
                                      PRM-III; `control_abiotic_blank`
                                      denotes the abiotic blank; and
                                      `control_biotic_empty_vector`
                                      denotes the biotic control
                                      containing the empty pTip-QC2
                                      vector.

  `substrate`                         Substrate measured in the assay:
                                      `dioxane` = 1,4-dioxane, `thf` =
                                      tetrahydrofuran, and `propane` =
                                      propane.

  `time`                              Sampling time during the oxidation
                                      assay, in hours (h).

  `concentration_mM`                  Measured substrate concentration at
                                      the indicated sampling time, in
                                      millimolar (mM; mmol/L).
  -----------------------------------------------------------------------

## Notes

-   Experimental replicate measurements are provided individually rather
    than as means.
-   The data can therefore be used to independently calculate summary
    statistics or reproduce the time-course plots presented in Figure 2.
