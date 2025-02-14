<h1>
  <span class="headline">Intro to PowerShell Lab</span>
  <span class="subhead">Creating, Deleting, and Modifying Files</span>
</h1>

**Learning objective**: By the end of this exercise, students will be able to create, delete, and modify files using PowerShell commands.

## Commands to learn

Let's dive into file operations. PowerShell provides a set of commands that allow you to create, delete, and modify files.

- `New-Item -ItemType File`: Creates the specified file.
- `Remove-Item`: Deletes the specified file.
- `Copy-Item`: Copies the specified file or directory to the second specified file or directory.
- `Move-Item`: Moves the specified file or directory to the second specified file or directory.
- `Get-Content`: Displays the content of the specified file.
- `Set-Content`: Modifies the content of the specified file.

## Practice

1. You should be in the <code class="filepath">intro-to-powershell-lab</code> directory if you're not already.
2. Use the `New-Item` command to create a new file called <code class="filepath">sample.txt</code>.
3. Use the `Set-Content` command to add some text to the <code class="filepath">sample.txt</code> file, such as `"Hello, PowerShell!"` or whatever else you desire. You may need to look up how to accomplish this task.
4. Use the `Get-Content` command to display the content of the <code class="filepath">sample.txt</code> file. You may need to look up how to accomplish this task.
5. Use the `Copy-Item` command to create a copy of the <code class="filepath">sample.txt</code> file named <code class="filepath">sample-copy.txt</code>. You may need to look up how to accomplish this task.
6. Create a new directory called <code class="filepath">backup</code> inside the <code class="filepath">intro-to-powershell-lab</code> directory. You've done this before - what command should you use?
7. Use the `Move-Item` command to move the <code class="filepath">sample-copy.txt</code> file into the new <code class="filepath">backup</code> directory. You may need to look up how to accomplish this task. Note that the `Move-Item` command cannot create directories, which is why you had to create the directory first.
8. Use the `Remove-Item` command to delete the <code class="filepath">sample.txt</code>.
