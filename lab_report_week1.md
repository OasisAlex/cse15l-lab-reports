First step:
Installing VScode
![Image](Lab1pic/VScode.JPG)
* Go to the website: [link] (https://code.visualstudio.com/)
* Personally already have it installed

Second step: Remotely Connecting
![Image](Lab1pic/DownSSH.png)
* download SHH by in Setting-Apps-Optional Feature; Add a feature and search for “OpenSSH Client”

![Image](Lab1pic/step_2.png)
* Find your account in [link]https://sdacs.ucsd.edu/~icc/index.php
* Open Terminal using Ctrl + ~
![Image](Lab1pic/ssh_type.png)
* Replace ga with your account
```
$ ssh cs15lfa22ga@ieng6.ucsd.edu
```
* Insert your password 
![Image](Lab1pic/sshcoonect.png)

step three:
![Image](Lab1pic/try.png)
* ls show your list of file of the current directory
* pwd show what's your current directory

step four:
![Image](Lab1pic/SCP.png)
* Use Scp to copy your file to server pc when you connect
* remember you are at the right directory of the file you want to copy to

Step five:
![Image](Lab1pic/Keu.png)
* don't put anything for passpharse , just do enter
* remember your are copying public key

Step six:
![Image](Lab1pic/Optimizing.png)
* run command using " " while accessing server
* You can use ; to seperate the commands and  run two or more command at the same time