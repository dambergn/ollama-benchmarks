# Raspberry Pi 5
## Hardware Specifications
- Broadcom BCM2712 2.4GHz quad-core 64-bit Arm Cortex-A76 CPU, with Cryptographic Extension, 512KB per-core L2 caches, and a 2MB shared L3 cache
- 8Gb LPDDR4X-4267
  - Frequency: 4267 MHz
  - Memory Buss: 32 bit
  - Bandwidth: 9590.72 MiB/sec
- Power Usage in Watts
  - Idle: 4W
  - Load: 11W


## CPU Benchmark Results
| | | Raspberry Pi 5 |
| ---------------- | ------ | ---- |
|                  | Memory | TPS   |
| Llama3.2:1b      | 2.2 GB | 7.69  |
| Llama3.2:3b      | 3.5 GB | 3.25  |
| Deepseek-R1:1.5b | 1.6 GB | 8.86  |
| Deepseek-R1:7b   | 5.5 GB | 1.53  |
| Deepseek-R1:8b   | 6.5 GB | 1.43  |
| Deepseek-R1:14b  |        | N/A   |
| Deepseek-R1:32b  |        | N/A   |
| Deepseek-R1:70b  |        | N/A   |
| Deepseek-R1:671b |        | N/A   |
| Qwen2.5:0.5b     | 820 MB | 20.35 |
| Qwen2.5:1.5b     | 1.6 GB | 7.49  |
| Qwen2.5:3b       | 2.6 GB | 3.59  |
| Qwen2.5:7b       | 5.5 GB | 1.61  |
| Qwen2.5:14b      |        | N/A   |
| Qwen2.5:32b      |        | N/A   |
| Qwen2.5:72b      |        | N/A   |
| phi3:3.8b        | 6.0 GB | 2.6   |
| phi3:14b         |        | N/A   |
| gemma2:2b        | 3.1 GB | 4.2   |
| gemma2:9b        |        | N/A   |
| gemma2:27b       |        | N/A   |