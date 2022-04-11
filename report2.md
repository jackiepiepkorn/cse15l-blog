# **Week 2 Lab Report**

## How do I log into a course-specific account on ieng6?
### Follow these steps!
### 1) Installing VS Code
I already had VS Code installed, but when I first installed it last quarter, I googled "VS Code" and clicked [this link](https://code.visualstudio.com/). I then clicked download for Windows and followed the instructions it gave me. Here's a picture of VS code open on my computer:

![Image](https://i.imgur.com/ltEuYS4.png)

### 2) Remotely Connecting
Next, you should open the terminal in VS Code. Type in `ssh cs15lsp22zzz@ieng6.ucsd.edu` into the terminal. (Replace _zzz_ with your specific username, which you can find on the [ACS Website](https://sdacs.ucsd.edu/~icc/index.php)). Then, type in the password that you reset on the ACS website prior to this. It's normal for it to look like you're not actually typing anything; that's the ssh's way of password protecting! Here's what mine looked like after login:

![Image](https://i.imgur.com/iAKCJT7.png)

### 3) Trying Some Commands
You can test out some commands that will help you become a more efficient programmer. One command I tested out was list files in your directory, which is `ls`. Try inputting that into your terminal. Here's a screenshot of what happened after I pressed enter: ![Image](https://i.imgur.com/Y8ImhqU.png)

### 4) Moving Files with scp
Let's try moving a file from your computer to a local computer! Make a file or choose a file you want to move. Then, type this into your terminal: `scp examplefile.java cs15lsp22zzz@ieng6.ucsd.edu:~/` Remember to replace _zzz_ with your personal ID. Input your password when prompted, and then try logging in with ssh. To see if the file transferred, do the `ls` command and see if it's there in your directory! Here's what showed up for me: ![Image](https://i.imgur.com/K3j1IYZ.png)

### 5) Setting an SSH Key
Want to use a trick to not have to input your password every time? Enter this code in the terminal:

```
# on client (your computer)
$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key
(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa
Enter passphrase (empty for no passphrase):
```
Make sure you press enter when it says _Enter passphrase_. If you have a Windows device, follow these additional instructions: [Windows SSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation)!

Look, it didn't ask for my password and just logged me in! ![Image](https://i.imgur.com/4zKVVyR.png)

### 6) Optimize Remote Running

One way I optimized the remote running was using the up arrow to basically and paste the last thing I entered into the terminal. Another thing I did was run the `ls` command on the same line as logging into ssh, with this code: `ssh cs15lsp22zzz@ieng6.ucsd.edu`
Here's what happened when I successfully optimized remote running:

![Image](https://i.imgur.com/Bq5wisQ.png)