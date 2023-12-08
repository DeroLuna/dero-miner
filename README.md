# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero CPU Miner.

Сurrently available only on Linux and Windows.

If you have problems with the miner, message me in Discord.

Developer fee: 10%

## Quick installation ##
### Linux ###
```
curl -Lo deroluna-miner-linux-amd64.tar.gz https://github.com/DeroLuna/dero-miner/releases/latest/download/deroluna-miner-linux-amd64.tar.gz
tar -xf deroluna-miner-linux-amd64.tar.gz
```

## Usage ##

```
./deroluna-miner -d <daemon-address:port> -w <wallet_address> [-t <threads>]
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

## Known issues
* May crash when starting with the "Assertion failed" exception. In this case, just run the program again.
