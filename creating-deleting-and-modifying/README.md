<h1>
  <span class="headline">Intro to Powershell</span>
  <span class="subhead">Creating, Deleting, and Modifying Files</span>
</h1>

**Learning objective:** In this exercise, you'll learn how to create, delete, and modify files using PowerShell commands.

Let's dive into file operations. PowerShell provides a set of commands that allow you to create, delete, and modify files with ease.

## Commands to Learn

- `New-Item -ItemType File`: Creates a new file.
- `Remove-Item`: Deletes a file.
- `Copy-Item`: Copies a file or directory.
- `Move-Item`: Moves a file or directory.
- `Get-Content`: Displays the content of a file.
- `Set-Content`: Modifies the content of a file.

## Practice

1. In the `PSLab` directory, create a new file called `sample.txt` using `New-Item -ItemType File`.
2. Use `Set-Content` to add some text to the `sample.txt` file, such as `"Hello, PowerShell!"` or whatever you desire.
3. Display the content of the `sample.txt` file using `Get-Content`.
4. Create a copy of the `sample.txt` file named `sample_copy.txt` using `Copy-Item`.
5. Move the `sample_copy.txt` file to a new directory called `Backup` using `Move-Item`.
6. Delete the `sample.txt` file using `Remove-Item`.
