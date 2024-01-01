# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero CPU Miner.\
As testing shows, it works 4-5 times faster for AMD Ryzen processors and 2-4 times faster for Intel processors than the official miner.

Available for Linux, Windows and HiveOS.

If you have problems with the miner, message me in Discord.

Developer fee: 10%

## Usage ##

```
deroluna-miner -d <daemon-address:port> -w <wallet_address> [-t <threads>]
```

#### Example (Linux)
```
./deroluna-miner -d minernode1.dero.io:10100 -w dero1qykyta6ntpd27nl0yq4xtzaf4ls6p5e9pqu0k2x4x3pqq5xavjsdxqgny8270
```
#### Example (Windows)
```
deroluna-miner.exe -d minernode1.dero.io:10100 -w dero1qykyta6ntpd27nl0yq4xtzaf4ls6p5e9pqu0k2x4x3pqq5xavjsdxqgny8270
```

### Options ###
```
    --help -h
        Shows help
    --version
        Shows the version

    --daemon-address -d
        The daemon address
    --wallet -w
        Your wallet address
    --threads -t
        Number of threads
    --no-lock
        Disables CPU core binding
    --period <number>
        The period in seconds for which the average hashrate is calculated
        Must be between 1 and 64
        The default value is 10
    --never-stop
        Simulate mining when connection is lost

    --old-console
        Changes the way information is output to the console
    --no-colors
        Removes colors from the console

    --debug-shares
        Shows found shares (the JSON message and the hash)
    --debug-getwork
        Shows getwork (the JSON message)

    --algo1 0
        Disables optimisations from Beta 1.11.1
    --algo2 0
        Disables optimisations from Beta 1.11.2a
```

## Quick installation ##
#### Linux ####
```
curl -Lo deroluna-miner-linux-amd64.tar.gz https://github.com/DeroLuna/dero-miner/releases/latest/download/deroluna-miner-linux-amd64.tar.gz
tar -xf deroluna-miner-linux-amd64.tar.gz
```

## Benchmarks (preliminarily) ##

The maximum observed hashrate

<details>
  <summary>AMD</summary>

```
AMD Ryzen 3 1200       5.2 kh/s
AMD Ryzen 3 2200G      5.6 kh/s
AMD Ryzen 3 4100       7.9 kh/s
AMD Ryzen 3 5300U      7.7 kh/s

AMD Ryzen 5 1400       6.6 kh/s
AMD Ryzen 5 1500X      8.2 kh/s
AMD Ryzen 5 1600      12.2 kh/s
AMD Ryzen 5 2600      13.4 kh/s
AMD Ryzen 5 2600X     13.3 kh/s
AMD Ryzen 5 3400G      8.2 kh/s
AMD Ryzen 5 3500X     10.5 kh/s
AMD Ryzen 5 3600      15.9 kh/s
AMD Ryzen 5 3600X     15.0 kh/s
AMD Ryzen 5 3600XT    14.5 kh/s
AMD Ryzen 5 4500      14.5 kh/s
AMD Ryzen 5 4600G     15.6 kh/s
AMD Ryzen 5 5500      16.7 kh/s
AMD Ryzen 5 5600      17.7 kh/s
AMD Ryzen 5 5600G     15.4 kh/s
AMD Ryzen 5 5600H     13.1 kh/s
AMD Ryzen 5 5600X     18.7 kh/s
AMD Ryzen 5 7600      20.6 kh/s

AMD Ryzen 7 1700      15.2 kh/s
AMD Ryzen 7 2700      16.1 kh/s
AMD Ryzen 7 2700X     18.7 kh/s
AMD Ryzen 7 3700X     20.9 kh/s
AMD Ryzen 7 3800X     20.9 kh/s
AMD Ryzen 7 3800XT    17.7 kh/s
AMD Ryzen 7 4700U      8.0 kh/s
AMD Ryzen 7 4800U     11.2 kh/s
AMD Ryzen 7 5700G     21.7 kh/s
AMD Ryzen 7 5700U     11.9 kh/s
AMD Ryzen 7 5700X     25.1 kh/s
AMD Ryzen 7 5800H     16.6 kh/s
AMD Ryzen 7 5800X     25.3 kh/s
AMD Ryzen 7 6800H     18.4 kh/s
AMD Ryzen 7 7730U     10.7 kh/s
AMD Ryzen 7 7735HS    18.8 kh/s
AMD Ryzen 7 7800X3D   23.8 kh/s

AMD Ryzen 9 3900      30.9 kh/s
AMD Ryzen 9 3900X     32.6 kh/s
AMD Ryzen 9 3900XT    29.1 kh/s
AMD Ryzen 9 3950X     40.4 kh/s
AMD Ryzen 9 5900HX    10.0 kh/s
AMD Ryzen 9 5900X     35.6 kh/s
AMD Ryzen 9 5950X     47.6 kh/s
AMD Ryzen 9 6900HX    19.7 kh/s
AMD Ryzen 9 7900      38.5 kh/s
AMD Ryzen 9 7900X     42.6 kh/s
AMD Ryzen 9 7900X3D   38.9 kh/s
AMD Ryzen 9 7950X     53.8 kh/s
AMD Ryzen 9 7950X3D   52.7 kh/s

AMD Ryzen Threadripper 3970X   73.4 kh/s
AMD Ryzen Threadripper 3990X   145.2 kh/s

AMD EPYC 7532   130.2 kh/s
AMD EPYC 7551    90.8 kh/s
AMD EPYC 7642   169.8 kh/s
AMD EPYC 7B12   220.3 kh/s
AMD EPYC 7H12   200.6 kh/s
```
</details>

