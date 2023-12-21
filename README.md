# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero CPU Miner.\
As testing shows, it works 4-5 times faster for AMD Ryzen processors and 2-4 times faster for Intel processors than the official miner.

Сurrently available only on Linux and Windows.

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

## Known issues
* May crash when starting with the "Assertion failed" exception. In this case, just run the program again.
