# Results: 208 iPerf3 TCP/UDP Sweep

**Main goal:** Measure TCP/UDP iperf3 throughput and stability  
**Tools:** Run iperf3 client (-J) and, for loopback, iperf3 -s -1

Reference results measured by the maintainer on the system shown in each section (generator TEMPLATE_00_143 · recorded 2026-11-16). Your own runs write `results/RESULTS_ACTUAL.md` in the same format.

> Smoke runs use deliberately small sizes. They check that the workload installs and runs end to end; their numbers are not performance results. Baseline and extended are.

<!-- profile:smoke -->
## smoke

- **System:** 1× NVIDIA H100 NVL (95830 MiB) · Intel(R) Xeon(R) Platinum 8452Y · Ubuntu 24.04.5 LTS · kernel 6.8.0-138-generic · driver 595.91.07
- **Run:** 2026-11-16T19:16:40Z · status **PASS** (exit 0)
- **Time (mm:ss):** setup 00:51 · benchmark 00:06 · whole run 01:03
- **Source:** run 208_20261116_191640
- **Command:** `bash run_benchmark.sh --smoke --protocol tcp,udp --port 5201 --reverse-mode false --window-size 256K --buffer-length 128K --parallel-streams 1 --bandwidth-limit 0 --omit-initial-seconds 0 --time 2`

| # | Metric | Result |
|---|---|---|
| 1 | TCP loopback throughput (tcp_loopback_gbps) | 31.786372607704767 |
| 2 | UDP loopback throughput (udp_throughput_gbps) | 34.88250006890533 |
| 3 | UDP jitter (udp_jitter_ms) | 0.0016291032009896342 |
| 4 | Packet loss, percent (packet_loss_rate) | 0.05398110661268556 |
| 5 | TCP retransmit count per run (tcp_retransmit_count) | 0.0 |
<!-- /profile:smoke -->
