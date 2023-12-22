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

Average hashrate reported by miners.\
May vary depending on your system and CPU frequency.

```
AMD Ryzen 5 3400G    7.5 kh/s
AMD Ryzen 5 1600    11.6 kh/s
AMD Ryzen 5 3600    13.8 kh/s
AMD Ryzen 7 3700X   15.4 kh/s
AMD Ryzen 7 5700X   16.6 kh/s
AMD Ryzen 7 5700G   19.8 kh/s
AMD Ryzen 9 3900X   27.5 kh/s
AMD Ryzen 9 3900    28.5 kh/s
AMD Ryzen 9 5900X   31.0 kh/s
AMD Ryzen 9 5950X   40.4 kh/s
AMD Ryzen 9 7900X   41.8 kh/s
AMD Ryzen 9 7950X   48.3 kh/s
```

## Known issues
* May crash on Linux when resolving the daemon address with the "Assertion failed" exception. In this case, just run the program again.
