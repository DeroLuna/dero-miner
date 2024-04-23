# AstroBWTv3 Dero Miner by DeroLuna

A new optimized AstroBWTv3 Dero CPU Miner.\
As testing shows, it works 4-5 times faster for AMD Ryzen and 2-4 times faster for Intel Core than the official miner.

Available for Linux, Windows and HiveOS.

If you have problems with the miner, message me in Discord.\
Discord server: https://discord.gg/vuJW8UahRV

Developer fee: 5%

## Usage ##

```
deroluna-miner -d <daemon-address:port> -w <wallet_address> [-t <threads>]
```

#### Example
```
deroluna-miner -d minernode1.dero.io:10100 -w dero1qykyta6ntpd27nl0yq4xtzaf4ls6p5e9pqu0k2x4x3pqq5xavjsdxqgny8270
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
    --period <time in seconds>
        The period for which the average hashrate is calculated (10 by default)
        Must be between 1 and 64
    --log-console-line <time in seconds>
        Enables logging of the console line with the specified period
    --show-pool-shares
        Shows the total count of shares sent to the pool
    --never-stop
        Simulate mining when connection is lost

    --exit-on-zero-hashrate
        Stops the miner if the hashrate has been zero for 15 seconds
        You should run the command in a loop for the miner to restart (except for HiveOS)
          See the examples in start.sh and start.bat

    --old-console
        Changes the way text is output to the console
    --no-colors
        Removes colors from the console
    --no-cr
        Replaces the carriage return (\r) with a new line (\n) in the console

    --debug-shares
        Shows info about found shares (the JSON message and the hash)
    --debug-getwork
        Shows info about getwork (the JSON message)

    --algo2 0
        Disables optimisations from Beta 1.11.2a
```

## Hashrate stats ##

#### The maximum average observed hashrate

<details>
  <summary>AMD</summary>

