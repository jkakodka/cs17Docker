# Development environment setup
If you are a VScode user , you can use this docker extension(https://code.visualstudio.com/docs/containers/overview) to browse and modify files that you create within your contianer.

1. The script in this directory "cs17-run-docker" is a wrapper script for docker run commands. It creates a container named "cs17_container".

2. Your docker container uses volume mounting. In short , once you start working within a container(ex you create files,folders,modify them) , these changes would remain persistent in between container reruns, restarts. If you have two or more simultaneous containers running , the changes you make to the files would be reflected across all of the containers.

3. You can either do a "./cs17-run-docker"  or
 "./cs17-run-docker restart" incase you broke something and want a clean slate.

## HOW WOULD YOU KNOW IF YOU ARE WITHIN THE CONTAINER?
After running either of the cmd from (3) , if your shell prompt looks like below
    
    6eab4a8d519f:/home/node/app# 

    NOTE : The first sequence of digits could be any random HEX number. If you see the above, you know you are inside the container.

4. Once you are inside the container you can use bsb -init to create folders for your projects/assignments as specified in your course instructions.
   