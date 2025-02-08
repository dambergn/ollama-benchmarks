## Raspberry Pi 4
- Broadcom BCM2711, Quad core Cortex-A72 (ARM v8) 64-bit SoC @ 1.8GHz
- 1GB, 2GB, 4GB or 8GB LPDDR4-3200 SDRAM (depending on model)
- LPDDR4 memory at 3200MHz with 32bit width bus(It is a 3733MHz LPDDR4 memory running at 3200MHz

## Raspberry Pi 5
- Broadcom BCM2712 2.4GHz quad-core 64-bit Arm Cortex-A76 CPU, with Cryptographic Extension, 512KB per-core L2 caches, and a 2MB shared L3 cache
- LPDDR4X-4267 SDRAM (options for 2GB, 4GB, 8GB and 16GB)
- clock speed of 4267 MHz
### Memory Bandwidth Test Results
```
Running the test with following options:
Number of threads: 16
Initializing random number generator from current time


Running memory speed test with the following options:
  block size: 1KiB
  total size: 102400MiB
  operation: write
  scope: global

Initializing worker threads...

Threads started!

Total operations: 98130779 (9811807.06 per second)

95830.84 MiB transferred (9581.84 MiB/sec)


General statistics:
    total time:                          10.0002s
    total number of events:              98130779

Latency (ms):
         min:                                    0.00
         avg:                                    0.00
         max:                                   41.95
         95th percentile:                        0.00
         sum:                                96903.13

Threads fairness:
    events (avg/stddev):           6133173.6875/80713.34
    execution time (avg/stddev):   6.0564/0.18
```

## Memory Bandwidth Test
```
sudo apt-get update
sudo apt-get install memtester sysbench -y
nano test_memory_bandwidth.sh

#!/bin/bash
# Script to test memory bandwidth using memtester and sysbench

echo "Testing Memory Bandwidth..."
echo ""

# Test using memtester (if installed)
echo "Running Memtester Memory Test..."
memtester 8M 10 || true
echo ""

# Test using sysbench (if installed)
echo "Running Sysbench Memory Test..."
sysbench --test=memory --num-threads=16 run
echo ""

echo "Memory bandwidth tests completed."

#ctrl x y

chmod +x test_memory_bandwidth.sh

sudo ./test_memory_bandwidth.sh

```