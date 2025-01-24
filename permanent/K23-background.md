---
date: 2024-03-30
category: project
stage: building
tags:
  - research
  - grants
  - literature
---

# Background

```mermaid
flowchart LR
	t1[Automaticity]
	t2[Reentry]
	t3[DAD]
	trig[Triggers]
	
	s1[LA size]
	s2[Diastology]
	s3[Fibrosis]
	
	epaf[Early AF]
	ppaf[Progressing AF]
	lpaf[Late AF]
	
	subgraph focus [Phenotyping]
	t1 --> trig
	t2 --> trig
	t3 --> trig
	trig --> epaf
	end
	
	s1 --> ppaf
	s2 --> ppaf
	s3 --> ppaf
	
	epaf --> ppaf --> lpaf
```

__Paroxysmal__ AF requires both a trigger and a substrate to progenerate. 
Paroxysmal, early AF rallies primarily through triggered activity
Electrical abnormalities preceed ± cause mechanical changes (fibrosis, myocardial disarray, leading to increased pre-disposed substrate.
Long-standing, chronic/persistent AF sustains primarily through substrate.
Firing mechanisms occurs primarily from pulmonary veins due to:

 -   Enhanced automaticity
 -   Myocardial micro-reentry
 -   Triggered activity

## Phenotyping

However, phenotyping is lmited.
E.g. PhenoKB uses binary diagnosis of AF (2012), while recent studies showed up to four potential clusters may exist. [@Pastori2020; @Vitolo2021]

1. Younger, lower comorbidities
2. High CV risk factors
3. High CV comorbidities
4. High rates of non-CV comorbidities (e.g. cancer)

## Autonomic influences

- From an ablation perspective, the ganglionated plexi and their locatins, as well as their mapping strategies, are described in [cardioneuroablation](cardioneuroablation.md) 
- From the perspective of basic physiology and basic cardiac electrophysiology, particulary as it pertains to the ganglionated plexi and intrinsic cardiac nervous system, are described in [intrinsic-cardiac-nervous-system](intrinsic-cardiac-nervous-system.md)
- To identify patients that would benefit from cardioneuroablation, would need to understand the sympathetic and parasympathetic state of the patient. Could potentially test at least their vagal responsiveness with the [baroreceptor-reflex](baroreceptor-reflex.md)

- Genetic variants that affect autonomic function along the neurocardiac axis may interplay with known inherited arrhythmis, such as the vagal-mediated triggers of SCD in LQTS patients
- Chronic VNS reduces drop in ejection fraction in different animal models of cardiomyopathy, including MI, but studies have mixed results in humans
	- NECTAR-HF ~ VNS or sham, no difference at 6 months in LV size/function, n = 96
	- INOVATE-HF ~ right VNS + GDMT vs. GDMT, no difference in mortality, n = 700
	- ANTHEM-HF ~ non-randomized VNS, improved LV function, pilot study (*required titrated VNS to cause decrease in HR*)

# Cardiac Electrophysiology

## Electrophysiology studies

- APD variability in the atria precede onset of AF at rapid pacing rates [@vanStaveren2020]
- AERP measurement durnig extrastimuli protocols (e.g. bottom quintile of fibrillatory intervals from endocardium) [@Capucci1995]
- @Avula2019 in JCI insight showed that AF rotors were associated with regions of the greatest heterogeneity of the APD, which was improved by pharmacological intervention regardless of spontaneous or pacing-induced AF (as long as APD heterogeneity was reduced)
- Different types of heterogeneity in atrial tissue may drive AF, as discussed by @Rabinovitch2023
- In a computational model, heterogenous fibrosis affects arrhythmia dynamics as described by @Kazbanov2016

## Stress mechanisms

- Two studies that have looked at mental stress and EPS are quite small (`n = 10` & `n = 12`), but neither looked at atrial properties [@Insulander2003; @Finlay2016]
- @Rosman2019 showed relationship with PTSD and EOAF

## Machine learning

- @Tang2022 looked at clinical risk prediction using ECG and EGM data, which used a machine learning model
	- Methods here are interesting because documents how time-series + multi-channel data can be brought together in ML approach
	- Notably also done by [Sanjiv-Narayan-MD](Sanjiv-Narayan-MD.md)

# Genetics

## Atrial fibrillation

- There are currently known associations of ECG intervals and monogenic arrhythmia susceptibility genes, done by @Choi2021
- Genetic susceptibility prediced by PRS and ECG in a machine learning approach, by @Wang2023
- @Shoemaker2020 showed association with rare variants in AF cases undergoing ablation

