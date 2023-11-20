---
title: "Ultimate Beginner’s Guide to Using the Terminal"
seoTitle: "Ultimate Beginner’s Guide to Using the Terminal"
seoDescription: "Unlock the Power of the Terminal: Learn essential commands for navigating directories, creating files, and customizing your workflow."
datePublished: Mon Nov 20 2023 07:42:12 GMT+0000 (Coordinated Universal Time)
cuid: clp6lmpfa00010al83c6mb3cn
slug: ultimate-beginners-guide-to-using-the-terminal
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1677820433567/24f590f4-dcfe-408c-8675-edf092cd139d.jpeg
tags: terminal, command-line, cli, terminal-command, command-line-interface

---

For years, I was afraid of the Terminal. I was scared that I would erase my entire hard drive with a single typo. 😱

But, then I started using a task runner to compile my Sass (among other things). My world changed forever. I found it to be so much faster and allowed far more task automation than the tools I had been using previously. Anything that will speed up your workflow is worth investing in (whether that’s time or money).

Once I started spending more time in the Terminal, I became more comfortable and confident. Trust me, I still prefer a good GUI (graphical user interface), but I’m no longer afraid I’m going to delete my entire hard drive. — And let’s be honest, you could delete your entire hard drive with a GUI too. Drag your hard drive to the trash and click "Empty Trash." But, nobody in the right their mind would do that. Similarly, you’d have to type a very specific command in the Terminal to delete your entire hard drive and nobody in their right mind would do that either. — Plus if you have a typo in the Terminal, generally, it will you that you have a typo and the command won’t run.

## Terminal Commands that I’ve Found Helpful

So, here are the commands that I've found to be the most useful.

> Typically when you see commands to run Terminal, you'll see a $ at the beginning of the line. Don’t copy the $, it signifies that it’s the beginning of a Terminal line.

### **Changing Directories**

`cd` stands for **change directory.** Similar to the Finder where you click on the folder, in Terminal, you just type in the directory that you want:

```bash
$ cd Sites
```

You can type `cd ..` to go up a level or `cd ../..` to go up 2 levels. `cd /` will take you to your home directory.

The Terminal also supports tab auto-completion. So you could type `cd De<TAB>` and it will fill in `cd Desktop` (assuming that’s a folder option) for you. Handy!

### **Listing a Folder's Contents**

`ls` will list all files and directories in your current location. If you want to see "hidden" files, or files that start with a period (.) Simply, add a "flag". You can think of a flag as a way of modifying your command or adding preferences. In our case, `ls -la`.

![File listing with the Terminal, include hidden files](https://cdn.hashnode.com/res/hashnode/image/upload/v1700403839722/62bd2bfd-3d04-43cc-a49c-c98baa2994a9.png align="center")

The dash `-` and any letter combination after the dash is called a flag.

If you want also want to see who owns the file and its permissions use `ls -la`.

![Detailed file listing within the Terminal](https://cdn.hashnode.com/res/hashnode/image/upload/v1700403755932/2a4bb493-9ad9-4af0-837d-7a0cd3dd9cdd.png align="center")

In our output, the weird looking letter combinations on the side, like `drwxr-xr-x` , is a shorthand for that file's/folder's permissions. In this case, everyone can read the directory, but its content can only be changed by the user. If you want to do a deep dive on permissions, you might find [this article from Serverwise](https://blog.ssdnodes.com/blog/linux-permissions/) useful.

`pwd` will show you the file path to your current location. This comes in real handy when you want to run a script from anywhere.

![Current file path within the Terminal](https://cdn.hashnode.com/res/hashnode/image/upload/v1700403881379/81708f52-aa73-45d3-b82b-93770c804925.png align="center")

### **Making a New Folder (or Directory)**

`mkdir FOLDERNAME` will **create a folder** named FOLDERNAME. `mkdir` stands for "Make Directory."

> ⚡ **Power Tip:** Anytime, you hit the up arrow on your keyboard, it will fill in the last command you ran. Hit it again and it will cycle to the command before that. The down arrow cycles in the opposite direction.

Just to give you an idea of how these commands are used together: when I first open the Terminal, I might type `ls` to see what the nested files / folder options are. Then:

```bash
$ cd Code/GIT/
$ mkdir NEWPROJECT
$ cd NEWPROJECT
```

This navigates to the GIT folder and then creates a new directory for a project. Then, navigates inside the folder I just created.

If this is still making your head spin, here’s a WYSIWYG way that I saved until the end:

* Open up your Terminal type in `cd .`
    
* Then, open up Finder, navigate to the Folder you want to open in Terminal
    
* Drag that folder from the Finder onto your Terminal window. It should enter the location for that file path for you.
    
* Now, hit `<RETURN>`. — You’re welcome.
    

%[https://vimeo.com/886120236?share=copy] 

### Creating a New File

You can create a new file by saying `touch` and then giving the filename:

```jsx
touch .gitignore
```

---

I have a FREE Cheatsheet of my most used Terminal Commands that you can [**download for FREE**](https://selfteachme.ck.page/5085fd4b48).

%%[convertkit-git-cheatsheet] 

---

## A **few other tips and tricks:**

### **Install Warp, Hyper, or iTerm2 as a Terminal Replacement**

If you’re working on a Mac, “Terminal” comes preinstalled.

* Pull up the **Finder**
    
* Type `Cmd + Shift + U` and you’ll automatically jump to the Utilities folder
    
* Inside, you’ll find an application literally called “Terminal”
    

This works great if you’re just getting started, but I actually prefer to use [**Warp**](https://warp.dev). It has a little bit more functionality. Besides, it doesn't hurt that it's **FREE!**

### **Customize the Look and Feel of your Terminal**

I keep it simple and maintain that less is more. However, you can add additional information for each prompt.

For example, you can change the prompt colors, display what git branch you're currently using, the current git state, etc.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1700406662672/33076cb8-7d89-480f-8921-92dfcd91b385.png align="center")

[Starship](https://starship.rs/) makes this easy.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1700406660214/7efe9f06-d216-498f-b80d-fda069b9dd50.png align="center")

1. Use a simple brew command to install:
    
    ```bash
    brew install starship
    ```
    
2. Add the initialization script to the end of your `./zshrc` file:
    
    ```bash
    eval "$(starship init zsh)"
    ```
    
3. Create a configuration file:
    
    ```bash
    mkdir -p ~/.config && touch ~/.config/starship.toml
    ```
    
    Then, all of your [customizations and configurations](https://starship.rs/config/) are done within your TOML file.
    

---

Overcoming any fears you might have of the Terminal can lead to significant improvements in productivity and efficiency. While graphical user interfaces have their lace, the Terminal is a powerful alternative, that in practice can increase your productivity and streamline tasks.