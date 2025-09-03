---
title: Setup
---

## R Genomics Workshop Setup Directions

## Logging into Rivanna/Afton

To log into the Rivanna or Afton HPC cluster, start by visiting the **HPC Login Instructions** page:  
[https://www.rc.virginia.edu/userinfo/hpc/login/](https://www.rc.virginia.edu/userinfo/hpc/login/)

You can either follow the instructions for **Web-based Access**, or the **Secure Shell Access (SSH)**

### Web-based Access
For web-based access, scroll down to the **Web-based Access**, and click on ``Launch Open OnDemand''. Log on using your UVA credentials (uva_compute_id and Netbadge password). You now have point and click access to your account on UVA’s HPC!. 8.	Click on ">_ Open in Terminal" on the upper left of the screen. 9.	This will open a UNIX terminal on your web browser.

### Secure Shell Access (SSH)
UVA HPC is accessible through ssh (Secure Shell) connections. Follow the instructions for Secure Shell Access (SSH) based on your operating system:

- **Windows**: Install the recommended SSH client, **MobaXterm**, by clicking the *Install MobaXterm* button under the Windows section of the page and following the instructions.  
- **macOS**: Open the **Terminal** application, located in the *Utilities* folder.  
  - On macOS Mojave and earlier, the default shell is **Bash**.  
  - On macOS Catalina and later, the default shell is **Zsh**. To temporarily switch to Bash, open Terminal, type `bash`, and press <kbd>Return</kbd>.  
- **Linux**: Most Linux systems use **Bash** as the default shell. Open a terminal using the Applications menu or search bar (look for **Terminal**, **Konsole**, or **xterm**). If your system defaults to another shell, you can switch by typing `bash` and pressing <kbd>Return</kbd>.  

Once you have a terminal open, connect to the HPC cluster by typing:

```bash
ssh -Y uva_compute_id@login.hpc.virginia.edu
```

Replace `uva_compute_id` with your UVA computing ID. You will then be prompted to enter your UVA NetBadge password.


### Workspace for This Lesson

First, make sure you are in your home directory. In the terminal, type:

```bash
cd
```

and press <kbd>Return</kbd>.
(The cd command changes your location. With no arguments, it takes you back to your home directory.)

Next, create a new directory called day2 where you will do your work:

```bash
mkdir day2
```

and press <kbd>Return</kbd>. (The mkdir command makes a new folder named day2.)

Move into this directory:

```
cd day2
```

and press <kbd>Return</kbd>.
(Now you are “inside” the day2 folder, and any files you create will be saved here.)

To confirm you are in the correct location, type:

```bash
pwd
```

and press <kbd>Return</kbd>.
(The pwd command prints your current working directory, i.e., the folder you are in.)

The output should look like:

```
/home/your_computing_id/day2
```

with your own computing ID in place of `your_computing_id`.

### Data for This Lesson
The data for today’s lesson is stored in `/standard/bims6000/r_day2`.

Let’s copy the file into your working directory so you have your own copy. Run:

```bash
cp /standard/bims6000/r_day2/combined_tidy_vcf.csv .
```

and press <kbd>Return</kbd>. The cp command copies files. Here, it copies the file `combined_tidy_vcf.csv` from the shared class folder into your current directory, day2. The . means “put it here.”

