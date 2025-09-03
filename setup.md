---
title: Setup
---

## R Genomics Workshop Setup Directions

### Logging into Rivanna/Afton

To log into the Rivanna or Afton HPC cluster, open your terminal (or **MobaXterm** if you are on Windows).  

- On **macOS Catalina or later**, the default shell is **Zsh**. To temporarily switch to **Bash**, open Terminal, type:

```bash
bash
```

and press <kbd>Return</kbd>. This switches your shell to Bash for the current session.

Once you have your terminal open, connect to the HPC cluster by typing:

```bash
ssh -Y uva_compute_id@login.hpc.virginia.edu
```

Replace `uva_compute_id` with your UVA computing ID in the above command. You will then be prompted to enter your UVA NetBadge password. This command securely connects you to the HPC cluster.


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

