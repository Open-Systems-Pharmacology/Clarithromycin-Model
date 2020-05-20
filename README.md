# Clarithromycin-Model
Whole-body PBPK model of clarithromycin. 

<a title="Clarithromycin" href="https://commons.wikimedia.org/wiki/File:Clarithromycin_structure.svg"><img width="256" alt="Clarithromycin structure" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Clarithromycin_structure.svg/256px-Clarithromycin_structure.svg.png"></a>


This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation-plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found [here](../../releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found [here](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**



Clarithromycin is a widely prescribed macrolide antibiotic and a substrate and mechanism-based inactivator of CYP3A4. Furthermore, clarithromycin is a substrate and inhibitor of P-gp and an inhibitor of OATP1B1 and OATP1B3. Clarithromycin has been proposed as one of the best alternative CYP3A4 inhibitors for clinical DDI studies to avoid further use of ketoconazole.

A whole-body PBPK model for clarithromycin was developed including its metabolism by CYP3A4 and its mechanism-based inactivation of the respective enzyme as well as its inhibition of P-gp.

The presented clarithromycin model was developed by Moj et al. [[1](#References)] and revised by Hanke et al. [[2](#References)].

## Code of conduct
Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution
We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License
The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] [Moj D, Hanke N, Britz H, Frechen S, Kanacher T, Wendl T, Haefeli WE, Lehr T. Clarithromycin, Midazolam, and Digoxin: Application of PBPK Modeling to Gain New Insights into Drug-Drug Interactions and Co-medication Regimens. AAPS J. 2017 Jan;19(1):298-312.](https://dx.doi.org/10.1208/s12248-016-0009-9)

[2] [Hanke N, Frechen S, Moj D, Britz H, Eissing T, Wendl T, Lehr T. PBPK models for CYP3A4 and P-gp DDI prediction: a modeling network of rifampicin, itraconazole, clarithromycin, midazolam, alfentanil and digoxin. CPT Pharmacometrics Syst Pharmacol. 2018 Oct;7(10):647-659.](https://ascpt.onlinelibrary.wiley.com/doi/abs/10.1002/psp4.12343)
