# dirtoshm  
Move directories to a RAMdisk to speed up app start times.  


Configuration:  
>  Usage: dirtoshmConfig [DIRECTORY]... | [ -h | --help ]  
>  Configure which directories dirtoshm moves to RAM.  
>
>  DIRECTORY has to be the ABSOLUTE path to the directory. It must not contain ~.  
>  Multiple directories can be specified, spaces in paths have to be quoted.  
>
>  If no directory specified, read from stdin.  
>
>  Exit status:  
>    0 if OK,  
>    1 if wrong arguments or aborted.  


Starting / Stopping the service (autostart at system startup after successful configuration):  
>  service dirtoshm start | stop  


Updates:  
>  https://github.com/I3Pdev/dirtoshm/release  


Packaging:  
>  Download source  
>  Move all directories except release (and except README.md and license) into one folder called dirtoshm  
>  (`apt install fakeroot dpkg-dev`)  
>  run `fakeroot dpkg-deb --build dirtoshm`  
