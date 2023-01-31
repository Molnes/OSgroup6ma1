# Mandatory assignment 1 Operating Systems
This repository contains the mandatory assignment 1 for the course [IDATA2305 - Operating Systems with System Programming](https://www.ntnu.edu/studies/courses/IDATA2305#tab=omEmnet) at NTNU.  

## Assignment
Simple single and multithreaded web server. We chose to solve the assignment in rust.  

## How to run
You can either compile the code yourself or use the precompiled binaries in the [releases](https://github.com/JakobHolkestadMolnes/OSgroup6ma1/releases).  
In order to compile you will need cargo installed.  

In order to run, simply run the binary with arguments, `single` or `multi`.  
`$ ./osgroup6ma1 [single|multi]`  

## Our observations
The single threaded server cannot handle multiple requests at the same time. If we refresh the page quickly multiple times, we need to wait for all the requests to finish before we can see the page again.  
The multi threaded server can handle multiple requests at the same time. If we refresh the page quickly multiple times, we can see the page again immediately (when the heavy task finishes).