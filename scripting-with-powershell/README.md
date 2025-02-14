<h1>
  <span class="headline">Intro to PowerShell Lab</span>
  <span class="subhead">Scripting with Powershell</span>
</h1>

**Learning objective:** In this exercise, you'll write and execute a simple PowerShell script to automate a routine task.

Scripting is where the true power of PowerShell shines. By combining the commands you've learned so far, you can create scripts to automate repetitive tasks and streamline your workflow. Let's create a simple script to get you started. ✨

## Steps

1. In your Powershell console, you should be in the <code class="filepath">intro-to-powershell-lab</code> directory if you're not already.

2. Create a new file called `get-system-processes.ps1` using `New-Item -ItemType File`.

3. Open the current directory in Visual Studio Code using `code .`.

4. Add code that will implement this functionality to the script:

   - Research the `Write-Host` cmdlet to display a message reading: "Running Processes:".

   - Use the `Get-Process` cmdlet to display a list of running processes. Research how to use the `Select-Object` cmdlet in combination with the `Get-Process` cmdlet to only show the `Name`, `Id`, `CPU`, and `WorkingSet` of each process.

5. Ensure the script is saved and close VS Code.

6. Execute the script by running `./get-system-processes.ps1` in the PowerShell console to test it.

   **Congratulations!** You've just written and executed your first PowerShell script. The script retrieves computer system information and displays a list of running processes. Scripts can be customized and expanded on to automate various tasks based on your needs.
