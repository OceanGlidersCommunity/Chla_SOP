(dmqc)=
# Delayed Mode Quality Control

Text

### Dark count re calibration

### Non photochemical quenching corrections

Fluorescence data has to be corrected for non-photochemical quenching (NPQ) in most cases. NPQ is a physiological response to high light environments used by plants and algae to protect themselves from damage and causes an evident weakening in fluorescence signal during the day (Müller et al. 2001). NPQ occurs only during the daytime or whenever light avaialbility is high, therefore when night measurements close in time and space are available, they can be used to correct daytime profiles. Different methods exist for NPQ the paper by Thomalla et al. (2018) provides a good overview on the various methodologies. 
The most suitable methodology will vary based on the study area as well as the research question. The assumptions and corrections of each method may not provide credible results for the diffent water column structures so the methodology has to be chosen carefully.

Shall we add the nice table from the Thomalla paper summrizing all the methodologes? I add the draft below

| Study  |  Equation | Assumptions | 
|---|---|---|
| Xing et al. (2012)  | 	C1 = max<sub>0≤z≤MLD</sub> (Fl(z)) <br> Flc(z) = C1; 0≤z≤d(C1)| - Fluorescence uniform within MLD  <br> - No quenching below max ﬂuorescence within MLD |
| Biermann et al. (2015) |  C2 = max<sub>0≤z≤ED</sub> (Fl(z)) <br> Flc(z) = C2; 0≤z≤d(C2) |  - Fluorescence within ED uniform |
| Swart et al. (2015)  | C3 = max<sub>0≤z≤ED</sub> $`\left(\frac{Fl}{b_{bp}}\right)`$ <br> Flc(z) = C3 × b<sub>bp</sub>(z); 0≤z≤d(C3) | - ﬂ : bbp ratio constant with depth |
| Hemsley et al. (2015)  | Chl<sub>NT</sub> = m × $`b_{{bp}_{NT}}`$ + c*  <br> Chl<sub>DT</sub>(z) = m × b<sub>bp</sub>(z)<sub>DT</sub> + c; 0≤z≤ED <br> *m (slope) and c (intercept) | - ﬂ : bbp ratio constant with depth and time |
| Thomalla et al. (2018)  |  Flc<sub>DT</sub> = $`\left(\frac{Fl_{NT}(z)}{Fl_{DT}(z)}\right)`$ × b<sub>bp</sub>(z)<sub>DT</sub>; 0≤z≤QD <br> If Flc<sub>DT</sub>(z) < Flc<sub>DT</sub>(z) then no correction is applied |  - Same depth distribution of ﬂ : bbp between night and day <br> - No quenching at night |

**b<sub>bp</sub>**: particulate backscattering proﬁle; **d**: depth; **DT**: daytime proﬁle; **ED**: euphotic zone depth; **Fl**: ﬂuorescence proﬁle; **Flc**: corrected ﬂuorescence proﬁle; **FlNT**: averaged ﬂuorescence over the night; **MLD**: mixed layer depth; **NT**: nighttime proﬁle; **QD**: quenching depth; **z**: depth domain

We can say that if day and night profiles are used, the sunset/sunrise time can be used to separate the profiles or if PAR is available, this variable can used instead
