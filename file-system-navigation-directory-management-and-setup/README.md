<h1>
  <span class="headline">Intro to PowerShell Lab</span>
  <span class="subhead">File System Navigation, Directory Management, and Setup</span>
</h1>

**Learning objective:** By the end of this exercise, students will be able to navigate the file system and manage directories using basic PowerShell commands.

## Commands to learn

PowerShell provides a set of intuitive commands for navigating and managing the file system. Let's explore some essential commands that will help you move around and organize your directories with ease. PowerShell commands are referred to as *cmdlets*, although the terms are often used interchangeably - they're the building blocks of PowerShell scripts.

- `Get-Location`: Displays the current working directory.
- `Set-Location`: Changes the current working directory to the specified directory.
- `New-Item -ItemType Directory`: Creates a new directory with the specified name.
- `Remove-Item`: Deletes the specified directory or file.
- `Rename-Item`: Renames the specified directory or file.

Notice how these commands follow a consistent pattern: `Verb-Noun`. The `Verb` describes the action you want to perform, and the `Noun` specifies the target of that action.

> 💡 As you complete this lab you may need to look up commands on the internet to get more information about them.

## Setup

Follow the steps below to set up your PowerShell environment and prepare for the lab exercise.

1. Launch your Terminal application. 
  - If you're using Windows, this will be the Powershell terminal. 
  - If you're using a Mac, you'll want to ensure Powershell is installed on your terminal. You can do this by running `brew install --cask powershell` in your terminal
    
2. Open a PowerShell console using the `pwsh` command.

3. Use `Get-Location` to display your current working directory.

4. Use `Set-Location` to navigate to a different directory. Navigate to the <code class="filepath">~/code/ga/labs</code> directory by providing it as an argument.

5. Use `Get-Location` to verify that you are in the correct directory.

6. After verifying you're in the correct location, use `New-Item -ItemType Directory` to create a new directory. Name the directory <code class="filepath">ps-lab</code> by providing that name as an argument to the command as shown below:

   ```powershell
   New-Item -ItemType Directory "ps-lab"
   ```

7. Use `Rename-Item` to rename the <code class="filepath">ps-lab</code> directory to <code class="filepath">intro-to-powershell-lab</code> by providing the current path to the item as the first argument and the new name for that item as the second argument.

   > 🧠 More complex commands, such as `Rename-Item` have parameters that may either be required or can help label positional items in a command. For example the above command to rename an item could be written as:
   >
   > ```powershell
   > Rename-Item "./ps-lab" "intro-to-powershell-lab"
   > ```
   >
   > or as:
   >
   > ```powershell
   > Rename-Item -Path "./ps-lab" -NewName "intro-to-powershell-lab"
   > ```

8. Use `Set-Location` to move into the <code class="filepath">intro-to-powershell-lab</code> directory.

### Git and GitHub setup

Git commands work like they do in Bash, so you can use the same commands you're familiar with to work with Git in PowerShell.

1. Initialize a new Git repository with these commands:

   ```bash
   git init
   git add .
   git commit -m "initial commit"
   ```

2. Create a new repository on [GitHub](https://github.com) named `intro-to-powershell-lab`.

3. Link your local repo to the remote GitHub repo:

   ```bash
   git remote add origin https://github.com/<github-username>/intro-to-powershell-lab.git
   git push origin main
   ```

   > 🚨 Do not copy the above command. It will not work. Your GitHub username will replace `<github-username>` (including the `<` and `>`) in the URL above.

4. When the time comes, don't forget to push your final code to GitHub!
