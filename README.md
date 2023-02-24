![](LOGO.png)

# ZBASH 

> zbash, a non-interactive bash wrapper


![https://img.shields.io/github/v/release/nickmitchko/zbash](https://img.shields.io/github/v/release/nickmitchko/zbash)

---

## Getting Started

```cos
%SYS> zpm "install zbash"
// OR
zpm:%SYS> install zbash
```

## Run bash command

```cos
%SYS> zbash "echo hello"

%SYS> zbash "whereis ssh"

%SYS> zbash "ps aux | grep irisdb"
```

## Support for interactive features

* This is a wrapper around `/bin/bash -c "command" 2>&1`
* Wrapper means that your command is executed and you get the output. There is no TTY or input.
* No guarantees that all commands work
  * For example, any interactive command needs a helper program, such as `sshpass` for ssh connections.


```

          _____                    _____                    _____                    _____                    _____          
         /\    \                  /\    \                  /\    \                  /\    \                  /\    \         
        /::\    \                /::\    \                /::\    \                /::\    \                /::\____\        
        \:::\    \              /::::\    \              /::::\    \              /::::\    \              /:::/    /        
         \:::\    \            /::::::\    \            /::::::\    \            /::::::\    \            /:::/    /         
          \:::\    \          /:::/\:::\    \          /:::/\:::\    \          /:::/\:::\    \          /:::/    /          
           \:::\    \        /:::/__\:::\    \        /:::/__\:::\    \        /:::/__\:::\    \        /:::/____/           
            \:::\    \      /::::\   \:::\    \      /::::\   \:::\    \       \:::\   \:::\    \      /::::\    \           
             \:::\    \    /::::::\   \:::\    \    /::::::\   \:::\    \    ___\:::\   \:::\    \    /::::::\    \   _____  
              \:::\    \  /:::/\:::\   \:::\ ___\  /:::/\:::\   \:::\    \  /\   \:::\   \:::\    \  /:::/\:::\    \ /\    \ 
_______________\:::\____\/:::/__\:::\   \:::|    |/:::/  \:::\   \:::\____\/::\   \:::\   \:::\____\/:::/  \:::\    /::\____\
\::::::::::::::::::/    /\:::\   \:::\  /:::|____|\::/    \:::\  /:::/    /\:::\   \:::\   \::/    /\::/    \:::\  /:::/    /
 \::::::::::::::::/____/  \:::\   \:::\/:::/    /  \/____/ \:::\/:::/    /  \:::\   \:::\   \/____/  \/____/ \:::\/:::/    / 
  \:::\~~~~\~~~~~~         \:::\   \::::::/    /            \::::::/    /    \:::\   \:::\    \               \::::::/    /  
   \:::\    \               \:::\   \::::/    /              \::::/    /      \:::\   \:::\____\               \::::/    /   
    \:::\    \               \:::\  /:::/    /               /:::/    /        \:::\  /:::/    /               /:::/    /    
     \:::\    \               \:::\/:::/    /               /:::/    /          \:::\/:::/    /               /:::/    /     
      \:::\    \               \::::::/    /               /:::/    /            \::::::/    /               /:::/    /      
       \:::\____\               \::::/    /               /:::/    /              \::::/    /               /:::/    /       
        \::/    /                \::/____/                \::/    /                \::/    /                \::/    /        
         \/____/                  ~~                       \/____/                  \/____/                  \/____/         
                                                                                                                             

Welcome to the zbash help page!

zbash is a command shortcut that allows you to execute a command in a Bash shell without having to manually enter the shell. This can be useful if you need to quickly execute a command or if you prefer to work in a Bash environment.

Usage:
zbash "[command]"

Examples:

    zbash "ls" : Execute the ls command in a Bash shell
    zbash "python script.py" : Execute a Python script in a Bash shell
    zbash "cd /path/to/directory && python script.py" : Change the current working directory in a Bash shell

Notes:

    The zbash command will automatically start a new Bash shell for each invocation.
    zbash does not support user input.
    To exit the Bash shell and return to the previous shell, type 'exit' at the Bash prompt.

I hope this information helps you use zbash effectively. If you have any further questions or concerns, please consult the Bash documentation.
```