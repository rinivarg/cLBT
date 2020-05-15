# Computerized Line Bisection Test (cLBT)
*Rini Varghese, Jasmine Ma, Carolee Winstein*<br>
**Welcome to the GitHub page for the computerized version of the Line Bisection Test!** <br><br>
The administration of this computerized line bisection test has **3 EASY STEPS**:
 1. Download and install the MATLAB Runtime file
 2. Dowload the cLBT app
 3. Administer the test!<br>
	
**See below for detailed instructions on setup and administration**<br>

<img src="images/img_lbt_2.png" align = "middle" width = "750">

# Instructions for setup
<details>
  <summary>Click to expand</summary>
	
## Step 1: Download MATLAB Runtime 
- The MATLAB Runtime is a FREE standalone set of shared libraries that enables the execution of compiled MATLAB applications or components. <br>
- Note that the Runtime file is quite large (1.7-2 GB).<br>
- **Right-Click on this link and open in a new tab:** https://www.mathworks.com/products/compiler/matlab-runtime.html <br>
- As shown below, download the *R2019a (9.6)* version suited to your platform (Mac, Windows, or Linux)<br>
	<img src="images/mcr_version_img.png" width = "700">

## Step 2: Install the MATLAB Runtime
- Double-Click on the downloaded MATLAB Runtime file from your *Downloads* folder. 
	<img src="images/install_mcr.png" width = "500">
- Follow steps for installation.
- Download and installation of the MATLAB Runtime file is only required the first time. 

## Step 3: Download the cLBT App
- **Right-Click to download the app suited to your platform (Mac or Windows):** <br> 
	- [cLBT App for Mac](https://github.com/rinivarg/cLBT/blob/master/acquisition/cLBT_Mac.zip) (approx. 23 MB)<br> 
	- [cLBT App for Windows](https://github.com/rinivarg/cLBT/blob/master/acquisition/cLBT_Windows.exe.zip) (approx. 47 MB) <br><br>
	<img src="images/dwld_zip.png" width = "700">
- Note that some computers are set up to automatically unzip the downloaded file. If so, proceed to the next step. Otherwise, unzip the file.

## Step 4: The app is ready for use. 
- The thumbnail for the app looks like this: <br>
	<img src="images/app_tn.png" width = "70"> <br>
- Open and follow instructions!

## Note:
- When you open the app, if you see a message like below due to your computer's firewall settings, please click ***Cancel***: <br>
	<img src="images/firewall_msg.png" width = "500"> <br>

- Then, similar to other apps that you might use, please grant permission to open the app by going to Settings or System Preferences. <br> 
On a Mac, you can go to	*System Preferences > Security & Privacy* and clicking on ***Open Anyway*** <br>
	<img src="images/open_anyway.png" width = "500"> <br>
	
- In the message box, confirm by clicking ***Open***. You will only need to grant this permission on the first use.

****
</details> 

# How to administer the test?
<details>
  <summary>Click to expand</summary><br>
	
1) **Screen:** It is recommended to use a screen that is at least 15" in size and is placed 2 feet away (depending on the size of your screen).
3) **Hand:** Use the right (or left) hand. It is advisable to use the hand which you think is proficient at using the computer mouse. Stroke surviovrs use their less-weaker hand while the other hand rests on the lap.
2) **Mouse:** It is recommended to use a wired or wireless mouse to use the pen tool instead of the trackpad of a laptop. Press and hold the left mouse key to activate the pen tool. Wait for the crosshairs to appear before you begin.
4) **Instructions:** Must include the following elements:
	- For each horizontal line in half by drawing a small vertical line through each line as close to its center as possible. 
	- You are only allowed a single try per line. Try to be as accurate as you can.
	- Mark on every line the best you can, without skipping.
	- Do not move the screen closer or to any one side.

****
</details> 

# How does the app work?
<details>
  <summary>Click to expand</summary><br>
	
