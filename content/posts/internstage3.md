+++
title = 'Internship Questions Set Stage 3'
date = 2024-05-22T09:18:44+02:00
draft = false
author = 'HackBio'
+++

![](images/Internship.png)

> To get started with learning bioinformatics, with mentorship and project experience, visit [HackBio](https://thehackbio.com)

## **Project 4a: Prevalence of resistance genes to selected antibiotics in sepsis across different countries.**

This project delves into the critical intersection of antibiotic resistance and severe infections such as sepsis. Sepsis, a life-threatening condition, often involves E. coli, a bacteria commonly found in the human gut. This research aims to comprehensively analyze the prevalence of antibiotic resistance genes within E. coli genomes isolated from sepsis patients.

By focusing on specific antibiotics, the study seeks to identify the prevalence and distribution of resistance genes, shedding light on the effectiveness of current treatment regimens. Understanding the genomic landscape of antibiotic resistance in E. coli associated with sepsis is pivotal for informing clinical practices, antibiotic stewardship, and public health policies.

This research not only contributes valuable insights into the evolving landscape of bacterial resistance but also aids in refining therapeutic strategies for sepsis management. By deciphering the genetic basis of antibiotic resistance in E. coli, the project plays a crucial role in the ongoing global effort to combat antimicrobial resistance and enhance patient outcomes in the face of severe infections.

**Selected antibiotics:** Penicillin(s), Ciprofloxacin and Aminoglycoside

**Notes**:

- Ensure that you focus on isolates gotten from Sepsis
- Your dataset should cover at least 3 continents
- Prepare a graphical abstract using Biorender, Bioicons or any other tool at your disposal
- As early as possible, prepare a 1-2 minutes pitch of your research topic and publish on twitter, youtube and instagram. Pitch should be as simple as possible, your ‘grandma’ should be able to understand. The links to your social media posts will be collected by the end of the first week in this stage.
- Votes from SM will be counted alongside the final presentation.
- Prepare powerpoint slides for your final presentation to the world. This is a global event. To ensure fairness, voting will be done by the public. No HackBio organizer or mentor will be allowed to vote

## 

---

## **Project 4b: Impact of mutations in intergenic regions.**

Recently, introns (intergenic regions) have gained increasing popularity for their role in the development of genetic disorders. In a recent project by the GnomAD, they developed a score for the identification of intergenic regions that could have variants with functional significance. They termed this the gnocchi (z) score which is calculated as (Obs -Exp)2/Exp.

Using the data source below (~2M variants), compute the gnocchi score (ignore the unfiltered_z).

Next, Using your own z_score, generate a chromosome level distribution plot (histogram, boxplot or density plot) showing the distribution of gnocchi score within each chromosome.

Assuming a cut-off of Z-score > 4.0; which chromosome has more significant variants?

For all the significant regions you have selected, use GenomicRanges() (in R) to identify the closest gene to the selected sequence frame between start and end columns. Download any of the Super Enhancer dataset from SEdb ([https://bio.liclab.net/sedb/download.php](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://bio.liclab.net/sedb/download.php%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1714472386517928%26amp;usg%3DAOvVaw1ZKKMOQWzWDem5jHpCU3yO&sa=D&source=docs&ust=1714472386529713&usg=AOvVaw09i4gngfLO2HMvxR-VF4Bz)). Use the nearest() function in GenomicRanges() to perform this step.

Notes:

- Prepare a graphical abstract using Biorender, Bioicons or any other tool at your disposal
- As early as possible, prepare a 1-2 minutes pitch of your research topic and publish on twitter, youtube and instagram. Pitch should be as simple as possible, your ‘grandma’ should be able to understand. The links to your social media posts will be collected by the end of the first week in this stage.
- Votes from SM will be counted alongside the final presentation.
- Prepare powerpoint slides for your final presentation to the world. This is a global event. To ensure fairness, voting will be done by the public. No HackBio organizer or mentor will be allowed to vote

## 

## 

---

## **Project 4c: How does bacterial resistance impact cancer (AML) patients.**

Bacterial infections are the second most common complication in patients with cancer due to both disease-related and treatment-related immunosuppression. By undermining treatment outcomes and reducing survival in cancer patients it is estimated that 8.5% of cancer deaths are due to severe sepsis.

In this project, you will profile the resistance patterns of 8 pathogens across 64 patients.

**Starting Dataset:**

1. 64 bacterial genomes reported here: SRP417207. Use [https://sra-explorer.info/](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://sra-explorer.info/%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1714472386519270%26amp;usg%3DAOvVaw04KC5qH_7sTRpWXrM3Ep5k&sa=D&source=docs&ust=1714472386530196&usg=AOvVaw06ESe7YGRrOrPgMD2MuysC) to download dataset

**Selected antibiotics:** Penicillin(s), Ciprofloxacin and Aminoglycoside

**Selected genes**: Do your research to identify at least 3 genes for each antibiotics class

**Specific Task**: Identify the pathogens in each of the 64 samples and describe the most common resistance pattern.

**Notes**:

- Ensure that you focus on isolates gotten from cancer patients (any kind of cancer is allowed, just remember to mention them)
- ⚠️Be sure you are not downloading metagenomic datasets
- Prepare a graphical abstract using Biorender, Bioicons or any other tool at your disposal
- As early as possible, prepare a 1-2 minutes pitch of your research topic and publish on twitter, youtube and instagram. Pitch should be as simple as possible, your ‘grandma’ should be able to understand. The links to your social media posts will be collected by the end of the first week in this stage.
- Votes from SM will be counted alongside the final presentation.
- Prepare powerpoint slides for your final presentation to the world. This is a global event. To ensure fairness, voting will be done by the public. No HackBio organizer or mentor will be allowed to vote

## 

---

## **Project 4d: Unique Mutations in Different Cancers.**

The **Cancer Cell Line Encyclopedia (CCLE)** project is a project that aims to characterize the different cancer cell lines. Using WGS techniques, they have completely sequenced different cancer cell lines representing different primary sites in the body.

Your task is to select any 5 cell lines and perform variant calling and interpretation for each of the cell lines. Use a clinical grade variant interpreter like mutSigCV, GATK or cuteVariant

Also, try to see the mutations that are present across all the selected cancer cell lines you selected and those that are unique. Try to describe them and interpret their functional consequences. (hint: gene enrichment analysis)

[Data Source](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://www.ncbi.nlm.nih.gov/sra?linkname%253Dbioproject_sra_all%2526from_uid%253D523380%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1714472386521147%26amp;usg%3DAOvVaw1Hm2WFnckXITu2QyNa1FVw&sa=D&source=docs&ust=1714472386530824&usg=AOvVaw1iLhQQwR-1xPY4teTyku_6)

**Notes**:

- Ensure that you focus on downloading WGS datasets from cancer.
- ⚠️Be sure you are not downloading metagenomic, RNA seq or epigenomic datasets
- Prepare a graphical abstract using Biorender, Bioicons or any other tool at your disposal
- As early as possible, prepare a 1-2 minutes pitch of your research topic and publish on twitter, youtube and instagram. Pitch should be as simple as possible, your ‘grandma’ should be able to understand. The links to your social media posts will be collected by the end of the first week in this stage.
- Votes from SM will be counted alongside the final presentation.

---
> 🍿 [Subscribe to get notified of news, opportunities, gigs and new roles in the bioinformatics world](https://forms.gle/foGNDfPUQgi3QmSf7).