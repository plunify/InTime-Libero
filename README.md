![alt text](images/Plunify_Logo_300.png)

# Run InTime in Tcl Mode (Libero)
This repository contains scripts to run InTime via its Tcl Console or on the command-line. There are 2 ways to run InTime using a Tcl script.
1. From a command-line shell
2. From the Tcl Console in the InTime GUI 

## Main Contents
1. [sample-designs](sample-designs/) : Quickstart designs for the various flows described here.
2. [scripts](scripts/) : Sample scripts to run InTime for each of these methods - command-line or InTime GUI. 

## Run InTime in Project Mode
Using a command-line shell, a typical way to start InTime is as showed below:

```intime.sh -mode batch -project <proj> -s intimeflow.tcl```

* For project mode, specify a PRJX file in the ```<proj>``` option.

*Sample projects and Tcl build scripts are available in the sample-designs folder.

## Requirements
1. Latest version of InTime.
2. Libero with an appropriate license properly registered in InTime. If you have not done so, refer to this [page](scripts/intime/configuration)

For more information about InTime, click [here](https://www.plunify.com/en/intime/). To learn more about the InTime GUI, refer to this [video](https://www.youtube.com/watch?v=lQvY_XZ3R7w).
