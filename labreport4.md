# Lab Report 4 
## Step 1,2,3
* Delete any existing forks of the repository existing on my account.
* Fork the repository.
* Start the timer!

## Step 4-Log into ieng6
**Key pressed**: `"ssh" <space> "cse15lsp23fh@ieng6.ucsd.edu" <enter>` Log into UCSD ieng6 using my own account, since lab7 taught us how to set no-password login so no password is required now.

## Step 5-Clone your fork of the repository from your Github account
**Key pressed**: `"git" <space> "clone" <space> <command+v>` Using git clone to copy my fork of lab7 to my ieng6 account. Since I have already copy the link of the fork on my Github account, I directly paste it on my terminal.

## Step 6-Run the tests, demonstrating that they fail
**Key pressed**: `"cd" <space> "lab7" <enter>`change directory to lab7 to access the files, `"bash' <space> "test.sh" <enter>` run the shell file which is used to run the JUnit tests.

## Step 7-Edit the code file to fix the failing test
**Key pressed**: 
* `"vim" <space> "ListExamples.java" <enter>` enter the vim editor, now in normal mode of file *ListExamples.java*.
* `"?" "index1" <enter>` since the prompt told us where the error comes from, I use "?" which is searching backwards and find the line I should edit(since this "index1" is the last occurrence of index1, I don't have to press "n" to continue searching).
* `"dw" <enter>` deleting the word "index1".
* `"i"` entering insert mode, `"index2"` changing index1 to index2, `<esc>` exiting the insert mode, `":wq" <enter>` save and exit the vim.

## Step 8-Run the tests, demonstrating that they now succeed
**Key pressed**: `<up><up><up><enter>`since I ran the "test.sh" before, it is 3 command lines above(I used vimtutor during the task so there's one more line), so I pressed <up> for 3 times and run the test again.

