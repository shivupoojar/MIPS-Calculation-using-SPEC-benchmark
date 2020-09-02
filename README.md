# MIPS-Calculation-using-SPEC-benchmark
This project will explain to calculate the MIPS of the x86 system
OS used for testing: ubuntu 18.0.LTS

Tools required :

perf (Refer: http://www.brendangregg.com/perf.html#CPUstatistics)

sudo apt-get install  linux-tools-generic linux-tools-4.15.0-72-generic

sysbench(Refer: https://www.howtoforge.com/how-to-benchmark-your-system-cpu-file-io-mysql-with-sysbench)

sudo apt-get install sysbench

Testing:

sudo perf stat -C 1 sysbench --test=cpu run

Using output of the command calculate IPS(Instructions per second) 

IPS = instructions * time


