#SysML Modelling Workshop Meeting Minutes
* Location: Alstom, Charleroi
* Duration: 22.10. - 25.10. 2013
* Minutes taken by: Bernd Hekele (only highlights and decisions)
* Participants:
  * Alstom Belgium: Valerio Raimondi, Stephane Besure, Nicolas Boverie, Nicolas Moussine-Pouchkine (conclusion only)
  * Alstom France: Christian Girano
  * CETIC: Yeann Guyot
  * DB: Baseliyos Jacob (not 23rd), Bernd Hekele
  * Lloyds Register: Jan Welvaarts
  * NS: Jos Holtzer (22nd only)
  * SNCF: Sylvain Baro
  * Siemens: Niklas Schaffrath, Uwe Steinke
  * Systerel: Marielle Petit-Doche
  * TU-BS: Jan Welte (not 22nd)

#### Tuesday October 22nd 2013

* Sessions:
  * 9h00 – 9h15: Welcome and Introduction (V. Raimondi)
  * 9h15 – 10h00: SSRS Working Group Outcomes (J. Welvaarts) ==> [presentation](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/2013-10-22 functional analysis of the ERA SRS.pdf)
  * 10h00 – 11h30 : Siemens’s Proposal (U. Steinke) ==> [presentation](FunctionalStructure/ETCS_OBU_FunctionalStructure.pdf)
  * 11h30 – 13h00 : ALSTOM’s Proposal (S. Besure) ==> [presentation](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/AlstomFunctionalModelling.pdf)
  * 14h00 – 14h15 : ERTMS DB’s Roadmap (OpenETCS, ICE-T, …) (B. Jacob) ==> [presentation](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/20131021_SRS%20Aanalyse%20Workshop_22_10_2013_BJV01.pdf)
  * 14h15 – 15h15 : Siemens’s Proposal (U. Steinke) ==> [presentation](Charleroi-Workshop-20131022-25/SiemensAPI-20131322.pdf)
  * 15h15 – 16h15 : ALSTOM’s Proposal (N. Boverie) ==> [presentation](Charleroi-Workshop-20131022-25/ALSTOM OETCS API presentation 2013_10_22.pdf)
  * 16h15 – 17h30   : Analysis of the convergence(s) and/or difference(s) between presented proposals
  * 17h30 – 18h00   : Open Discussion on organization for next days work

* **Findings**
  * We agreed to not make use of interrupts in the Kernel
  * Interrupts are only allowed when working with software close to hardware
  * For the software design a data-centred approach is agreed
  * We agree on a cyclic Software Design:
    * At beginning of the processing we handle input data
    * Good description of data kept in Data Stores 
    * Multiple functions are executed in a predefined order
  * We limit our scope to the functionality defined in the ERA documents (e.g., no contry-specific items in focus)
  * We start from scratch. But, we take into account as much as possible from available results.
  * The functional breakdown ahown by Alstom, Siemens and the SSRS team shows close similarities. We need to decide on a common functional breakdown for openETCS.
  * Customer view on openETCS: Most important use-case Level 2; Limited Supervision

####   Wednesday October 23rd 2013

* Sessions:
  * Getting started with SysML (Marielle Petit-Doche)
  * ProR Overview and Model Evaluation
  * Teamwork Analysis of Function "3.6.6 Geographical position reporting"
    * Ranked as Low Effort"
  * Step 1: [Operational Analysis](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/WP_20131023_001.jpg)
  * Step 2: [Data Stores and Functions](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/WP_20131023_003.jpg)
  * Result: [Functional Analysis, Data Definition](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/GeographicalPosition.docx)

* **Findings**
  * If the allocation of a function to a unit is not unique, the allocation of SIL 4 parts shall be in the Kernel, Non-Sil4 functions in other units (e.g., DMI).
  * Keep kernel as small as possible
  * Template for Analysis: [==>](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/Template.docx)
  * Performance Evaluations are part of the analysis work.
  
####   Thursday October 24th 2013   
* Sessions:
  * Group Work in smaller multi-functional teams to proof process:
    * [Manage TSR](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/3-11-5-Manage-TSR.docx) 
    * [Display Text Message](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/DisplayTextMessagesComingFromTrackside.docx)
    * [Manage National Values](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/ManageNationalValues.docx)
    * [Route Suitability Supervision](https://github.com/openETCS/SRS-Analysis/blob/master/System%20Analysis/RouteSuitabilitySupervision.docx)
  * In parallel, the set of [functions](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/Functional_breakdown_list_131024_PIC.xls) have been reviewed and agreed on in an expert Session (Alstom/Siemens)
  
####   Friday October 25th 2013 
* 9h00 – 9h15 : Welcome and Introduction
* 9h15 – 11h00    : Sharing and organisation of work (for next 2 weeks) based on agreed functional structure and available ressources (Who is doing what when ?)
* 11h00 – 12h00   : Conclusion (V. Raimondi/Nicolas Moussine-Pouchkine)

* Findings: 
  * Team Definition is part of the [Functional Breakdown](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/Functional_breakdown_list_131024_PIC.xls)
  * [Agreed Action Items](https://github.com/openETCS/SRS-Analysis/blob/master/Charleroi-Workshop-20131022-25/OpenETCS_WP3_TF_MoMs_2013W43_01.pdf)
  