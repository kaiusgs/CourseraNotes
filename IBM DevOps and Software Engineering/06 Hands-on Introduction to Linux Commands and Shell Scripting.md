# Hands-on Introduction to Linux Commands and Shell Scripting  
## Linux  
- Operating System (OS): is a software that manages hardware and resources, and allows interaction with hardware to perform useful tasks.  
- **Architecture**  
    ![five_layers](./static/06/five_layers.png)  
    - UI (User Interface): Allow users to interact with the machine.  
    - Applications: Softwares that let you perform a task. System tools, Programming languages, Shells, User apps.  
    - Operating System: Controls the jobs and programs vital to health and stability.  
        - Assigns software to users.  
        - Helps detect errors and prevent failures.  
        - Performs file management tasks.  
    - Kernel: lowest-level of software, starts on boot, perform vital operations, bridge between apps and hardware. Key jobs:  
        - Memory management  
        - Process management  
        - Device drivers  
        - Security  
    - Hardware: all physical and electronic devices. CPU, RAM, Storage, Screen, USB devices ...  
- **Shell**: an OS-level application that interprets commands.  
    - Terminal: an application used to interact with shell.  
    ![shell](./static/06/shell.png)  
- **File editing with Vim**  
    ![vim](./static/06/vim.png)  
    > [Runoob Linux Vim](https://www.runoob.com/linux/linux-vim.html)  
    > ![vim_vi](./static/06/vim_vi.png)  
- Pakages  
    ![deb_rpm](./static/06/deb_rpm.png)  
    ![upgrade_install_pkg](./static/06/upgrade_install_pkg.png)  
## Commands  
> [WikiPedia of Unix command](https://en.wikipedia.org/wiki/List_of_POSIX_commands)  

![getting_information](./static/06/getting_information.png)  
`tldr` - similar to `man` but not verbose  
`date -r myfile.txt` - to verify the change date of a file  
    ![which](./static/06/which.png)  
![working_with_files](./static/06/working_with_files.png)  
    ![chmod](./static/06/chmod.png)  
    ![wc](./static/06/wc.png)  
![working_with_dirs](./static/06/working_with_dirs.png)  
    ![ls_command](./static/06/ls_command.png)  
    `-R` - recursively list all files and folders  
    ![finding_files](./static/06/finding_files.png)  
![printing_files](./static/06/printing_files.png)  
    ![less](./static/06/less.png)  
    ![sort](./static/06/sort.png)  
    ![uniq](./static/06/uniq.png)  
    ![grep](./static/06/grep.png)  
    ![grep1](./static/06/grep1.png)  
    ![cut](./static/06/cut.png)  
    ![cut2](./static/06/cut2.png)  
    ![paste](./static/06/paste.png)  
![files_compression](./static/06/files_compression.png)  
`tar -cf xxx.tar folder` - archive  
`tar -tf xxx.tar` - list archive contents  
`tar -xf xxx.tar folder` - extract  
`tar -czf xxx.tar.gz folder` - archive and compress  
`tar -xzf xxx.tar.gz folder` - decompress and extract  
    ![zip](./static/06/zip.png)  
    `unzip -l xxx.zip` - list files of the zip archive  
    ![unzip](./static/06/unzip.png)  
![networking](./static/06/networking.png)  
> `sudo apt update`  
> `sudo apt install iproute2`  

`ip a` - display system network interfaces  
`ip addr show eth0` - display details for a specific device (eth0)  
>
    > ![host_clients_servers](./static/06/host_clients_servers.png)  
    > ![packets_pings](./static/06/packets_pings.png)  
    > ![ip](./static/06/ip.png)  

## Shell Scripting  
- Shebang  
![shebang](./static/06/shebang.png)  
![shebang1](./static/06/shebang1.png)  
- Variable  
    ![shell_variable1](./static/06/shell_variable1.png)  
    - no spaces around "="  

    ![shell_variable2](./static/06/shell_variable2.png)  
    - `unset var_name` - deletes a variable   
    - `export var_name` - extends a variable to an environment variable  
    - `set` - list all shell variables  
    - `env` - list all environment variables  
- Pipes  
    ![pipes_filters](./static/06/pipes_filters.png)  
    ![export](./static/06/export.png)  
    ![pipes_tr](./static/06/pipes_tr.png)  
    ![pipes_tr1](./static/06/pipes_tr1.png)  
    ![pipes_grep](./static/06/pipes_grep.png)  
- Script Quoting  
    ![quoting](./static/06/quoting.png)  
- I/O Redirection  
    ![io_red](./static/06/io_red.png)  
- Command Substitution  
    ![command_substitution](./static/06/command_substitution.png)  
- Execution Modes  
    ![execution_modes](./static/06/execution_modes.png)  
- Bash Scripting  
    - Conditionals  
    ![if_else](./static/06/if_else.png)  
    ![if_else1](./static/06/if_else1.png)  
    ![if_else2](./static/06/if_else2.png)  
    - Arithmetic calculations  
    ![arithmetic_calculations](./static/06/arithmetic_calculations.png)  
    - Arrays  
    `my_array=(1 2 "three" "four" 5)` - create an array  
    `declare -a empty_array` - create an empty array  
    `my_array+=("six")`  `my_array+=(7)` - add items to an array  
    ![arrays](./static/06/arrays.png)  
    - For Loop  
        ![for1](./static/06/for1.png)  
        - sum up an array's elements  

        ![for2](./static/06/for2.png)  
- Job Scheduling  
    ![crontab_syntax](./static/06/crontab_syntax.png)      
    - minute, hour, day of month, month, and day of week  

    ![crontab_syntax1](./static/06/crontab_syntax1.png)  
    - append the current date to the file ‘sundays.txt’ at 15:30 every Sunday  

    `crontab -l` - list all cron jobs  
    `crontab -r` - remove all cron jobs  
