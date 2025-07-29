# Battery-Analysis
Lithium-ion batteries are composed of two electrodes—anode and cathode—along with an electrolyte and a separator. To understand the electrochemical behavior and degradation patterns over the life of a battery, it is critical to analyze both the individual electrodes and the full-cell performance at various stages of life: Beginning of Life (BOL) and End of Life (EOL).
In this study, we used a set of benchmark datasets that provide individual half-cell measurements and full-cell measurements for a lithium-ion cell over thousands of cycles. The aim is to visualize and analyze how various metrics such as voltage vs. state of charge (SoC) and dV/dSoC vs. SoC change from BOL to EOL, which provides insight into the degradation mechanism and capacity fade over time.
Data Used
We analyzed the following four datasets:

an_T23_C_24_dis.csv
This file contains anode half-cell data during discharge. It has columns for state of charge (SoC) and the corresponding voltage. It reflects how the anode voltage responds to SoC changes.
ca_T23_C_6_ch.csv
This file provides cathode half-cell data during charge. It helps us understand how the cathode behaves electrochemically, especially how voltage changes with SoC.
charge2.csv
This dataset represents the full-cell behavior at the Beginning of Life (BOL). It includes SoC, voltage, and computed derivatives such as dSoC/dV and dV/dSoC. This is a benchmark reference to understand the battery’s pristine performance.
charge3866.csv
This file captures the full-cell data at the End of Life (EOL) after extensive cycling. By comparing this with BOL data, we observe degradation in battery characteristics.
Voltage vs. SoC (for Anode, Cathode, Full Cell BOL and EOL)
We plotted voltage vs. SoC curves for all four datasets to understand how the voltage profile evolves with state of charge:
• The anode and cathode half-cells show individual electrode behavior.
• The full-cell at BOL (charge2) shows the original voltage response.
• The full-cell at EOL (charge3866) helps visualize capacity loss or shifts in voltage profiles.
dV/dSoC vs. SoC (for Full Cell BOL and EOL)
The derivative dV/dSoC helps amplify small changes in voltage response to SoC, making it easier to:
• Detect phase transitions and reactions occurring inside the battery.
• Identify SoC ranges where degradation has impacted voltage response.
• Pinpoint flattening or steepening of curves which is a sign of electrode aging.
The comparative plot between BOL and EOL shows that peaks flatten or shift, indicating a loss of capacity, increased resistance, and possibly lithium plating or loss of cyclable lithium
Why Benchmarking ?
Using benchmark data from a trusted source like NREL allows us to:
• Validate our analysis against known performance standards.
• Ensure that the dQ/dV and dV/dSoC plots we generate are consistent with real-world electrochemical behavior.
• Use the BOL data as a baseline to compare degradation at the EOL state and draw meaningful inferences
Markdown Editor
Markdown input: edit mode selected.
Write
Preview
