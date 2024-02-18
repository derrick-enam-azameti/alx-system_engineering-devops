# Command line for the win
<img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/324/06AChAO.png" target="_blank">
CMD CHALLENGE is a pretty cool game challenging you on Bash skills. Everything is done via the command line and the questions are becoming increasingly complicated. It’s a good training to improve your command line skills!

## SFTP steps followed to upload files
### Connection
At the command prompt, type (without the $):
```console
$ sftp your_username@server_ip_or_remote_hostname
```
where:
`your_username` is your username
`server_ip_or_remote_hostname` is your server ip address or remote hostname

You will then be prompted for your password. Enter it.

### Successful Connection
Upon successful connection, your prompt changes to `sftp>`

### Getting Help
You can get a summary of helpful SFTP commands by typing `help` or `?` at the prompt:
```console
sftp> help
```
or 
```console
sftp> ?
```
NB: Don't type `sftp>`, it is the prompt you're expected to have.

### Navigating with SFTP
#### Remote Directory
Type the following at the `sftp>` prompt:
`pwd` - print remote working directory
`ls` - view contents of the remote directory
`cd` - change remote working directory

#### Local Directory
Type the following at the `sftp>` prompt:
`lpwd` - print local working directory on your computer
`lls` - view contents of your local directory
`lcd` - change your local working directory

# Specifics
- Thus, I used the `pwd` command to print my remote working directory and the `ls` command to list the files and direcotories in it.
- I then typed `cd alx-system_engineering-devops` to change my working directory to `alx-system_engineering-devops`
- I used `ls` to list the files in the `alx-system_engineering-devops` directory.
- I then typed `cd command_line_for_the_win` to change to that directory.
- I then used `lpwd` to print my local directory on my machine, and
- used `lcd` to navigate to the appropriate local directory where my screenshots are.
- I used `lls` to list them
- I used `put -r folderName` to upload all the contents of the folder and the folder itself
- I then exited (by typing `exit`) the sftp prompt since I have successfully uploaded them to my server.

- I then `ssh` to my server and moved the files from the uploaded folder to the `command_line_for_the_win` folder and deleted the uploaded folder.
- I used git to upload the files to my github repo.

[Image of steps followed on the commandline](https://github.com/derrick-enam-azameti/alx-system_engineering-devops/tree/master/command_line_for_the_win/process.png)


