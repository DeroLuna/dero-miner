# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero Miner.
Сurrently available only on Linux.
Use it for testing purposes only. There are no guarantees that it will work stably.

Developer fee: 10%

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
