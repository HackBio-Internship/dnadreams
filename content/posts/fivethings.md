+++
title = 'Five things you master in bioinformatics through experience'
date = 2024-04-29T16:40:07+02:00
draft = false
author = 'Wale Ogunleye'
+++

> 🍎 Simple but powerful secrets that make life easier while coding.

Bioinformatics is a game of practice. The more you practice, the better you become at it. The thing with practicing is that you encounter more errors, problems and challenges, but these errors only reinforce your skillsets. You get better at interpreting them and solving them each time they appear, even if its in a different form. The interesting thing about errors is that you will probably still make them even though you are forewarned about it.

From experience, we present you with some of the things that you can always do to solve coding based problems faster.

- Tab Key for autocompletion: Coding terminals/consoles have the worst user experience in the world. This is because they lacks a graphical interface. So sometimes, you don’t know the right command or files/folders you are working with. The tab ⇥ key (usually on the left side of letter Q on the keyboard) can help you with that. For example,
    
    ```bash
    cd
    cd hackbio
    cat f⇥ 
    #prints out all the words starting with f
    cat forensics
    ```
    
- Arrow Up/Down for history: Did you just use a code and it worked perfectly? Or want to quickly see that code again. Don’t worry, I gat you. Just press your arrow up key ⬆️. The more you press it, the more it shows you previous commands you have parsed
- Your working directory: This is by far the reason why most beginners give up on bioinformatics. They are working from a wrong directory, and as such the computer keeps telling them `File does not exist`. This can be really frustrating especially if you keep repeating it, fixing every other thing, and not the working directory. Always remember to confirm your working directory. Also, using the tab autocomplete key can help to reduce misdirected file paths
- Deleting files with `rm`: On the terminal, there is no such thing `**recycle bin**`. Once you delete, you delete permanently. If you don’t have the original files, premium tears await you. The horrible thing is that there is no warning! Once you press enter, its gone, no way back. There is no solution to this. You just have to make sure you really want to delete a file everytime you use `rm` .
- Always use `ls -lh` after every download or command: `ls -lh` is a basic quality check to see the size of your file after every download. Why? Sometimes, with wget or some commands that generate new files, you may just be outputting a plain text or an empty file (because the provider of the link had some errors) or a broken file (because of internet connection) or error in the pipeline (many things could cause this). When you check the file size, you realize that you have a ‘fake’ or ‘incomplete’ file. The file size usually is a preliminary indicator of what is in the file. If you go ahead to use such files without checking their file size or content, you will usually get an error.

These advice are very invaluable. You will understand their value with time and probably thank me later.  

Happy Coding!

Happy Bioinformatiking!!