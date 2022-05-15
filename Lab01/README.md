# Lab 1 - Exploring the Command Line
## Example Commands
* `hostname`
    * prints the name of the device that will be reported to the netowrk's dns server
    * ![hostname output](hostname.gif)
* `env`
    * prints currenly registered environment variables
    * ![env output](env.gif)
* `ps`
    * prints currently running process (note: generally more useful with `-aux` flags)
    * ![ps output](ps.gif)
* `pwd`
    * prints the current absolute working directory of the current command line isntance
    * ![pwd output](pwd.gif)
* `git clone https://github.com/kevinwlu/iot.git`
    * downloads the repository `https://github.com/kevinwlu/iot.git` into a folder named after the repository name (iot in this case) and initializes it for use with git
    * ![git output](git.gif)
* `cd iot`
    * changes the working dirctory (folder) that you are in to the given folder (in this case iot); No output is printed
    * ![cd output](cd.gif)
* `ls`
    * prints files in the current working directory
    * ![ls output](ls.gif)
* `cd`
    * changes working directory; when used with no parameters it changes to the parent directory
    * ![cd output](cd2.gif)
* `df`
    * prints current disk usage separated by partition
    * ![df output](df.gif)
* `mkdir demo`
    * makes a new directory with the name given (demo in this case); has no output
    * ![mkdir output](mkdir.gif)
* `cd demo`
    * see above `cd`
    * ![cd output](cd3.gif)
* `nano file`
    * opens "file" in the nano command line text editor; use `ctrl`+`x` to exit and you will be asked to save
    * ![nano output](nano.gif)
* `cat file`
    * prints the contents of "file" assuming current console text encoding
    * ![cat output](cat.gif)
* `cp file file1`
    * creates a copy of "file" at location "file1"
    * ![cp output](cp.gif)
* `mv file file2`
    * renames "file" to "file2" (if "file2" location is on same drive as "file") or copies "file" to location "file2" and then deletes "file" (if files are on different drives)
    * ![mv output](mv.gif)
* `rm file2`
    * deletes "file2" (does not use a "recylcing bin")
    * ![rm output](rm.gif)
* `clear`
    * clears output from the console's screen and sets up a new line at the top, history is still preserved
    * ![clear output](clear.gif)
* `man uname`
    * shows the manual page for the package "uname", uses the same controls/keyboard shortcuts as [`less`](https://www.man7.org/linux/man-pages/man1/less.1.html#COMMANDS)
    * ![man output](man.gif)
* `uname -a`
    * prints information obout the kernel, hostname, build date, arch, and operating system
    * ![uname output](uname.gif)
* `ifconfig`
    * shows all interfaces, their settings, and their connection status
    * [as noted by the linux foundation](https://wiki.linuxfoundation.org/networking/net-tools), `ifconfig` is obsolete in favor of `ip addr` (aliases `ip a` and `ip address`)
    * ![ifconfig output](ifconfig.gif)
* `ip a`
    * current replacement for `ifconfig`
    * ![`ip a` output](ipa.gif)
* `ping localhost`
    * sends a "ping" to the address specified (localhost in this case); used to determine if a host is resolvable and online (does not determine if ports are open)
    * ![ping output](ping.gif)
* `nestat`
    * shows network configuration of device (e.g. listening ports, requesting ports, services, etc.)
    * ![netstat output](netstat.gif)

## Commands I Find Useful

* `dotnet`
    * used for making and managing dotnet (C#, F#, and Visual Basic) projects
    * Example using the command: [Discord Bot Application](https://github.com/StevensIEEE/DiscordBotExampleCSharpRemora)
* `rsync`
    * used for syncing files between systems
    * using with `-avhzd` is good for archivingin and monitoring the process, along with `--delete-excluded` and `--exclude <pattern>` to remove any files that were deleted from the source and any files you don't want archived
* `systemctl`
    * for making and managing services that can be long running, running at startup, and automatically restarting
* `ffmpeg`
    * used for processing images and videos (e.g. transcoding, filtering, etc.)