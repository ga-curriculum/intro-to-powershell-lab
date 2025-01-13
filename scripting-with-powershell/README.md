<h1>
  <span class="headline">Intro to Powershell</span>
  <span class="subhead">Scripting with Powershell</span>
</h1>

**Learning objective:** In this exercise, you'll write and execute a simple PowerShell script to automate a routine task.

Scripting is where the true power of PowerShell shines. By combining the commands you've learned so far, you can create scripts to automate repetitive tasks and streamline your workflow. Let's create a simple script to get you started. ✨

## Steps

1. Open a PowerShell console and navigate to the `PSLab` directory.
2. Create a new file called `SystemInfo.ps1` using `New-Item -ItemType File`.
3. Open the `SystemInfo.ps1` file in a text editor, such as PowerShell ISE or Visual Studio Code.
4. Add the following code to the script:

``` powershell
# Display computer system information
Write-Host "Computer System Information:"
Get-ComputerInfo | Select-Object -Property CsName, OsName, OsVersion, CsProcessors, CsPhyicallyInstalledMemory

# Display a list of running processes
Write-Host "Running Processes:"
Get-Process | Select-Object -Property Name, Id, CPU, WorkingSet
```

5. Save the script and close the text editor.
6. Execute the script by running `.\SystemInfo.ps1` in the PowerShell console.

**Congratulations!** You've just written and executed your first PowerShell script. The script retrieves computer system information and displays a list of running processes. You can customize and expand this script to automate various tasks based on your needs.
