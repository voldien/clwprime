# clwprime #
---------------------------
*clwprime* is a program for solving if *p* is a prime or not by using Wilson's theorem. It solves it with parallel computation. Reducing the time complexity for bigger *p* than if it were to be computed with serial computation.

## Examples ##
------------
1. Check if 13 is prime. Returns 1 if true or 0 if false.
```
clwprime 13
```
2. Check if 13 is prime. Will print the result in a human readable format.
```
clwprime 13 -h
```
3. Check if piped 13 is prime.
```
echo '13' | clwprime 
```


## Dependencies ##
----------------
In order to compile the program, the following Debian packages has to be installed.
```bash
apt-get install opencl-headers
```
Because each graphic card vendor has their own driver for implementing OpenCL. You'll have check what packet has to be installed for what graphic card on host in order for the OpenCL to be installed on the system.

The *clinfo* programmed can be installed with apt-get. It will display information about each OpenCL compatible devices on the host. If not information is displayed, then either there is not OpenCL compatible devices or the driver is not installed.