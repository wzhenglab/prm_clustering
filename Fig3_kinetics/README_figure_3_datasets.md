# Figure 3 Kinetic Datasets

## Description

The Figure 3 kinetic data are provided in two files:

-   `figure_3_kinetic_ppm.csv` contains the substrate oxidation kinetic
    data used for the ppm-level kinetic analyses presented in Figure 3a
    and Figure 3b.
-   `figure_3_kinetic_ppb.csv` contains the low-concentration dioxane
    kinetic data at the ppb (µg/L) level.

Individual biological replicate measurements are retained as separate
rows.

## `figure_3_kinetic_ppm.csv`

This file contains kinetic measurements for dioxane and propane
oxidation by the indicated PRMs.

### Column descriptions

  -----------------------------------------------------------------------
  Column                              Description
  ----------------------------------- -----------------------------------
  `prm`                               PRM used in the kinetic assay.
                                      `ph06` denotes PH-06 PRM-I, `e11`
                                      denotes E11 PRM-II, and `env421`
                                      denotes ENV421 PRM-III.

  `substrate`                         Substrate used for the kinetic
                                      measurement: `dioxane` =
                                      1,4-dioxane and `propane` =
                                      propane.

  `group`                             Identifier for the nominal
                                      substrate-concentration group used
                                      to organize biological replicate
                                      measurements at the same target
                                      concentration. Rows with the same
                                      PRM, substrate, and group
                                      correspond to replicate
                                      measurements for that concentration
                                      level.

  `initial_substrate_concentration`   Measured initial substrate
                                      concentration. **Units depend on
                                      the substrate:** dioxane
                                      concentrations are reported in
                                      **mg/L (ppm)**, whereas propane
                                      concentrations are reported in **mM
                                      (mmol/L)**.

  `velocity`                          Initial linear substrate oxidation
                                      velocity. For dioxane,
                                      velocity is reported in **mg
                                      substrate/h/mg-protein**; for
                                      propane, velocity is reported in
                                      **µmol substrate/h/mg-protein**.

  -----------------------------------------------------------------------

## `figure_3_kinetic_ppb.csv`

This file contains low-concentration dioxane kinetic measurements at the
ppb level for E11 PRM-II and ENV421 PRM-III.

### Column descriptions

  ---------------------------------------------------------------------------
  Column                                  Description
  --------------------------------------- -----------------------------------
  `prm`                                   PRM used in the kinetic assay.
                                          `e11` denotes E11 PRM-II and
                                          `env421` denotes ENV421 PRM-III.

  `substrate`                             Substrate used for the kinetic
                                          measurement; all entries in this
                                          dataset are `dioxane`
                                          (1,4-dioxane).

  `group`                                 Identifier for the nominal
                                          dioxane-concentration group used to
                                          organize biological replicate
                                          measurements at the same target
                                          concentration.

  `initial_substrate_concentration_ppb`   Measured initial dioxane
                                          concentration in **µg/L (ppb)**.

  `velocity`                              Initial linear dioxane oxidation velocity
                                          reported in **µg/h/mg-protein**.

  ---------------------------------------------------------------------------

## Notes

-   Replicate measurements are provided individually rather than as
    averaged values.
-   The `group` column is an organizational identifier and is not itself
    a concentration value.
-   The ppm-level file uses a single `initial_substrate_concentration`
    column for both substrates; therefore, the substrate-specific units
    described above should be applied when interpreting this column.
