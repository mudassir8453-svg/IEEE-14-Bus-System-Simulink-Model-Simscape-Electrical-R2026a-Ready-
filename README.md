## Overview
A working IEEE 14-bus test system Simulink model for MATLAB R2026a and later, 
where Specialized Power Systems (SPS) support — including the `powergui` block — 
has been removed by MathWorks.

## What this is
This model is based on Bharath Yk's original *IEEE 14 Bus System Simulink Model* 
(File Exchange, first published 2014). That model, after the standard SPS-to-
Simscape conversion tools were applied, had only its Series RLC branches migrated — 
the synchronous generators, transformers, and synchronous compensator were left 
as unconverted SPS blocks and would not run at all once SPS was removed in R2026a.

This submission completes that conversion: every block is now native Simscape 
Electrical, with no SPS or powergui dependency anywhere in the model.

## Compatibility
- Tested on MATLAB R2026a
- No Specialized Power Systems (SPS) library required
- No powergui block

## How to use
1. Extract the .zip
2. Open the .slx file in MATLAB R2026a or later
3. Run the model — no additional setup required

## Acknowledgements
Based on Bharath Yk's *IEEE 14 Bus System Simulink Model* 
(https://www.mathworks.com/matlabcentral/fileexchange/46067-ieee-14-bus-system-simulink-model), 
with generator, transformer, and synchronous compensator blocks converted from 
Specialized Power Systems to Simscape Electrical.
