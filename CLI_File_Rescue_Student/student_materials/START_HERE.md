# CLI File Rescue

## Competency Mastery Activity

Your development team inherited a disorganized command-line game project. Your job is to rescue it **without using File Explorer, Finder, or an IDE's file browser**. You must inspect, reorganize, search, and run the project entirely from a Bash-compatible terminal.

## Rules

1. Work only inside the provided `project-rescue` directory.
2. Use a Bash-compatible terminal, such as Git Bash, Linux, macOS Terminal, or WSL.
3. Do not reorganize files with a graphical file manager or IDE file browser.
4. You may consult `man COMMAND` or `COMMAND --help`.
5. Do not delete a file until you have inspected enough information to know it is safe to delete.
6. Record the commands you use in `command-log.txt`.
7. Commands may vary. You are graded on the result and your ability to explain your choices.

## Mission

Start in the directory that contains `project-rescue`.

### Part 1: Orient yourself

1. Enter `project-rescue` using a relative path.
2. Print the full path of your current working directory.
3. List all items, including hidden items.
4. Find the hidden mission file and read it.
5. Locate and read the file whose name contains spaces.

### Part 2: Build the project structure

Create this directory structure inside `project-rescue`:

```text
project-rescue/
├── assets/
├── docs/
├── logs/
├── reports/
└── src/
```

Do not create a second `project-rescue` directory.

### Part 3: Rescue the files

6. Rename `old-app.py` to `app.py` and move it into `src`.
7. Move `helpers.py` into `src`.
8. Move `game-banner.svg` into `assets`.
9. Move `development.log` into `logs`.
10. Move `project notes.txt` into `docs` and rename it `project-notes.txt`.
11. Copy `README-original.md` into `docs`, renaming the copy `README.md`.
12. Move `command-reference.txt` into `docs`.
13. Inspect the two Python backup files. Remove only the obsolete backup identified by the hidden mission file. Leave the other backup where it is.

### Part 4: Search and analyze

14. Find every `.py` file below `project-rescue` and save the results in `reports/python-files.txt`.
15. Search `logs/development.log` for lines containing `ERROR` and save only those lines in `reports/errors-only.txt`.
16. Count the error lines and save the number in `reports/error-count.txt`.
17. Create `reports/unique-testers.txt` containing the tester names from `data/testers.txt`, alphabetized with duplicates removed. You must use a pipe.
18. Search the whole project recursively for `TODO` and save the matching lines, including filenames, in `reports/todos.txt`.

### Part 5: Run and verify

19. Navigate into `src` and run `app.py` with Python.
20. Return to the `project-rescue` root without closing the terminal.
21. Use terminal commands to verify the final contents of every directory.
22. Complete `command-log.txt`. Include at least one command that uses:
    - a relative path;
    - a path containing `..`;
    - `find`;
    - `grep`;
    - output redirection (`>` or `>>`); and
    - a pipe (`|`).

## Required final structure

```text
project-rescue/
├── .mission-clue.txt
├── assets/
│   └── game-banner.svg
├── command-log.txt
├── data/
│   └── testers.txt
├── docs/
│   ├── command-reference.txt
│   ├── project-notes.txt
│   └── README.md
├── logs/
│   └── development.log
├── mixed-files/
│   └── app-backup-working.py
├── README-original.md
├── reports/
│   ├── error-count.txt
│   ├── errors-only.txt
│   ├── python-files.txt
│   ├── todos.txt
│   └── unique-testers.txt
└── src/
    ├── app.py
    └── helpers.py
```

The order shown by your terminal may differ.

## Version Control

1. Create a local repository and give it an inital commit with the message "initial commit".
2. Make a small change to any of the log txt files and create a commit with a message that reflects the changes.
3. Connect the repo to a GitHub remote repo and add KramlichMHS as a collaborator.
4. On GitHub make a change to one of the .txt or .md files, then make a commit on the website.
5. Move back to your local repo and pull the changes from the remote.
6. Make more local changes to a log txt file and commit and push the commit to the remote repo.

Your final repo should have a git history that reflects all of the above steps.

## Submission

Create a .zip of the entire project-rescue directory and upload to Schoology. Make sure KramlichMHS is added as a collaborator on the remote repo.


## Mastery check

You should be able to explain what a command will do **before** running it. Accidentally reaching the correct final structure without being able to explain your commands does not demonstrate mastery.