```
AMD Athlon 3000G        4.3 kh/s

AMD Ryzen 3 1200        5.5 kh/s
AMD Ryzen 3 3200G       6.1 kh/s
AMD Ryzen 3 3300X       9.9 kh/s
AMD Ryzen 3 4100        8.7 kh/s
AMD Ryzen 3 4300G       9.8 kh/s
AMD Ryzen 3 4300GE      7.8 kh/s

AMD Ryzen 5 1400        7.6 kh/s
AMD Ryzen 5 1500X       8.7 kh/s
AMD Ryzen 5 1600       13.1 kh/s
AMD Ryzen 5 2400G       7.8 kh/s
AMD Ryzen 5 2600       13.7 kh/s
AMD Ryzen 5 2600X      14.4 kh/s
AMD Ryzen 5 PRO 3400GE  7.3 kh/s
AMD Ryzen 5 3400G       8.6 kh/s
AMD Ryzen 5 3500X      10.5 kh/s
AMD Ryzen 5 3550H       5.5 kh/s
AMD Ryzen 5 3600       16.4 kh/s
AMD Ryzen 5 3600X      16.6 kh/s
AMD Ryzen 5 3600XT     15.6 kh/s
AMD Ryzen 5 4500       15.2 kh/s
AMD Ryzen 5 4600G      15.9 kh/s
AMD Ryzen 5 4600H      11.3 kh/s
AMD Ryzen 5 PRO 4650GE 13.5 kh/s
AMD Ryzen 5 PRO 4650G  14.6 kh/s
AMD Ryzen 5 5500       18.0 kh/s
AMD Ryzen 5 5600       18.5 kh/s
AMD Ryzen 5 5600G      18.1 kh/s
AMD Ryzen 5 5600H      15.4 kh/s
AMD Ryzen 5 5600X      19.0 kh/s
AMD Ryzen 5 7500F      22.7 kh/s
AMD Ryzen 5 7600       21.0 kh/s
AMD Ryzen 5 7600X      21.3 kh/s

AMD Ryzen 7 1700       17.1 kh/s
AMD Ryzen 7 1700X      16.4 kh/s
AMD Ryzen 7 1800X      17.0 kh/s
AMD Ryzen 7 2700       16.9 kh/s
AMD Ryzen 7 2700X      19.1 kh/s
AMD Ryzen 7 PRO 3700   19.8 kh/s
AMD Ryzen 7 3700X      21.7 kh/s
AMD Ryzen 7 3800X      21.7 kh/s
AMD Ryzen 7 4800H      15.9 kh/s
AMD Ryzen 7 5700G      25.4 kh/s
AMD Ryzen 7 5700X      25.5 kh/s
AMD Ryzen 7 5800H      17.0 kh/s
AMD Ryzen 7 5800X      25.3 kh/s
AMD Ryzen 7 5800X3D    23.9 kh/s
AMD Ryzen 7 6800H      18.4 kh/s
AMD Ryzen 7 7700       28.4 kh/s
AMD Ryzen 7 7700X      29.2 kh/s
AMD Ryzen 7 7735HS     19.5 kh/s

AMD Ryzen 9 3900       32.2 kh/s
AMD Ryzen 9 3900X      33.1 kh/s
AMD Ryzen 9 3900XT     31.3 kh/s
AMD Ryzen 9 3950X      43.8 kh/s
AMD Ryzen 9 5900HX     20.1 kh/s
AMD Ryzen 9 5900X      38.1 kh/s
AMD Ryzen 9 5950X      48.6 kh/s
AMD Ryzen 9 6900HX     19.7 kh/s
AMD Ryzen 9 7900       43.4 kh/s
AMD Ryzen 9 7900X      44.6 kh/s
AMD Ryzen 9 7900X3D    39.6 kh/s
AMD Ryzen 9 7940HS     20.9 kh/s
AMD Ryzen 9 PRO 7945   35.7 kh/s
AMD Ryzen 9 7945HX     50.5 kh/s
AMD Ryzen 9 7950X      57.1 kh/s
AMD Ryzen 9 7950X3D    53.6 kh/s

AMD Ryzen Threadripper 1920X     26.0 kh/s
AMD Ryzen Threadripper 1950X     31.8 kh/s
AMD Ryzen Threadripper 2950X     32.1 kh/s
AMD Ryzen Threadripper 2970WX    39.9 kh/s
AMD Ryzen Threadripper 2990WX    57.3 kh/s
AMD Ryzen Threadripper 3970X     84.8 kh/s
AMD Ryzen Threadripper 3990X    146.7 kh/s
AMD Ryzen Threadripper 7970X     89.8 kh/s

AMD EPYC 7402      49.0 kh/s
AMD EPYC 7402P     51.3 kh/s
AMD EPYC 7451      38.8 kh/s
AMD EPYC 7452      62.1 kh/s
AMD EPYC 7532      65.1 kh/s
AMD EPYC 7542      45.5 kh/s
AMD EPYC 7551      46.8 kh/s
AMD EPYC 7551P     47.0 kh/s
AMD EPYC 7601      48.2 kh/s
AMD EPYC 7642      88.9 kh/s
AMD EPYC 7702     100.3 kh/s
AMD EPYC 7742     108.2 kh/s
AMD EPYC 7B12     116.3 kh/s
AMD EPYC 7B13     104.3 kh/s
AMD EPYC 7D12      50.1 kh/s
AMD EPYC 7H12     104.7 kh/s
AMD EPYC 7J13     115.8 kh/s
AMD EPYC 7V12     111.9 kh/s
AMD EPYC 9254      56.5 kh/s
```
</details>

<details>
  <summary>Intel</summary>

