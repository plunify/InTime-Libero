# Using Tcl Scripts

Here is a sample Tcl script to run in InTime.
```Tcl
# Sample script for InTime Optimization. Works in Windows & Linux environments
# Adjust the run_target, runs_per_round and round variables according to your recipe
flow reset
flow set run_target private_cloud
flow set runs_per_round 40
flow set rounds 1
flow set concurrent_runs 10
flow set control_create_bitstreams false
flow run_recipe "intime_default"
```

Let's say you have saved the above as ```intimeflow.tcl```
To run InTime in commandline mode, execute the following command:
<InTime installation dir>/intime.sh -mode batch -platform minimal -project <your PRJX file> -vendor_toolchain libero -vendor_toolchain_version <e.g. 12.4> -s intimeflow.tcl

Explanation:

    -mode batch: Run in batch mode
    -platform minimal: Run in non-GUI mode
    -project: The project to open
    -vendor_toolchain: Name of the FPGA tool e.g. libero
    -vendor_toolchain_version: E.g. 12.4
    -s <Tcl script>: Tcl script to execute

# Sample Designs

```
### [Project mode](project_mode/)

Use the File > Open Example Project > Libero option in the InTime GUI to create a sample project.

