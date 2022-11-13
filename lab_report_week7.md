# Part 1
```
/start <enter>
```
![Image](lab7pic\search_start.PNG)


Searching Start and move the cursor to the start of "start"

```
ce
```
![Image](lab7pic\ce.PNG)


Delete the Start and enter insert mode

```
base<escape>
```
![Image](lab7pic\base_escape.PNG)


enter in the new word "base" and escape to normal mode
```
n
```
![Image](lab7pic\n_1.PNG)


press n to find the next "start" in the file
```
.
```
![Image](lab7pic\redone1.PNG)


And . means repeat the last modification which is delete "start" and insert "base"

```
n
```
![Image](lab7pic\n_2.PNG)


press another n to find the last "start" in the file

```
.
```
![Image](lab7pic\redone2.PNG)


Press . which repeat the modification of delet "start" and insert "base"

```
:wq 
```
![Image](lab7pic\wq.PNG)


Save and exit the vim.

```
<enter>
```
![Image](lab7pic\enter_finish.PNG)


after enter, you exit out of the mode.

# Part 2

## SCP method
It took me 31 seconds to edit a file localy and scp it to the server and go to the remot server to test it

The difficulties is that you need to log in to the remot after you scp the file. This can take longer time.

## ssh session
It took me 29 second to edit a file in the remot server using vim and test it

The difficulties is getting familiar with vim especially remembering to save and exit.

## Answer to the Question

1. I personally prefer the second one, I think with enough practice using vim, then I don't need to log in to run the bash file after every change I make to the file.

2. If I am only editing multiple files at the same time, I proabbly would use the local method, since I can see every code files I have and easily edit them without using vim to different files in the remot server.
