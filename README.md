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
```

## Quick installation ##
#### Linux ####
```
curl -Lo deroluna-miner-linux-amd64.tar.gz https://github.com/DeroLuna/dero-miner/releases/latest/download/deroluna-miner-linux-amd64.tar.gz
tar -xf deroluna-miner-linux-amd64.tar.gz
```

## Benchmarks (preliminarily) ##

The maximum observed hashrate

```
AMD Ryzen 3 2200G      5.6 kh/s
AMD Ryzen 5 1600      11.8 kh/s
AMD Ryzen 5 2600      12.9 kh/s
AMD Ryzen 5 3400G      8.2 kh/s
AMD Ryzen 5 3500X      8.6 kh/s
AMD Ryzen 5 3600      15.6 kh/s
AMD Ryzen 5 4600G     15.3 kh/s
AMD Ryzen 5 5500      16.3 kh/s
AMD Ryzen 5 5600      16.3 kh/s
AMD Ryzen 5 5600G     15.5 kh/s
AMD Ryzen 5 5600X     13.9 kh/s
AMD Ryzen 5 7600      20.0 kh/s
AMD Ryzen 7 1700      14.6 kh/s
AMD Ryzen 7 1800X     10.4 kh/s
AMD Ryzen 7 2700      15.6 kh/s
AMD Ryzen 7 3700X     18.3 kh/s
AMD Ryzen 7 3800X     20.0 kh/s
AMD Ryzen 7 4700U      8.0 kh/s
AMD Ryzen 7 4800U     11.3 kh/s
AMD Ryzen 7 5700G     21.1 kh/s
AMD Ryzen 7 5700U     12.0 kh/s
AMD Ryzen 7 5700X     22.5 kh/s
AMD Ryzen 7 5800X     23.4 kh/s
AMD Ryzen 7 6800H     12.8 kh/s
AMD Ryzen 9 3900      30.2 kh/s
AMD Ryzen 9 3900X     30.0 kh/s
AMD Ryzen 9 3900XT    28.4 kh/s
AMD Ryzen 9 3950X     37.3 kh/s
AMD Ryzen 9 5900X     34.4 kh/s
AMD Ryzen 9 5950X     43.8 kh/s
AMD Ryzen 9 7900      37.5 kh/s
AMD Ryzen 9 7900X     43.8 kh/s
AMD Ryzen 9 7950X     51.9 kh/s
AMD Ryzen 9 7950X3D   48.3 kh/s
```

## Known issues
* May crash on Linux when resolving the daemon address with the "Assertion failed" exception. In this case, just run the program again.