1) Open the app. Note that sometimes the app takes a few seconds to open up. Please be patient.
2) You should see a *Welcome* message.
3) After you click **OK**, a dialog box appears asking for 3 required inputs:<br>
		<img src="images/data_name.png" width = "200"><br>
		(1) **Enter an appropriate ID.**
			This ID will be the Participant ID in your data output file. <br>
		(2) **Enter Gender.**
			Use a single letter: M (Male), F (Female), or N (Not disclosed). <br>
		(3) **Enter Number of Trials.**
			You can use any whole number starting from 1. 
			It is advisable to use at least 10 trials, but you can use more.
			Click **OK**. <br><br>
4) Next, you will be prompted to ***Select*** a location to save your output files. 
		<img src="images/output_fld.png" width = "400"><br><br>
5) Once you have selected your desired location, you will see the instructions for the task:<br>
		<img src="images/instr.png" width = "500"><br><br>
6) You will now see the first trial for the line bisection test. Wait for the cross-hairs to appear (see below) before you mark the midpoint of the horizontal line. Note that the horizontal line will appear in different quadrants of the screen.<br>
		<img src="images/crosshair.png" width = "400"><br><br>
7) Draw a short vertical line to indicate your response (see below):<br>
		<img src="images/mrkd_trial.png" width = "400"><br><br>
8) After you have completed all the trials, you will see a summary figure (see below) and a *Thank you* message.<br>
		<img src="images/summ_fig.png" width = "300"><br><br>
9) Your output data folder is saved at the destinastion that you indicated at the start of the test and will be named: **LBT_[yourID_yourGender]**<br>
10) The app will close when you close these windows.
****
</details> 

# What does the output folder contain?
<details>
  <summary>Click to expand</summary><br>
	
The output folder contains the following files: <br>
- **00a_LBT_summary.tiff**<br>This is the summary image file that you see at the end of the test.<br>
- **00b_Average_Report_LBT_[yourID_yourGender].txt**<br>This file contains the average absolute and percent deviation across all trials. It also contains the total time taken to complete the test (in seconds). <br>
- **00b_TrialWise_Report_LBT_[yourID_yourGender].txt**<br>This file containts the trial-wise absolute (in a.u.) and percent deviations across all trials. The trial-wise file also outputs two additional variables: WorkspaceX and WorkspaceY. These two variables define the quadrant in which the line appeared. For example, ***left*** (WorkspaceX) and ***bottom*** (WorkspaceY).<br>
- **LBT_[yourID_yourGender].mat**<br>Contains raw trial-wise data with x and y cursor position data. Note that you will only be able to open this file if you have MATLAB installed on your machine.<br>
- **log_[mm-dd-yyyy-hh-mm].txt**<br>Log file containing outputs from the MATLAB command window. Will contain any errors in running the app. If no errors, it will report the mean and sd of percent deviation from the center and total time taken to complete the test.<br>
- **LBT_[yourID_yourGender_trial#].jpeg**<br> Low-res image files for each trial showing participant performance.

See here for an [example data folder](https://github.com/rinivarg/cLBT/tree/master/example/LBT_051020rv_F)
****
</details> 

## Questions/Comments?<br>
- If you have any questions or suggestions for improvement, please post them through Issues. <br>
- You can also contact the first author directly at rinivarg_at_usc_dot_edu

## References<br>
1. **Schenkenberg T, Bradford DC, Ajax ET.** [Line bisection and unilateral visual neglect in patients with neurologic impairment.](https://github.com/rinivarg/cLBT/blob/master/LBT_Schenkenberg_1980.pdf) *Neurology.* 1980;30:509–17. 

## How to cite this?
**Varghese, R, Ma, J, and, Winstein CJ.** (May 9, 2020). A Computerized Version of the Line Bisection Test (v.1.2). GitHub. GitHub repository: https://github.com/rinivarg/cLBT/#667c1f6

	@misc{Varghese2020,
	  author = {Varghese, Rini, Ma, Jasmine, and Winstein, Carolee},
	  title = {A Computerized Version of the Line Bisection Test},
	  year = {2020},
	  publisher = {GitHub},
	  journal = {GitHub repository},
	  howpublished = {\url{https://github.com/rinivarg/cLBT}},
	  commit = {#667c1f6}
	}
