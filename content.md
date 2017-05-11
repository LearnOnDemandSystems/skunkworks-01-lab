
<!---
Version: 1.0 
-->

# Introduction to PowerShellGet

## INTRODUCTION MESSAGE
PowerShellGet is an extension of the Package Management feature in Windows PowerShell that facilitates the distribution and management of PowerShell modules. In this exercise, you will learn how to install and update modules that are available to PowerShellGet via the PowerShell Gallery.

## COMPLETION MESSAGE

### Install a module
Using PowerShellGet, find and install the **ProtectedData** module for all users.

#### :bulb: KNOWLEDGE
Hint \#1: Installing modules for all users with PowerShellGet requires elevation.

Hint \#2: The verbs for the commands you need can be found in the instructions for this task.

If you get stuck, review the video again, paying close attention to the list of commands that are shown near the end -- the command that you need to use can be found in that list.

If you're really stuck and just can't figure it out, click Done and the video in the next task will show you how this task can be completed.


#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 588654.mp4
>* ShowAutomatically = Once

### Install a module - solution
Click the **video camera** icon to view the solution, or click **Done** to continue with the next task.

#### :bulb: KNOWLEDGE
If you would like the solution entered for you, place your cursor at the PowerShell prompt and click on the **caret** icon.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 599205.mp4
>* ShowAutomatically = Once

#### :calling: COMMAND
```TypeText
Find-Module ProtectedData | Install-Module
```

### Update a module
Using PowerShellGet, update the **ImportExcel** module that was installed on this system with PowerShellGet.

#### :bulb: KNOWLEDGE
Hint \#1: As a reminder, you should be in an elevated PowerShell session.

Hint \#2: The verb required to perform this task is included in the task instructions.

The commands required to complete this exercise was displayed in the list of \*-Module commands you saw in the first video. You can review any video as many times as you like.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 588666.mp4
>* ShowAutomatically = Once

### Update a module - solution
Click the **video camera** icon to view the solution, or click **Done** to continue with the next task.

#### :bulb: KNOWLEDGE
If you would like the solution entered for you, place your cursor at the PowerShell prompt and click on the **caret** icon.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 599210.mp4
>* ShowAutomatically = Once

#### :calling: COMMAND
```TypeText
Update-Module ImportExcel
```

### Update a module that ships with Windows
Using PowerShellGet, update the **Pester** module that was automatically installed with Windows.

#### :bulb: KNOWLEDGE
Sometimes modules that ship with Windows are updated in between Windows releases. When this happens, the updates are usually shared in the PowerShell Gallery. Pester is one example of a module that ships with Windows that receives frequent updates on the PowerShell Gallery.

If you're stuck with this task, here's a hint: when you want to update a shipped module that has not been installed locally with PowerShellGet, you need to use the -Force.

If you're still stuck with this task and you tried using Update-Module already, note that the error you receive from Update-Module points you to the command you really need to be looking at.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 588685.mp4
>* ShowAutomatically = Once

### Update a module that ships with Windows - solution
Click the **video camera** icon to view the solution, or click **Done** to continue with the next task.

#### :bulb: KNOWLEDGE
If you would like the solution entered for you, place your cursor at the PowerShell prompt and click on the **caret** icon.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 599212.mp4
>* ShowAutomatically = Once

#### :calling: COMMAND
```TypeText
Install-Module Pester -Force
```

### Install a module with specific contents
Using PowerShellGet, find a module that contains the **Get-History** command that was written by Kirk Munro, and install it.

#### :bulb: KNOWLEDGE
Hint \#1: PowerShellGet supports discovery of modules that contain specific commands.  You just need to know how to *find* them (hint, hint).

Hint \#2: If you're stuck, have a closer look at the parameters in a command you would use to *find* a *module.*

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 588719.mp4
>* ShowAutomatically = Once

### Install a module with specific contents - solution
Click the **video camera** icon to view the solution, or click **Done** to continue with the next task.

#### :bulb: KNOWLEDGE
If you would like the solution entered for you, place your cursor at the PowerShell prompt and click on the **caret** icon.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 599215.mp4
>* ShowAutomatically = Once

#### :calling: COMMAND
```TypeText
Find-Module -Command Get-History | Where-Object Author -eq 'Kirk Munro' | Install-Module
```

### Submit your results for scoring
Once you are satisfied with your progress, click **Done** to submit your results for scoring.

#### :movie_camera: VIDEO
>LODSProperties
>* Uri = 589455.mp4
>* ShowAutomatically = Once