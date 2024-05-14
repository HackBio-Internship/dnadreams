+++
title = 'Everything BASh in 10 minutes'
date = 2024-04-29T16:36:29+02:00
draft = false
author = "HackBio"
+++

# Everything BASh in 10 minutes

> 🧠 This is a straight, hands-on, instruction based tutorial

Now that you know how to access the terminal; it is time to learn how to navigate the terminal. 

Why: For the rest of your career in bioinformatics and data science, you will handle thousands of datasets, files and folders. The terminal gives you superpower to handle this huge data scale. It also helps you to automate your analysis pipelines as you will see later in this course. Your ability to navigate the terminal is arguably 25% of everything you need in your entire bioinformatics career. It is a skill you will use for the rest of your life in bioinformatics. **It is non-negotiable**.  

### Tasks

> 🚧 I will also show you the GUI equivalent of what you are doing.

- Who are you?
    
    ```bash
    whoami
    ```
    
- Where are you?
    
    ```bash
    pwd
    echo $PWD
    ```
    
- Where is home?
    
    ```bash
    echo $HOME
    ```
    
- Let’s start by creating a folder named HackBio
    
    ```bash
    mkdir hackbio
    ```
    
- Let’s see the list of files and folders that we have
    
    ```bash
    ls 
    ls -l
    ls -lh
    ```
    
- Let’s download a simple file from the web
    
    ```bash
    wget https://raw.githubusercontent.com/josoga2/sc_data/main/forensics/forensics.fasta -O forensics.fasta
    ```
    
- Now, let’s see if the file was truly downloaded and copy it to the right destination
    
    ```bash
    ls
    ls -lh #to see the file size
    cp forensics.fasta hackbio/ #you can use the same code for mv
    ```
    
- We are outside the hackbio folder, let’s get in and see what’s inside
    
    ```bash
    cd hackbio/
    ls 
    ls -lh
    pwd
    ```
    
- Let’s open up the file we downloaded
    
    ```bash
    #first thing, make sure you are in the right working directory
    pwd #if you are in hackbio proceed
    ls #to check if your file is in there
    cat forensics.fasta
    #that was too fast, let's do it little by little
    less forensics.fasta
    #use q to quit
    ```
    
- Let’s make a simple text based file manually
    
    ```bash
    touch hackbio.txt
    ls -lh
    ```
    
- The file is empty and I actually do not need it, not now not in the future
    
    ```bash
    rm hackbio.txt
    ```
    
- Finally, let’s look for a specific pattern inside the forensics.fasta file

```bash
#let's go to our home directory
cd
grep 'Sample' hackbio/forensics.fasta #note that I still rerouted it back to the host folder hackbio

#let's print everything that does not contain Sample
grep -v 'Sample' hackbio/forensics.fasta
```

Overall, knowing your working directory is very important. I have seen situations where the wrong working directory made a full-grown adult cry.

---

### Pipes 🪈, arrows 🏹 and ampersands &

Like you have already seen, the Bash/Linux terminal is a powerful command-line interface that allows users to interact with their systems efficiently. Understanding how to use pipes (**`|`**), arrows (**`>`** and **`<`**), and ampersands (**`&`**) can significantly enhance your command-line skills. In this tutorial, we'll cover the basics of these essential features.

### **1. Pipes (`|`)**

A pipe is used to redirect the output of one command as the input to another command. This allows you to create powerful command pipelines.

### Example:

```bash
#let's create a new file
touch hackbio.txt
ls -lh
ls -l | grep "hackbio"
```

In this example, the output of the **`ls -l`** command (file listing) is passed as input to **`grep`**, which then filters the lines containing the word "hackbio"

### 2. Wildcard

The **`*`** wildcard represents any sequence of characters (including none). It is often used to match filenames or patterns. Say you have 50 files, 10 are txt, and 40 are fasta, you can use the wildcard to quickly access all the txt (or fasta) as the case may be

### Example:

```bash
ls #prints all
ls *.txt #prints only txts
ls *.fasta #prints only fasta
#of course, your flags also work
ls -lh
ls -lh *.txt #prints only txts
ls -lh *.fasta #prints only fasta

```

### 3. Ampersand

The `&&` double ampersand is used to join two commands together and operate them at once. For example. most times we create a folder and want to jump right into the folder. Let’s try that

```bash
mkdir bio && cd bio
```

It makes the directory and jumps right into it. You can also add a third component `ls`

```bash
mkdir bio && ls && cd bio
```

### 4. Outputs

The `>` and `<` can be used to export the printout of a terminal into a new file.

```bash
#to print the number of lines in a file
cd hackbio/
wc -l forensics.fasta

#let's print this output into a new file
wc -l forensics.fasta > output.txt
```

---



Happy Coding!

Happy Bioinformatiking!!