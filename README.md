# Awesome Engineering Toolbox [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of awesome software development frameworks, libraries, software and resources.

---

## Software Product Development Guidelines

* [How do I choose an open source LICENSE?](https://choosealicense.com/)
* [How do I make a good VERSION?](https://semver.org/spec/v2.0.0.html)
* [How do I make a good CHANGELOG?](https://keepachangelog.com/en/1.1.0/)
* [Debugging with VSCode](https://code.visualstudio.com/docs/editor/debugging)
* [Flight Rules for Git](https://github.com/k88hudson/git-flight-rules)

## Awesome Study Materials For Being A Better Engineer

* [The Missing Semester of Your CS Education](https://missing-semester-cn.github.io/)
* [High Performance Browser Networking](https://hpbn.co/)
* [The Linux kernel Source Code Online Reading](https://elixir.bootlin.com/linux/v5.2-rc7/source)
* [The Linux kernel Diagram Online Reading](https://makelinux.github.io/kernel/)
* [CNCF Cloud Native Interactive Landscape](https://landscape.cncf.io/)

## Http/Https/gRPC Dev&Ops

*Tools for Http/Https/gRPC Dev&Ops.*

* [HTTP/HTTPS request tool, httpstat](https://github.com/davecheney/httpstat)

httpstat is like curl -v, with colours.

* [HTTP/HTTPS inspection tool, wuzz](https://github.com/asciimoo/wuzz)

Interactive cli tool for HTTP inspection.

* [HTTP/HTTPS inspection tool, httping](https://www.vanheusden.com/httping/)

httping is like 'ping' but for http-requests.

* [HTTP/HTTPS load testing tool, vegeta](https://github.com/tsenart/vegeta)

vegeta is a versatile HTTP load testing tool built out of a need to drill HTTP services with a constant request 
rate.
* [HTTP/HTTPS load testing tool, hey](https://github.com/rakyll/hey)

hey is the ApacheBench (ab) replacement.

* [HTTP/HTTPS load testing tool, wrk](https://github.com/wg/wrk)

wrk is a modern HTTP benchmarking tool capable of generating significant load when run on a single multi-core CPU. 
It combines a multithreaded design with scalable event notification systems such as epoll and kqueue.
* [HTTP/HTTPS testing framework, httprunner](https://github.com/httprunner/httprunner)

httprunner is an open-source API/UI testing tool that is simple to use, powerful, and has a rich plugin mechanism 
and high scalability.
* [HTTP/HTTPS traffic replay tool, goreplay](https://github.com/buger/goreplay)

goreplay is an open-source tool for capturing and replaying live HTTP traffic into a test environment in order to 
continuously test your system with real data.
* [TCP traffic replay tool, tcpreplay](https://github.com/appneta/tcpreplay)

tcpreplay is a suite of utilities for UNIX (and Win32 under Cygwin) operating systems for editing and replaying network traffic which was previously captured by tools like tcpdump and Wireshark.
* [gRPC request tool, grpcurl](https://github.com/fullstorydev/grpcurl)

grpcurl is like 'curl' but for gRPC.

* [gRPC load testing tool, ghz](https://github.com/bojand/ghz)

ghz is a modern gRPC benchmarking and load testing tool.

* [gRPC debugging and development tool suite, grpc-tools](https://github.com/bradleyjkemp/grpc-tools)

A suite of gRPC debugging tools. Like Fiddler/Charles but for gRPC.

* [Web App Stress Test](https://pagespeed.web.dev/)

## TCP/IP Network Dev&Ops

*Tools for TCP/IP Network Dev&Ops.*

* [IP inspection tool, gping](https://github.com/orf/gping)

Ping, but with a graph.

* [Simulating non-ideal network environments, tc](https://man7.org/linux/man-pages/man8/tc-netem.8.html)

The netem queue discipline provides Network Emulation functionality for testing protocols by emulating the properties of real-world networks. The queue discipline provides one or more network impairments to packets such as: delay, loss, duplication, and packet corruption.

* [TCP/UDP network infrastructure tool, netstat](https://linux.die.net/man/8/netstat)

The netstat tool does print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.

Most Common Commands:
```
sudo netstat -alnpt | grep ':$PORT'
```

* [TCP/UDP network infrastructure tool, ss](https://linux.die.net/man/8/netstat)

Another utility to investigate sockets, like netstat, but display more TCP and state informations.

Most Common Commands:
```
sudo ss -anpt | grep ':$PORT'
```

* [TCP/UDP network infrastructure tool, nmap](https://nmap.org/)

The nmap tool does for network discovery and security auditing.

Most Common Commands:
```
sudo nmap -sT -O $TARGET_IP
```

* [TCP/UDP traffic monitoring tool, it groups bandwidth by process, nethogs](https://github.com/raboof/nethogs)

The nethogs tool does for network usage what top does for CPU usage. Instead of breaking the traffic down per protocol or per subnet, like most tools do, it groups bandwidth by process.

* [TCP/UDP traffic monitoring tool, it groups bandwidth by interface, iftop](http://www.ex-parrot.com/pdw/iftop)

The iftop tool does for network usage what top does for CPU usage. It listens to network traffic on a named interface and displays a table of current bandwidth usage by pairs of hosts.

* [TCP/UDP network throughput benchmark tool, ntttcp](https://github.com/microsoft/ntttcp-for-linux)

The ntttcp tool is a multiple-threaded Linux network throughput benchmark tool.

* [TCP/UDP network bandwidth measurement tool, iperf3](https://github.com/esnet/iperf)

iperf is a tool for active measurements of the maximum achievable bandwidth on IP networks.

* [TCP/UDP comprehensive network measurement tool, ethr](https://github.com/microsoft/ethr)

Ethr provide a native tool for comprehensive network performance measurements of bandwidth, connections/s, packets/s, latency, loss & jitter, across multiple protocols such as TCP, UDP, HTTP, HTTPS, and across multiple platforms such as Windows, Linux and other Unix systems.

* [TCP/UDP network bandwidth measurement tool, iperf3](https://github.com/esnet/iperf)

iperf is a tool for active measurements of the maximum achievable bandwidth on IP networks.

## C/C++ Dev&Ops

*Tools&Libraries& for C/C++ Dev&Ops.*

* [gperftools heapprofile by google](https://gperftools.github.io/gperftools/heapprofile.html)
* [gperftools heap-checker by google](https://gperftools.github.io/gperftools/heap_checker.html)
* [gperftools cpuprofile by google](https://gperftools.github.io/gperftools/cpuprofile.html)
* [memory profile tool, valgrind](http://valgrind.org/)

Valgrind is an instrumentation framework for building dynamic analysis tools. There are Valgrind tools that can automatically detect many memory management and threading bugs, and profile your programs in detail.

### Awesome C/C++ Study Materials

* [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines)
* [A curated list of awesome C++ (or C) resources](https://github.com/fffaraz/awesome-cpp)
* [A curated list of awesome C++ (or C) resources, but more modern](https://github.com/rigtorp/awesome-modern-cpp)
* [Modern C++ Tutorial: C++11/14/17/20 On the Fly](https://github.com/changkun/modern-cpp-tutorial)
* [A template for modern C++ projects using CMake/Clang-Format/UT/CI, and more](https://github.com/filipdutescu/modern-cpp-template)
* [Useful CMake Examples](https://github.com/ttroy50/cmake-examples)
* [C++ Syntax, Data Structures, and Algorithms Cheat Sheet](https://github.com/gibsjose/cpp-cheat-sheet)

## Python Dev&Ops

*Tools&Libraries& for Python Dev&Ops.*

* [A high-performance, high-precision CPU, GPU, and memory profiler for Python with AI-powered optimization proposals, scalene](https://github.com/plasma-umass/scalene)
* [Create Call Graphs for Python Programs, pycallgraph](https://github.com/gak/pycallgraph)
* [Matplotlib Cheat Sheet](https://github.com/matplotlib/cheatsheets)

## Linux Platforms Dev&Ops

* [a top/htop alternative for GNU/Linux, glances](https://github.com/nicolargo/glances)
* [Monitor a process and trigger a notification, noti](https://github.com/variadico/noti)
* [Flexible i/o tester, fio](https://github.com/axboe/fio)
* [Linux performance analysis tools, perf and more beyond](http://www.brendangregg.com/perf.html)
* [Manage procfile-based applications, foreman](https://github.com/ddollar/foreman)
* [A terminal client for MySQL with auto-completion and syntax-highlighting, mycli](https://github.com/dbcli/mycli)
* [A terminal client for Redis with auto-completion and syntax-highlighting, iredis](https://github.com/laixintao/iredis)
* [Tool to bootstrap CAs, certificate requests, and signed certificates, certstrap](https://github.com/square/certstrap)
* [Tool to give warnings and suggestions for bash/sh shell scripts, shellcheck](https://www.shellcheck.net/)
