# Assignment-1
Assignment 1 for CMPE 283 Course

- Team Details: 
   `Done by Myself`
   
- Describe in detail the steps you used to complete the assignment:
   In order to identify the virtualization features present in the CPU, a kernel module is constructed in this assignment and it reads various MSR values.
   I use Ubuntu as my OS for this assigment.
   
   Steps followed to complete assignment
   
  - Incorporated Makefile and the source code from `assi1.c` into a directory that was just established.
  - Installed packages like make, gcc and unzip
  - From there, four additional instances of the capability info structs were made, as follows:
       - `primary_proc_based`
       - `secondary_proc_based`
       - `exit_based`
       - `entry_based`

  - These examples include the bit number and a description of the characteristic that bit stands for.
  - Report capabilities function was modified to call it four more times with the proper `parameters`, `displaying proc`, `exit`, and `entry-based ` capabilities.
  - Added the `MODULE LICENSE()` function, which is necessary for module compilation. Commit displaying these adjustments is:https://github.com/AkashRupapara/CMPE283-Assignment-1/commit/4920099d7391bfcd05949be7a61889d6766ce62a

  - The module was compiled using the make command once the code had been modified. This created the file `assi1.ko`, a kernel object that may be loaded.
  - The following commands were used to install and unload kernel modules:
        `sudo insmod assi1.ko` this command loads module into kernel
        `sudo rmmod assi1.ko` this command unloads module into kernel 
  - To view the output of the kernel logs on a terminal, use the dmesg tool. The module's output is as follows:

<img width="1512" alt="Screen Shot 2022-11-07 at 2 41 22 PM" src="https://user-images.githubusercontent.com/29530515/200431020-044dc082-72b1-4c0d-ae75-2f502aeeffef.png">
<img width="1512" alt="Screen Shot 2022-11-07 at 2 41 29 PM" src="https://user-images.githubusercontent.com/29530515/200431027-a5490ecd-c133-46ba-80bf-68b04a4ed300.png">


<img width="1510" alt="Screen Shot 2022-11-07 at 2 46 30 PM" src="https://user-images.githubusercontent.com/29530515/200431545-3b2ae84f-26b6-4c6e-aefd-624916b25592.png">
