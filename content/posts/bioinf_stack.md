+++
title = 'The Ideal Stack for Beginners in Bioinformatics'
date = 2024-04-29T14:23:00+02:00
draft = false
author = 'Wale Ogunleye'
+++

![](https://media.licdn.com/dms/image/D4E12AQHTCroCXAMkYQ/article-cover_image-shrink_720_1280/0/1707258578993?e=1720051200&v=beta&t=6XpBNN9O5j6vzRNqVlXmmVmtTNLfq60koNeRHseyVVk)
Welcome to the dynamic world of bioinformatics! As a beginner, embarking on the journey of mastering bioinformatics can be both exciting and overwhelming. One of the first challenges you'll encounter is figuring out the right combination of tools and skills to build a strong foundation. In this guide, I'll break down the bioinformatics tech landscape into clear categories, making it easier for you to navigate and build the ideal stack that suits your interests and career journey.

I will take a cue from [Kevin Blighe, Ph.D.](https://www.linkedin.com/in/kevinblighe/) who (to my knowledge) was the first person to suggest that bioinformatics specialities should be divided into clear tech stacks just like our colleagues in tech. Developers in tech have a clear stacking structure (front-end, back end or full (both) stack), and these structure makes skill development and career navigation easy. and straightforward.

Dr Kevin in his LinkedIn post suggested:

- Upstream Developers
- Downstream Developers
- Full/Main Stream Developers.

Before I explain each category, it will be nice to know what a typical bioinformatics project looks like.

Bioinformatics projects have heavy data components. In some cases, the data generation step (wet lab) is part of the project and in others, it might not. Most modern projects are beginning to adopt the hybrid (both wet and dry) project style because of data ownership issues.

These projects typically generate big but raw data, we are talking about hundreds of gigabytes to few terabytes of raw biological data. For example, the Mexican Biobank Project (Nature, 2023) houses about 6000 biological samples which includes their raw sequence data. If the genome of a single human is about 3gb on your computer’s hard disk, it means they would need about 18000 Gb (or 18 Tb) of storage to house the data. This is the **proper Big Data** 😎.

By now, three things must be obvious to you;

- You cannot store this dataset on your personal computer to store this dataset. You probably have a 500 Gb or 1Tb (at best) 🥹
- If you cannot store it on your computer, then you cannot analyze it on your computer
- Finally, you need something more powerful than excel (or any spreadsheet program) to analyze this dataset.

NB: Data type is not restricted to genomic sequencing dataset. [Learn about other data types here](https://omicstutorials.com/what-types-of-data-does-bioinformatics-work-with/)

**Upstream Dev**: Given the amount of data size and its potential complexity, you need a specialist who can parse the data from its raw form into processed analysis ready datasets. These are the upstream developers. They develop custom, project specific pipelines to perform quality control and pre-process the raw data. They make first contact with the raw data and determine if the data is bonafide to answer the biological question at hand. Usually, the datasets come in batches. It is their job to systematise the process of receiving the dataset and subjecting the data to the same set of quality control and pre-processing procedures. For this reason, I like to think of them as bioinformatics engineers.

Typical bioinformatics pipelines are built with **snakemake** or **nextflow** and implemented on a **BASh** terminal with a **Unix** Operating System. The entire set of tools for quality control and data preprocessing is connected in such as way that the output from one end is the input for the next tool thereby making the data flow seamlessly [Article on data preprocessing]. The output from all these steps goes to the Downstream Devs.

**Basic** **Techstack for Upstream dev:**

- Linux: The operating system of your life
- Git: For version control and collaboration
- BASh Scripting (For handling tonnes of bioinformatics packages)
- Nextflow / Snakemake: For building pipelines
- SLURM: For scheduling bioinformatics tasks to run while you sleep 🛌
- A cloud computing / HPC platform: Most organization rely on them for storing / computing data

**Downstream Dev.:** Downstream developers receive a cleaner downsized version of the dataset. In fact, they might receive the data in a spreadsheet worthy format. They also build pipelines, but their pipelines are strongly analytical. It is their job to connect the data back to answer the research question we started with. They conduct all the data filtering, wrangling, statistical testings and final data interpretation. The process involves a lot of back and forth in order to catch the main insights in the data. In the modern AI era, I would classify machine/deep learning tasks as downstream tasks.

Typical downstream data processing analysis are done on R or Python since they have most of the libraries for analysis and visualisation. I also think downstream devs are better storytellers since have to think of the research questions and answer them in form of graphs, plots and charts. Their outputs (usually visualisations, dashboards and tables) go into publications, websites, blogs and reports for communication with a wider audience.

**Basic** **Techstack for Downstream dev:**

- Data Language: Python or R
- Git: for version control and collaboration
- BASh Scripting (minimal but necessary)
- ggplot2 or matplotlib: For visualisation of any data type/form
- Data Libraries Python: Pandas for managing dataframes Numpy for calculating higher order dimensions of data Sci-kit learn for machine learning (ML) Keras / Tensorflow / Pytorch for deep learning (DL) R Base R (I honestly think this is more than enough. Even for basic ML applications) Tidyverse (has a lot of enemies these days) Shiny for dashboarding
- Every other thing is built on experience.

*Note: Don’t get into the cul-de-sac of having to pick either R or Python. Just close your eyes and pick one and you will be fine. Should you need to learn the second language, the knowledge of the first will make it extremely easy to learn the second one. They are like Spanish and Portuguese.*

**Full/Main Stream** is a combination of both. I really think this is more tedious and making the entire datastream go through one person can be risky. However, you have the opportunity to be skilled in a lot of things (although not necessarily with depth). Also, since you are not transferring data between users/departments, there are less chances for error due to communication. Bioinformaticians in smaller companies or PhD students find themselves in the FullStream situation. Larger companies tend to be able to hire more people to handle several aspects of a single project.

**Choosing where to start from**: If you are interested in learning a lot of things, full stream is the way to go, it gives you the opportunity to fight gain a lot of experience after fighting many battles. However, if you love to have a focus, one of up or down stream will be your way. Upstream is a little bit more abstract and may not be fulfilling for visual persons. It is more appealing for people who like to build and solve problems at scale using systems. If you like visual things with an opportunity to report/present your findings, then go downstream. On the flipside, downstream dev requires a good knowledge of the subject area (domain expertise) and an ability to switch between experimental numbers and biological theories.

Personality Quiz: Who are you, how do you think/approach problems and how does that help you define where to start. Take this [personality test](https://thehackbio.com/path-finder) to get you started.

Final Notes: In this article, we have seen the landscape of technologies in bioinformatics and how to approach them. Now that you know what you want, go out their and start learning. Pick a single battle (out of the 3 above) and start fighting (learning). At HackBio, we call these biostacks, and we have developed beginner courses for up and downstream development. Feel free to reach out to me should you need further help/clarification or collaboration on a project.

