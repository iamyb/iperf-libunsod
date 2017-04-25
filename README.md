# iperf-libunsod
iperf integrated with libunsod. Around 50 LOC modified in iperf source code!

### Perfromance
Test result with iperf-libunsod for one TCP connection 

	[  3] local 192.168.56.12 port 11111 connected to 192.168.56.12 port 11111
	[ ID] Interval           Transfer     Bandwidth
	[  3]   0.00-1.00   sec  30.3 MBytes   254 Mbits/sec
	[  3]   1.00-2.00   sec  36.2 MBytes   303 Mbits/sec
	[  3]   2.00-3.00   sec  29.1 MBytes   244 Mbits/sec
	[  3]   3.00-4.00   sec  28.4 MBytes   238 Mbits/sec
	[  3]   4.00-5.00   sec  28.9 MBytes   243 Mbits/sec
	[  3]   5.00-6.00   sec  28.8 MBytes   242 Mbits/sec
	[  3]   6.00-7.00   sec  31.2 MBytes   262 Mbits/sec
	[  3]   7.00-8.00   sec  30.7 MBytes   258 Mbits/sec
	[  3]   8.00-9.00   sec  31.6 MBytes   265 Mbits/sec
	[  3]   9.00-10.00  sec  31.2 MBytes   262 Mbits/sec
	[  3]  10.00-10.18  sec  4.92 MBytes   236 Mbits/sec
	- - - - - - - - - - - - - - - - - - - - - - - - -
	[ ID] Interval           Transfer     Bandwidth
	[  3]   0.00-10.18  sec  0.00 Bytes  0.00 bits/sec                  sender
	[  3]   0.00-10.18  sec   311 MBytes   257 Mbits/sec                  receiver
	-----------------------------------------------------------

Test result with iperf official for one TCP connection
 
	Accepted connection from 192.168.56.101, port 51184
	[  5] local 192.168.56.11 port 11111 connected to 192.168.56.101 port 51185
	[ ID] Interval           Transfer     Bandwidth
	[  5]   0.00-1.00   sec  32.4 MBytes   272 Mbits/sec
	[  5]   1.00-2.01   sec  8.95 MBytes  74.7 Mbits/sec
	[  5]   2.01-3.00   sec  20.1 MBytes   170 Mbits/sec
	[  5]   3.00-4.00   sec  15.2 MBytes   128 Mbits/sec
	[  5]   4.00-5.00   sec  8.19 MBytes  68.8 Mbits/sec
	[  5]   5.00-6.00   sec  7.23 MBytes  60.6 Mbits/sec
	[  5]   6.00-7.00   sec  11.4 MBytes  95.4 Mbits/sec
	[  5]   7.00-8.00   sec  8.88 MBytes  74.5 Mbits/sec
	[  5]   8.00-9.00   sec  6.26 MBytes  52.5 Mbits/sec
	[  5]   9.00-10.00  sec  9.99 MBytes  83.8 Mbits/sec
	[  5]  10.00-10.20  sec  62.7 KBytes  2.65 Mbits/sec
	- - - - - - - - - - - - - - - - - - - - - - - - -
	[ ID] Interval           Transfer     Bandwidth
	[  5]   0.00-10.20  sec  0.00 Bytes  0.00 bits/sec                  sender
	[  5]   0.00-10.20  sec   129 MBytes   106 Mbits/sec                  receiver

NOTE: The two test were executed on a same VM with Intel i5-4300 hosted.