<details>
  <summary>Intel</summary>

```
Intel Core i3-7100       2.0 kh/s
Intel Core i3-8100       3.3 kh/s
Intel Core i3-8100T      2.7 kh/s
Intel Core i3-9100       3.5 kh/s
Intel Core i3-9100F      3.7 kh/s
Intel Core i3-10100      4.3 kh/s
Intel Core i3-10100F     4.2 kh/s
Intel Core i3-10105      4.5 kh/s
Intel Core i3-1115G4     3.9 kh/s

Intel Core i5-2400       2.0 kh/s
Intel Core i5-2500K      2.1 kh/s
Intel Core i5-3570       2.4 kh/s
Intel Core i5-4440S      2.5 kh/s
Intel Core i5-4460       2.6 kh/s
Intel Core i5-4570       2.8 kh/s
Intel Core i5-4590T      2.2 kh/s
Intel Core i5-4670       2.7 kh/s
Intel Core i5-4670K      2.5 kh/s
Intel Core i5-4690K      3.1 kh/s
Intel Core i5-6500       2.9 kh/s
Intel Core i5-6600       3.1 kh/s
Intel Core i5-6600K      3.2 kh/s
Intel Core i5-7400       2.9 kh/s
Intel Core i5-7600K      3.7 kh/s
Intel Core i5-8500       5.2 kh/s
Intel Core i5-8500T      4.1 kh/s
Intel Core i5-8600       4.2 kh/s
Intel Core i5-8600K      4.9 kh/s
Intel Core i5-9400F      5.3 kh/s
Intel Core i5-9500       5.6 kh/s
Intel Core i5-10210U     2.5 kh/s
Intel Core i5-10300H     4.1 kh/s
Intel Core i5-10400      6.2 kh/s
Intel Core i5-10400F     6.0 kh/s
Intel Core i5-10500      6.3 kh/s
Intel Core i5-1135G7     6.1 kh/s
Intel Core i5-11400     12.9 kh/s
Intel Core i5-11400F    12.6 kh/s
Intel Core i5-11400H     9.7 kh/s
Intel Core i5-11600K    11.3 kh/s
Intel Core i5-12400F    13.7 kh/s
Intel Core i5-12500     12.8 kh/s
Intel Core i5-13400     18.5 kh/s

Intel Core i7-2600       2.8 kh/s
Intel Core i7-3770       3.1 kh/s
Intel Core i7-3770K      3.6 kh/s
Intel Core i7-4770K      3.8 kh/s
Intel Core i7-4790       3.7 kh/s
Intel Core i7-5820K      5.0 kh/s
Intel Core i7-6700       3.8 kh/s
Intel Core i7-6700HQ     3.1 kh/s
Intel Core i7-6700K      3.7 kh/s
Intel Core i7-6850K      5.4 kh/s
Intel Core i7-7700       4.1 kh/s
Intel Core i7-7700K      4.7 kh/s
Intel Core i7-8550U      2.2 kh/s
Intel Core i7-8700       5.2 kh/s
Intel Core i7-8700K      6.8 kh/s
Intel Core i7-8750H      4.2 kh/s
Intel Core i7-9700       6.3 kh/s
Intel Core i7-9750H      4.3 kh/s
Intel Core i7-1065G7     4.5 kh/s
Intel Core i7-10700      9.5 kh/s
Intel Core i7-10700F     7.6 kh/s
Intel Core i7-10700K     9.5 kh/s
Intel Core i7-10700KF    8.0 kh/s
Intel Core i7-11700     10.9 kh/s
Intel Core i7-11700F    14.2 kh/s
Intel Core i7-11800H    10.1 kh/s
Intel Core i7-12650H     8.5 kh/s
Intel Core i7-12700     19.2 kh/s
Intel Core i7-12700H    15.7 kh/s
Intel Core i7-13700F    12.1 kh/s

Intel Core i9-7940X     11.1 kh/s
Intel Core i9-9900K      9.9 kh/s
Intel Core i9-9900KF     7.0 kh/s
Intel Core i9-10850K    12.6 kh/s
Intel Core i9-10980XE   19.7 kh/s
Intel Core i9-11900KF   15.8 kh/s
Intel Core i9-14900KF   45.3 kh/s

Intel Xeon E5-2690      10.5 kh/s
Intel Xeon E5-2650 v2   10.0 kh/s
Intel Xeon E5-2660 v2   10.5 kh/s

Intel Xeon E5-2630 v3   10.8 kh/s
Intel Xeon E5-2666 v3   14.2 kh/s
Intel Xeon E5-2670 v3   15.6 kh/s
Intel Xeon E5-2680 v3   19.4 kh/s
Intel Xeon E5-2698 v3   22.1 kh/s
Intel Xeon E5-2699 v3   25.6 kh/s

Intel Xeon E5-2650 v4   15.2 kh/s
Intel Xeon E5-2680 v4   20.9 kh/s
Intel Xeon E5-2686 v4   24.5 kh/s

Intel Xeon Platinum 8124M    32.3 kh/s
Intel Xeon Platinum 8259CL   39.4 kh/s
Intel Xeon Platinum 8369B    81.8 kh/s
```
</details>

## Known issues
* May crash on Linux when resolving the daemon address with the "Assertion failed" exception. In this case, just run the program again.
