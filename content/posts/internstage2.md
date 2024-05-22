+++
title = 'Internship Questions Set Stage 2'
date = 2024-05-22T09:12:04+02:00
draft = false
author = 'HackBio'
+++

![](images/Internship.png)

> To get started with learning bioinformatics, with mentorship and project experience, visit [HackBio](https://thehackbio.com)

## **Project 3: Run a simple NGS analysis pipeline**

In this section, you will implement a simple NGS analysis on a simple dataset

**Starting Datasets:**

- [Forward Strand](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://zenodo.org/records/10426436/files/ERR8774458_1.fastq.gz?download%253D1%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907983611%26amp;usg%3DAOvVaw1s7cFGXEu-p2dYmmTorvHU&sa=D&source=docs&ust=1712325907992477&usg=AOvVaw38coaiMy7t0gwZ1YS8a75k)
- [Reverse Strand](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://zenodo.org/records/10426436/files/ERR8774458_2.fastq.gz?download%253D1%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907983787%26amp;usg%3DAOvVaw3vnmcuR34nF70vpiQMVDsW&sa=D&source=docs&ust=1712325907992631&usg=AOvVaw3EFwehhBGPjWr_GjlvjmS5)
- [Reference](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://zenodo.org/records/10886725/files/Reference.fasta?download%253D1%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907983909%26amp;usg%3DAOvVaw1cwZjXPZIofYZzkkKAkLlg&sa=D&source=docs&ust=1712325907992699&usg=AOvVaw2EdUT1BtuagiTf1Ls-AyDV) Genome

**Proposed Pipeline**:

Download dataset (**wget**) => Quality Control (**FastQC**) => Trimming (**FastP**) => Genome Mapping (**bwa**) => Variant Calling (**bcftools/freebayes**)

Feel free to add software as you prefer.

**Let’s get bigger:**

Use your pipeline to analyze more datasets

**Reference**: [https://raw.githubusercontent.com/josoga2/yt-dataset/main/dataset/raw_reads/reference.fasta](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://raw.githubusercontent.com/josoga2/yt-dataset/main/dataset/raw_reads/reference.fasta%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907984707%26amp;usg%3DAOvVaw3rTrRHWoEsMG8IUDC4E-q_&sa=D&source=docs&ust=1712325907993012&usg=AOvVaw14Q14b4QXRqxLegzXOTxGE)

**ACBarrie**

- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/ACBarrie_R1.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/ACBarrie_R1.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907984921%26amp;usg%3DAOvVaw3aAKOQkR7TcZIOuU8Tjzw2&sa=D&source=docs&ust=1712325907993133&usg=AOvVaw2_OGxD9UBZJE_atThtniLB)
- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/ACBarrie_R2.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/ACBarrie_R2.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985018%26amp;usg%3DAOvVaw1vekcLDkKpnYnDTDW4p2zh&sa=D&source=docs&ust=1712325907993201&usg=AOvVaw3v2KrSdeEPXOuR-j2azjLd)

**Alsen**

- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Alsen_R1.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Alsen_R1.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985349%26amp;usg%3DAOvVaw2f5_k1c1msG2Reh2JMntn2&sa=D&source=docs&ust=1712325907993282&usg=AOvVaw2mtzJ8Q0dKs_P5nBt0_CTw)
- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Alsen_R2.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Alsen_R2.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985443%26amp;usg%3DAOvVaw1yPExNHd-v_Bbm-dSVKzT1&sa=D&source=docs&ust=1712325907993333&usg=AOvVaw1yabCUo0CnuGGsCo-aLn87)

**Baxter**

- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Baxter_R1.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Baxter_R1.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985618%26amp;usg%3DAOvVaw0LzmGsDcTFIJGFFcS9EUvq&sa=D&source=docs&ust=1712325907993407&usg=AOvVaw36C7hfLfg-o8KzKaDDdPCX)
- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Baxter_R2.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Baxter_R2.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985702%26amp;usg%3DAOvVaw3itTpdGAWV4XyKP9kINsYN&sa=D&source=docs&ust=1712325907993459&usg=AOvVaw3HOCgjL255gFci7Ti8t1dJ)

