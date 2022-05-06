Context:
The goal of this project was to determine the ideal network for a LAN for a community with no access to the internet.

# Best Wifi standard

The first part of my experiments was determining the best the differences between the various WiFi standards

### 5GHz vs 2.4GHz
5GHz has a higher data rate but shorter range, while 2.4GHz has a lower data rate but higher range. For this reason 2.4GHz is more useful for us.

### Wifi Standards
There are various wifi standards/protocols the ones of interest to us were 802.11n, 802.11b

Using iperf we were able to see the differences in throughput

* 802.11n on 2.4GHz
[  5] local 192.168.1.148 port 50740 connected to 192.168.1.143 port 5201
[ ID] Interval           Transfer     Bitrate
[  5]   0.00-1.00   sec  18.8 MBytes   158 Mbits/sec
[  5]   1.00-2.00   sec  18.9 MBytes   159 Mbits/sec
[  5]   2.00-3.00   sec  17.3 MBytes   145 Mbits/sec
[  5]   3.00-4.00   sec  16.2 MBytes   136 Mbits/sec
[  5]   4.00-5.00   sec  19.0 MBytes   159 Mbits/sec
[  5]   5.00-6.00   sec  16.8 MBytes   140 Mbits/sec
[  5]   6.00-7.00   sec  16.8 MBytes   142 Mbits/sec
[  5]   7.00-8.00   sec  17.5 MBytes   147 Mbits/sec
[  5]   8.00-9.00   sec  18.6 MBytes   156 Mbits/sec
[  5]   9.00-10.00  sec  16.7 MBytes   140 Mbits/sec
- - - - - - - - - - - - - - - - - - - - - - - - -

[ ID] Interval           Transfer     Bitrate
[  5]   0.00-10.00  sec   177 MBytes   148 Mbits/sec                  sender
[  5]   0.00-10.05  sec   176 MBytes   147 Mbits/sec                  receiver

* 802.11b on 2.4GHz
* [  5] local 192.168.1.148 port 51008 connected to 192.168.1.143 port 5201
[ ID] Interval           Transfer     Bitrate
[  5]   0.00-1.00   sec   405 KBytes  3.31 Mbits/sec
[  5]   1.00-2.00   sec   406 KBytes  3.33 Mbits/sec
[  5]   2.00-3.00   sec  1.58 MBytes  13.2 Mbits/sec
[  5]   3.00-4.00   sec   134 KBytes  1.10 Mbits/sec
[  5]   4.00-5.00   sec  0.00 Bytes  0.00 bits/sec
[  5]   5.00-6.00   sec  1.14 MBytes  9.53 Mbits/sec
[  5]   6.00-7.00   sec   632 KBytes  5.18 Mbits/sec
[  5]   7.00-8.00   sec   628 KBytes  5.15 Mbits/sec
[  5]   8.00-9.00   sec   370 KBytes  3.03 Mbits/sec
[  5]   9.00-10.00  sec  0.00 Bytes  0.00 bits/sec
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bitrate
[  5]   0.00-10.00  sec  5.23 MBytes  4.39 Mbits/sec                  sender
[  5]   0.00-11.11  sec  5.23 MBytes  3.95 Mbits/sec

## Metrics

Using Netdata we were able to find the limits of the setup outlined here:

https://docs.google.com/presentation/d/1OGvD1Tdpx4ogBjKujY9GRqIwQSofuNaK9f86NpKi8v0/edit?usp=sharing
