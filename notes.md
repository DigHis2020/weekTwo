Week two notes! 

I installed the Sublime text editor with literally no issues. It appears to be a very user-friendly application with simple controls. I'm interested to incorporate this into the course when I have the chance. 

I installed Conda and this presented several issues for me. 
I installed both the graphical installer and the command line installer from Python 3.7, but as the files were finishing, a notification appeared that said: 
"This type of file could harm your computer"
I exited the download in a panic. 

I tried again, the notification didn't appear. 
I went onto my terminal and entered the code:

conda --version 

and this appeared: conda --version
conda 4.8.2

Python version 3.7 was also installed. 

The WGET saga 

I added the given line of code to download Homebrew to my Mac. 

This entire paragraph appeared: 
Warning: The Ruby Homebrew installer is now deprecated and has been rewritten in
Bash. Please migrate to the following command:
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

I followed this new command and Homebrew began downloading, albeit very slowly. 
Massive walls of unintelligible code appeared, but the download continued, followed by a line that stated: 
Cloning into '/usr/local/Homebrew/Library/Taps/homebrew/homebrew-core'...

Some links that helped me along to this point were: 

https://discourse.brew.sh/t/password-when-installing-homebrew/226

https://github.com/Homebrew/brew/issues/4579

Ah yes, this appeared at the final second: 

error: RPC failed; curl 56 LibreSSL SSL_read: SSL_ERROR_SYSCALL, errno 54
fatal: the remote end hung up unexpectedly
fatal: early EOF
fatal: index-pack failed
Error: Failure while executing; `git clone https://github.com/Homebrew/homebrew-core /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core` exited with 128.
Error: Failure while executing; `/usr/local/bin/brew tap homebrew/core` exited with 1.

I looked at https://stackoverflow.com/questions/24952683/git-push-error-rpc-failed-result-56-http-code-200-fatal-the-remote-end-hun/36843260#36843260

It seems to have to have the solution but literally everything I read goes above my head. 
