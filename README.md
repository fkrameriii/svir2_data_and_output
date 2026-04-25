```
"Simulation Data.xlsx" is the master file for the simulation output
    Worksheet "Simulation Results - S2" is the main worksheet
        Each row corresponds to a simulation scenario that was conceived at the beginning
            Many were not run or deemed unnessary as the simulation process began
            Additional scenarios were added to the end
                  No rows were deleted or cleaned up, even if not run
                      This is because each row corresponds to <row>.png files for easy identification
            Rows were not removed even if they were no longer deemed necessary
            Rows correspond to the following scenarios:
                  Rows 3 - 182) Scenario 1
                  Rows 183 - 362) Scenario 2 PRIOR to the pivot to make Beta_V a variable parameter
                  Rows 363 - 497) Scenario 2 with Beta_C = 0.5, and Beta_V tested with values of 1, 0.5, and 0.75
                  Rows 498 - 502) Extending Scenario 1 to test a scenario where NO vaccination is available
                  Rows 503 - 517) Scenario 2 with Beta_C = 0.25, and Beta_V tested with values of 1, 0.25, and 0.625
        Each row corresponds to two images in the /images subfolder, that share the name of the row number
            <row>_full.png is the graphical simulation output showing all 8 states of the experimental model
            <row>_ic.png is the graphical simulation that shows only the infection curves:
                  1) Experimental model compliant infectious curve
                  2) Experimental model antagonist infectious curve
                  3) Experimental model TOTAL infectious curve (compliant + antagonist curves)
                  4) SVIR-A comparison infection curve
                  5) SVIR-C comparison infection curve
        Column Definitions:
            Columns A - J) Parameter values for each simulation
            Columns K - M) Simulation results for the Experimental model COMBINED infection curve
            Columns N - O) Simulation results for Experimental model Antagonist infection curve
            Columns P - Q) Simulation results for Experimental model Compliant infection curve
            Columns R - T) Simulation results for SVIR-A infection curve
            Columns U - W) Simulation results for SVIR-C infection curve

"*.CSV" files contain values extracted from "Simulation Data.xlsx" and condensed into a format that was easier to ingest into R 
for generating the results graphs that were included in the paper

/images/* are the .PNG files of the graphical output from the simulator 
that correspond to each simulation/row
    <row>_full.png is the graphical simulation output showing all 8 states of the experimental model
    <row>_ic.png is the graphical simulation that shows only the infection curves:
          1) Experimental model compliant infectious curve
          2) Experimental model antagonist infectious curve
          3) Experimental model TOTAL infectious curve (compliant + antagonist curves)
          4) SVIR-A comparison infection curve
          5) SVIR-C comparison infection curve
```
