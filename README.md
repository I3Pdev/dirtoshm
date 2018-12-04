# dirtoshm  
Move directories to a RAMdisk to speed up app start times.  

DirToShm: Move directories to a RAMdisk to speed up app start times.  

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

Starting / Stopping the service:  
>  service dirtoshm start | stop  

Updates:  
>  https://github.com/I3Pdev/dirtoshm/release  

Packaging:  
>  Downloads source  
>  Move all directories except README.md, license and release folder into one folder called dirtoshm  
>  run `fakeroot dpkg-deb --build dirtoshm`
