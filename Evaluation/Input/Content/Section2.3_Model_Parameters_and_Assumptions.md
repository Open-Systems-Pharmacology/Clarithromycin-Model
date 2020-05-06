### 2.3.1	Absorption

The specific intestinal permeability was optimized during parameter identification to accurately describe the absorption of clarithromycin after oral administration.

### 2.3.2	Distribution

Values for lipophilicity and fraction unbound in plasma were fixed to literature values (namely to 2.3 ([Lappin 2011](#5-References)) and 0.30 ([Chu 1993b](#5-References)) for lipophilicity and fraction unbound, respectively). 

It was not possible to adequately describe the observed plasma concentration-time profile after intravenous administration using standard input parameters (e.g. lipophilicity) and calculation methods. Simulated concentration-time profiles overestimated C<sub>max</sub> and underestimated the observed data for time to C<sub>max</sub> (T<sub>max</sub>). According to literature data, clarithromycin accumulates in mononuclear and polymorphonuclear leukocytes, probably via active transport ([Ishiguro 1989](#5-References)). Implementing this process in the model improved the model fit significantly. Due to limited knowledge on this active transport, this process was technically implemented in the model by adjusting the permeability of clarithromycin across the membrane of the red blood cells (`P (blood cells->plasma)` and `P (plasma->blood cells)`). 

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard`. 

### 2.3.3	Metabolism and Elimination

Metabolism was described using Michaelis-Menten kinetics, while the Michaelis-Menten constant K<sub>m</sub> was taken from in-vitro experiments from literature and the turnover rate k<sub>cat</sub> was optimized during parameter identification. 

K<sub>I</sub> and k<sub>inact</sub> to describe the mechanism-based inhibition of CYP3A4 were optimized during parameter identification.

A kidney plasma clearance was implemented to describe the renal elimination of clarithromycin. The specific renal clearance was optimized during parameter identification.

### 2.3.4	Automated Parameter Identification

This is the result of the final parameter identification.

| Model Parameter                                 | Optimized Value | Unit   |
| ----------------------------------------------- | --------------- | ------ |
| `kcat` (CYP3A4)                                 | 76.5            | 1/min  |
| `Specific clearance` in process renal clearance | 0.87            | 1/min  |
| `Specific intestinal permeability`              | 1.23 E-6        | dm/min |
| `P (plasma->blood cells)`                       | 3.62 E-5        | dm/min |
| `P (blood cells->plasma)`                       | 1.04 E-6        | dm/min |
| `K_kinact_half` (K<sub>I</sub>)                 | 6.04            | µmol/L |
| `kinact` (k<sub>inact</sub>)                    | 0.04            | 1/min  |

