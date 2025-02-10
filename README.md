# ollama-benchmarks
A list of benchmark results based on hardware and models I have tested.

## Benchmark Results
| |        | Raspberry Pi 4 | Raspberry Pi 5 | 4060Ti | P40 | 2xP40 | 2xXeonHT |
| ---------------- | ------ | ---- | ----- | ------ | ------ | ----- | ----- |
|                  | Memory | TPS  | TPS   | TPS    | TPS    | TPS   | TPS   |
| Llama3.2:1b      | 2.2 GB | 2.55 | 7.69  | 130.12 | 111.72 |       | 27.89
| Llama3.2:3b      | 3.5 GB | 1.5  | 3.25  | 92.21  | 68.60  |       | 15.27
| Llama3.3:70b     | 49 GB  | N/A  | N/A   | N/A    | N/A    | 5.40  | 1.01 
| Deepseek-R1:1.5b | 1.6 GB | 3.13 | 6.48  | 138.31 | 98.51  |       | 27.36
| Deepseek-R1:7b   | 5.5 GB | 0.76 | 1.53  | 48.38  | 39.27  |       | 10.32
| Deepseek-R1:8b   | 6.5 GB | 0.7  | 1.43  | 45.41  | 38.06  |       | 9.44
| Deepseek-R1:14b  | 11 GB  | N/A  | N/A   | 25.25  | 21.12  |       | 4.94
| Deepseek-R1:32b  | 23 GB  | N/A  | N/A   | N/A    | 8.62   |       | 2.25
| Deepseek-R1:70b  | 49 GB  | N/A  | N/A   | N/A    | N/A    | 5.29  | 1.18
| Deepseek-R1:671b |        | N/A  | N/A   | N/A    | N/A    | N/A   |
| Qwen2.5:0.5b     | 820 MB | 7.92 | 20.35 | 201.73 | 127.44 |       |
| Qwen2.5:1.5b     | 1.6 GB | 3.54 | 7.49  | 136.27 | 94.64  |       |
| Qwen2.5:3b       | 2.6 GB | 1.74 | 3.59  | 86.67  | 65.41  |       |
| Qwen2.5:7b       | 5.5 GB | 0.78 | 1.61  | 48.80  | N/A    |       |
| Qwen2.5:14b      | 11 GB  | N/A  | N/A   | 25.71  | 22.25  |       |
| Qwen2.5:32b      | 23 GB  | N/A  | N/A   | N/A    | 10.94  |       |
| Qwen2.5:72b      | 52 GB  | N/A  | N/A   | N/A    | N/A    | N/A   | 1.11
| phi3:3.8b        | 6.0 GB | 1.51 | 2.6   | 87.81  | 80.33  |       |
| phi3:14b         | 11 GB  | N/A  | N/A   | 29.68  | 29.79  |       |
| gemma2:2b        | 3.1 GB | 1.94 | 4.2   | 92.01  | 66.95  |       |
| gemma2:9b        | 9.4 GB | N/A  | N/A   | 36.91  | 31.90  |       |
| gemma2:27b       | 20 GB  | N/A  | N/A   | N/A    | 14.32  |       |