```
Intel Core i3-10100      4.5 kh/s
Intel Core i3-10100F     4.5 kh/s
Intel Core i3-10105      4.6 kh/s
Intel Core i3-10105F     4.5 kh/s

Intel Core i5-7600K      4.0 kh/s
Intel Core i5-8400       5.4 kh/s
Intel Core i5-8500       5.2 kh/s
Intel Core i5-8500T      4.2 kh/s
Intel Core i5-8600       4.4 kh/s
Intel Core i5-8600K      6.7 kh/s
Intel Core i5-9400       5.4 kh/s
Intel Core i5-9400F      5.5 kh/s
Intel Core i5-9500       5.6 kh/s
Intel Core i5-9600K      6.1 kh/s
Intel Core i5-10300H     4.1 kh/s
Intel Core i5-1035G1     4.6 kh/s
Intel Core i5-10400      6.6 kh/s
Intel Core i5-10400F     6.6 kh/s
Intel Core i5-10500      6.6 kh/s
Intel Core i5-10500H     5.3 kh/s
Intel Core i5-10600      6.8 kh/s
Intel Core i5-10600K     7.8 kh/s
Intel Core i5-11300H     7.7 kh/s
Intel Core i5-11400H    11.7 kh/s
Intel Core i5-1145G7     5.1 kh/s
Intel Core i5-12400     13.8 kh/s
Intel Core i5-12400F    14.3 kh/s
Intel Core i5-12450H    11.8 kh/s
Intel Core i5-12500     13.6 kh/s
Intel Core i5-12500T     9.7 kh/s
Intel Core i5-13400     19.1 kh/s
Intel Core i5-13600K    25.9 kh/s

Intel Core i7-4790K      4.4 kh/s
Intel Core i7-4930K      4.4 kh/s
Intel Core i7-6700       4.0 kh/s
Intel Core i7-6700K      4.3 kh/s
Intel Core i7-6950X     10.5 kh/s
Intel Core i7-7700       4.3 kh/s
Intel Core i7-7700K      4.7 kh/s
Intel Core i7-7740X      4.0 kh/s
Intel Core i7-7820X      8.3 kh/s
Intel Core i7-8700       7.1 kh/s
Intel Core i7-8700K      7.8 kh/s
Intel Core i7-8750H      4.6 kh/s
Intel Core i7-9700       8.2 kh/s
Intel Core i7-9700F      5.8 kh/s
Intel Core i7-9700K      7.4 kh/s
Intel Core i7-1065G7     5.0 kh/s
Intel Core i7-10700K    10.2 kh/s
Intel Core i7-10700KF    9.8 kh/s
Intel Core i7-10750H     5.3 kh/s
Intel Core i7-11800H    14.0 kh/s
Intel Core i7-12700     24.5 kh/s
Intel Core i7-12700H    21.6 kh/s
Intel Core i7-12700K    20.1 kh/s
Intel Core i7-13700HX   21.6 kh/s
Intel Core i7-13700K    32.8 kh/s
Intel Core i7-13700KF   34.3 kh/s

Intel Core i9-9900K     10.0 kh/s
Intel Core i9-10850K    13.0 kh/s
Intel Core i9-10900F    11.9 kh/s
Intel Core i9-10900K    13.1 kh/s
Intel Core i9-10980XE   19.7 kh/s
Intel Core i9-11900H    11.9 kh/s
Intel Core i9-12900     26.4 kh/s
Intel Core i9-12900F    31.5 kh/s
Intel Core i9-12900H    23.0 kh/s
Intel Core i9-13900K    48.4 kh/s
Intel Core i9-13900KF   50.2 kh/s
Intel Core i9-14900KF   45.3 kh/s
```
</details>

## Algo switching ##
With the algo switching the miner will switch between Dero and any coin you can mine with xmrig.\
The miner switches to xmrig when the Dero difficulty is high and switches back when it's low.\
This should be about 30% more profitable in case you mine something as profitable as Dero.

### Linux & Windows

If you use `config.json` for xmrig then find the `"http"` block and change it to this:
```
    "http": {
        "enabled": true,
        "host": "127.0.0.1",
        "port": 37329,
        "access-token": "auth",
        "restricted": false
    },
```

Otherwise, if you use command line options for xmrig then add this to xmrig options:
`--http-port 37329 --http-no-restricted --http-access-token auth`

Run xmrig\
Run deroluna-miner with the additional option `--xmrig`

### HiveOS

Create a Flight Sheet with xmrig and deroluna-miner in it.

Add this line in the `Extra config arguments` for xmrig:
`"http": { "enabled": true, "host": "127.0.0.1", "port": 37329, "access-token": "auth", "restricted": false }`

Add `--xmrig` in the `Extra config arguments` for deroluna-miner

### Notes
**You should mine Dero in solo** (use port 10100) otherwise you will get much less Dero.\
This also means you will need to register your own Dero wallet.

The algorithms are switching about 6 times per minute.

## Known issues
* May crash on Linux when resolving the daemon address with the "Assertion failed" exception. In this case, just run the program again.
* If you have a dual CPU and you are using Windows, then most likely only one of the CPUs will be used. To use the second CPU, run another instance of the miner.