**Chara**

- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Chara_R1.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Chara_R1.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985869%26amp;usg%3DAOvVaw2hypkLI76NBQL73KeB8jRY&sa=D&source=docs&ust=1712325907993532&usg=AOvVaw2QRsFiLv6ahhQxaafQUyhV)
- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Chara_R2.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Chara_R2.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907985951%26amp;usg%3DAOvVaw1VOokVJ8aOJVy45lxDKqGV&sa=D&source=docs&ust=1712325907993589&usg=AOvVaw1OJo4qeqQwCl5LwyDNBNRr)

**Drysdale**

- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Drysdale_R1.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Drysdale_R1.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907986133%26amp;usg%3DAOvVaw1yWbfz5VzkfLhAqjx52CVt&sa=D&source=docs&ust=1712325907993669&usg=AOvVaw2rjW15M3D83PC6eDpGXdak)
- [https://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Drysdale_R2.fastq.gz](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://github.com/josoga2/yt-dataset/raw/main/dataset/raw_reads/Drysdale_R2.fastq.gz%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907986280%26amp;usg%3DAOvVaw11d68NWrFyGtg8aqp-JviI&sa=D&source=docs&ust=1712325907993728&usg=AOvVaw0G09RvMtMAOSAi3yGmI58K)

**Submission**:

- We look forward to receiving your final pipeline **script.sh** (you can use bash, snakemake, nextflow or any pipeline tool you know how to use).
- Alongside, create a **setup.sh** file that anyone can use to install all the tools needed for making the pipeline work.
- Make a **requirement.txt** file that simply lists all the tools you used
- Upload the 3 files to your team’s github repo. Each team member should have a folder and their folder should contain their 3 scripts.
- Copy the link to the team’s repo and paste it on HackBio Submission platform
- Finally, be ready to discuss your pipeline with everyone

**Resources**

- [Introduction to Whole Genome Sequencing and Variant Calling](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://www.youtube.com/watch?v%253DNxRECdxKP40%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907987103%26amp;usg%3DAOvVaw13LRKERNM9nPfZFXtHaHm0&sa=D&source=docs&ust=1712325907994143&usg=AOvVaw3PqKIMj8wZ4duB2G2ysVig)
- [Raw Sequence to Variant Calling Pipeline with FreeBayes](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://www.youtube.com/watch?v%253DgmJ6LteXAq0%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907987311%26amp;usg%3DAOvVaw3AwcToFIPx1dWMh2BY-92V&sa=D&source=docs&ust=1712325907994212&usg=AOvVaw2SP5F2YwqDT6LBEuB_iPfK) (Hands-On)
- [Galaxy Tutorial for Variant Calling (with Code)](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://training.galaxyproject.org/training-material/topics/data-science/tutorials/bash-variant-calling/tutorial.html%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907987483%26amp;usg%3DAOvVaw1VLYT40aQSowPcnaNmUAhl&sa=D&source=docs&ust=1712325907994291&usg=AOvVaw2Eango74qMHDO-uYB3ls8T)
- [Using For loops in BASh](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://www.youtube.com/watch?v%253DT7hVOiTsSUU%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907987615%26amp;usg%3DAOvVaw2PRroqkzTbPbmvyR0kC-_m&sa=D&source=docs&ust=1712325907994356&usg=AOvVaw2hvmvQ6ZDcC-uFWa9KbLnM)
- [HackBio Video for loops for multiple datasets using FastP](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://youtu.be/HNE0VPZK8yM%26amp;sa%3DD%26amp;source%3Deditors%26amp;ust%3D1712325907987720%26amp;usg%3DAOvVaw1VOZ0BM60qJw7AgIrgVKvJ&sa=D&source=docs&ust=1712325907994428&usg=AOvVaw1XP6w97CG4jfo4DlMDDj5e)

---
> 🍿 [Subscribe to get notified of news, opportunities, gigs and new roles in the bioinformatics world](https://forms.gle/foGNDfPUQgi3QmSf7).