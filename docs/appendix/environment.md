# Appendix: Environment


## Kali Linux 
- [Kali Tools Documentation](https://www.kali.org/tools/)



## Windows Subsystem for Linux

For information about using Kali via. WSL for the NCL competition, check out [this article from CryptoKait](https://cryptokait.com/2020/08/19/ncl-and-wsl-leaving-the-kali-vm-behind/).
If you want to install WSL, instructions can be found [here](https://learn.microsoft.com/en-us/windows/wsl/install). 
The Kali Linux installation on WSL is a [minimum install setup](https://www.kali.org/docs/troubleshooting/common-minimum-setup/). 
That means you'll probably want to [install Kali Linux Metapackages](https://www.kali.org/docs/general-use/metapackages/).



## Python Virtual Environments
 
Python documentation on how to create a virtual environment with `venv` can be found [here](https://docs.python.org/3/library/venv.html).
Information on installing packages with `pip` in a virtual environment can be found [here](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).



## Background Commands and Persistent Sessions

To run a command in the background, add ampersand to the end of the command:
```bash
command &
```
To suppress the `stdout` and `stderr` messages, use:
```bash
command > /dev/null 2>&1 &
```
To display the status of all stoped and background jobs in the current shell session:
```bash
jobs -l
```
To bring a background process to the foreground, use the `fg` command (or `fg %1` if you have multiple background jobs.

To terminate the background process, use the `kill` command followed by the process ID (which can be obtained through the `jobs -l` command, above. In this example it's 12928):
```bash
kill -9 12928
```

Generally, if connection drops or you exit the shell session, the background process terminates. 
To keep the process running, use the `disown` command or start the process with the `nohup` command.

Alternatively, use [Tmux](https://linuxize.com/post/getting-started-with-tmux/) ("terminal multiplexer") to switch between multiple programs in one terminal. 
Tmux sessions are persistent; programs will continue to run even if you exit the shell or are disconnected.




