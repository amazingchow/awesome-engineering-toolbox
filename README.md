<div align="center">

# Awesome Engineering Toolbox [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated collection of awesome tools, frameworks, libraries, and resources for software engineers and developers. This list focuses on practical, production-ready tools that can enhance your development workflow and engineering productivity.

[中文版本](README_ZH.md) • [Contributing](#contributing)

</div>

---

## Contents

- [Development Guidelines](#development-guidelines)
- [Learning Resources](#learning-resources)
- [HTTP/HTTPS/gRPC](#httphttpsgrpc)
- [Network Tools](#network-tools)
- [Language-Specific Tools](#language-specific-tools)
  - [C/C++](#cc)
  - [Go](#go)
  - [Python](#python)
  - [Rust](#rust)
- [Linux System Tools](#linux-system-tools)
- [Database Tools](#database-tools)
- [Container & Orchestration](#container--orchestration)
- [Performance & Profiling](#performance--profiling)
- [Terminal & CLI Enhancements](#terminal--cli-enhancements)
- [Security & Penetration Testing](#security--penetration-testing)
- [Productivity Tools](#productivity-tools)
- [Web-Based Tools](#web-based-tools)

---

## Development Guidelines

Essential resources for software development best practices.

- [Choose an Open Source License](https://choosealicense.com/) - A guide to help you choose the right license for your project.
- [Semantic Versioning](https://semver.org/spec/v2.0.0.html) - A simple set of rules for version numbers.
- [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) - Guidelines for maintaining a useful changelog.
- [Flight Rules for Git](https://github.com/k88hudson/git-flight-rules) - A guide for what to do when things go wrong with Git.
- [Debugging with VSCode](https://code.visualstudio.com/docs/editor/debugging) - Official VSCode debugging documentation.

## Learning Resources

High-quality educational materials for becoming a better engineer.

- [The Missing Semester of Your CS Education](https://missing-semester-cn.github.io/) - Master command-line, version control, text editing, and more.
- [High Performance Browser Networking](https://hpbn.co/) - A comprehensive guide to network protocols and performance optimization.
- [The Linux Kernel Source Code](https://elixir.bootlin.com/linux/latest/source) - Browse the Linux kernel source code online.
- [Linux Kernel Diagrams](https://makelinux.github.io/kernel/) - Interactive diagrams of Linux kernel internals.
- [CNCF Cloud Native Interactive Landscape](https://landscape.cncf.io/) - A comprehensive view of the cloud native ecosystem.
- [Performance Ninja Class](https://github.com/dendibakh/perf-ninja) - Learn performance analysis and optimization techniques.
- [Performance Analysis and Tuning on Modern CPU](https://github.com/dendibakh/perf-book) - In-depth guide to CPU performance.
- [Linux Tracing Workshop Materials](https://github.com/goldshtn/linux-tracing-workshop) - Learn Linux tracing and profiling tools.
- [Linux Server Administration](https://github.com/livialima/linuxupskillchallenge) - A month-long challenge to learn Linux administration.

## HTTP/HTTPS/gRPC

Tools for HTTP/HTTPS/gRPC development, testing, and operations.

### Request & Inspection

- [httpstat](https://github.com/davecheney/httpstat) - curl statistics made simple. Like `curl -v` but with colors and better visualization.
- [wuzz](https://github.com/asciimoo/wuzz) - Interactive CLI tool for HTTP inspection and debugging.
- [httping](https://www.vanheusden.com/httping/) - Ping-like tool for HTTP requests. Measure latency and availability.

### Load Testing & Benchmarking

- [vegeta](https://github.com/tsenart/vegeta) - HTTP load testing tool with constant request rate. Excellent for stress testing APIs.
- [hey](https://github.com/rakyll/hey) - Modern HTTP benchmarking tool. A worthy replacement for ApacheBench (ab).
- [wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool capable of generating significant load. Multi-threaded with event notification.
- [Page Speed Insights](https://pagespeed.web.dev/) - Analyze and optimize web application performance.

### Testing & Automation

- [httprunner](https://github.com/httprunner/httprunner) - API/UI testing framework with rich plugins and high scalability.
- [goreplay](https://github.com/buger/goreplay) - Capture and replay live HTTP traffic for continuous testing with real data.

### gRPC Tools

- [grpcurl](https://github.com/fullstorydev/grpcurl) - Command-line tool for interacting with gRPC servers. Like curl for gRPC.
- [ghz](https://github.com/bojand/ghz) - gRPC benchmarking and load testing tool with detailed statistics.
- [grpc-tools](https://github.com/bradleyjkemp/grpc-tools) - Suite of gRPC debugging tools. Like Fiddler/Charles but for gRPC.

### Traffic Replay

- [tcpreplay](https://github.com/appneta/tcpreplay) - Suite of utilities for editing and replaying network traffic captured by tcpdump/Wireshark.

## Network Tools

Comprehensive tools for network development, monitoring, and troubleshooting.

### Network Monitoring & Diagnostics

- [gping](https://github.com/orf/gping) - Ping with a graph. Visualize ping statistics in real-time.
- [tcpprobe](https://github.com/mehrdadrad/tcpprobe) - Modern TCP performance observability tool.
- [nethogs](https://github.com/raboof/nethogs) - Network bandwidth monitoring grouped by process. Like top but for network usage.
- [iftop](http://www.ex-parrot.com/pdw/iftop) - Display bandwidth usage by host pairs on a network interface.

### Network Infrastructure

- [netstat](https://linux.die.net/man/8/netstat) - Print network connections, routing tables, interface statistics, and more.
  ```bash
  sudo netstat -alnpt | grep ':$PORT'
  ```
- [ss](https://man7.org/linux/man-pages/man8/ss.8.html) - Socket statistics tool. Faster than netstat with more TCP information.
  ```bash
  sudo ss -anpt | grep ':$PORT'
  ```
- [nmap](https://nmap.org/) - Network discovery and security auditing tool.
  ```bash
  sudo nmap -sT -O $TARGET_IP
  ```

### Performance Testing & Benchmarking

- [iperf3](https://github.com/esnet/iperf) - Tool for active measurements of maximum achievable bandwidth on IP networks.
- [ntttcp](https://github.com/microsoft/ntttcp-for-linux) - Multi-threaded Linux network throughput benchmark tool.
- [netperf](https://github.com/HewlettPackard/netperf) - Network performance benchmarking for TCP/UDP/SOCKETS protocols.
- [ethr](https://github.com/microsoft/ethr) - Comprehensive network performance measurement tool by Microsoft. Supports TCP, UDP, HTTP, HTTPS.

### Network Emulation

- [tc (netem)](https://man7.org/linux/man-pages/man8/tc-netem.8.html) - Network emulation for testing protocols. Simulate delay, loss, duplication, and corruption.

### Network Proxy

- [anyproxy](http://anyproxy.io/) - HTTP/HTTPS traffic proxy with web interface for debugging.

## Language-Specific Tools

### C/C++

Development tools, libraries, and resources for C/C++ engineering.

#### Development Libraries

- [cpp-httplib](https://github.com/yhirose/cpp-httplib) - Single-header C++ HTTP/HTTPS server and client library.
- [libunwind](http://download.savannah.gnu.org/releases/libunwind/) - Portable and efficient C programming interface for determining the call-chain.

#### Performance & Profiling

- [gperftools](https://github.com/gperftools/gperftools) - High-performance multi-threaded malloc() and performance analysis tools by Google.
  - [Heap Profiler](https://gperftools.github.io/gperftools/heapprofile.html) - Heap memory profiling.
  - [Heap Checker](https://gperftools.github.io/gperftools/heap_checker.html) - Memory leak detection.
  - [CPU Profiler](https://gperftools.github.io/gperftools/cpuprofile.html) - CPU performance profiling.
- [Valgrind](http://valgrind.org/) - Framework for building dynamic analysis tools. Detects memory management and threading bugs.

#### Learning Resources

- [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) - Collaborative effort led by Bjarne Stroustrup.
- [Awesome C++](https://github.com/fffaraz/awesome-cpp) - Curated list of awesome C/C++ frameworks, libraries, and resources.
- [Awesome Modern C++](https://github.com/rigtorp/awesome-modern-cpp) - Collection of resources on modern C++.
- [Modern C++ Tutorial](https://github.com/changkun/modern-cpp-tutorial) - Modern C++ features (C++11/14/17/20) explained.
- [Modern C++ Template](https://github.com/filipdutescu/modern-cpp-template) - Template for modern C++ projects with CMake, CI/CD, and testing.
- [CMake Examples](https://github.com/ttroy50/cmake-examples) - Useful CMake examples for common use cases.
- [C++ Cheat Sheet](https://github.com/gibsjose/cpp-cheat-sheet) - C++ syntax, data structures, and algorithms reference.
- [Asynchronous Programming with Seastar](http://docs.seastar.io/master/tutorial.html) - High-performance asynchronous programming framework.

### Go

Tools and resources for Go development.

#### Official Resources

- [Go Official Website (China)](https://golang.google.cn/) - Official Go website for China region.
- [Go Module Proxy (China)](https://goproxy.io/) - Go module proxy for faster downloads in China.

#### Development Tools

- [g](https://github.com/voidint/g) - Go version manager. Easily switch between Go versions.
- [delve](https://github.com/go-delve/delve) - Debugger for the Go programming language.
- [goleak](https://github.com/uber-go/goleak) - Goroutine leak detector by Uber.
- [gcvis](https://github.com/davecheney/gcvis) - Visualize Go GC trace data in real-time.
- [go-spew](https://github.com/davecgh/go-spew) - Deep pretty printer for Go data structures.
- [kuberesolver](https://github.com/sercand/kuberesolver) - gRPC load balancer with Kubernetes resolver.

#### Learning Resources

- [Go Performance Book](https://github.com/dgryski/go-perfbook) - Thoughts on Go performance optimization.
- [Go HTTP/2 Testing Server](https://http2.golang.org/) - Online HTTP/2 testing server.

#### Utilities

- [JSON to Go Struct](http://json2struct.mervine.net/) - Convert JSON to Go struct definitions.

### Python

Tools and resources for Python development.

#### Performance & Profiling

- [scalene](https://github.com/plasma-umass/scalene) - High-performance CPU, GPU, and memory profiler with AI-powered optimization.
- [pycallgraph](https://github.com/gak/pycallgraph) - Create call graphs for Python programs.

#### Learning Resources

- [Matplotlib Cheat Sheets](https://github.com/matplotlib/cheatsheets) - Official Matplotlib cheat sheets.

### Rust

- [Rust in Databend](https://github.com/wubx/rust-in-databend) - Learn Rust through real-world database engineering.
- [Rust on Raspberry Pi OS](https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials) - Learn to write an embedded OS in Rust.

## Linux System Tools

Essential tools for Linux system administration and development.

### System Monitoring

- [glances](https://github.com/nicolargo/glances) - Modern system monitoring tool. A top/htop alternative with more features.
- [gtop](https://github.com/aksakalli/gtop) - System monitoring dashboard for terminal with beautiful interface.
- [iotop](http://guichaz.free.fr/iotop/) - Top-like UI for I/O monitoring.
- [noti](https://github.com/variadico/noti) - Monitor processes and trigger notifications on completion.

### Performance Analysis

- [perf](http://www.brendangregg.com/perf.html) - Linux performance analysis tools. Official kernel performance profiler.
- [perf-tools](https://github.com/brendangregg/perf-tools) - Unofficial Linux perf tools by Brendan Gregg.
- [fio](https://github.com/axboe/fio) - Flexible I/O tester and benchmark tool.
- [BCC](https://github.com/iovisor/bcc) - Tools for BPF-based Linux I/O analysis, networking, and monitoring.

### Process Management

- [goreman](https://github.com/mattn/goreman) - Foreman clone written in Go. Manage Procfile-based applications.
- [foreman](https://github.com/ddollar/foreman) - Manage Procfile-based applications.

### File & Directory Tools

- [fd](https://github.com/sharkdp/fd) - Simple, fast, user-friendly alternative to find.
- [ripgrep](https://github.com/BurntSushi/ripgrep) - Extremely fast grep alternative written in Rust.
- [fzf](https://github.com/junegunn/fzf) - Command-line fuzzy finder.
- [duf](https://github.com/muesli/duf) - Better df alternative with colorful output.
- [dust](https://github.com/bootandy/dust) - More intuitive du alternative.
- [nnn](https://github.com/jarun/nnn) - Fast, feature-rich terminal file manager.
- [broot](https://github.com/Canop/broot) - New way to see and navigate directory trees.

### Shell & Terminal

- [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) - Delightful framework for managing Zsh configuration.
- [Oh My Zsh Themes](https://github.com/ohmyzsh/ohmyzsh/wiki/themes) - Collection of themes for Oh My Zsh.
- [kitty](https://sw.kovidgoyal.net/kitty/) - Fast, feature-rich, GPU-based terminal emulator.
- [mosh](https://mosh.org/) - Mobile shell. Remote terminal that supports intermittent connectivity.
- [tldr](https://github.com/tldr-pages/tldr) - Simplified and community-driven man pages.
- [shellcheck](https://www.shellcheck.net/) - Static analysis tool for shell scripts.

### Debugging & Development

- [pwndbg](https://github.com/pwndbg/pwndbg) - GDB plugin that makes debugging with GDB easier.
- [OpenGrok](https://github.com/oracle/opengrok/wiki/How-to-setup-OpenGrok) - Fast and powerful source code search and cross-reference engine.

### Log Analysis

- [lnav](https://github.com/tstack/lnav) - Advanced log file navigator and analyzer.
- [ngxtop](https://github.com/lebinh/ngxtop) - Real-time metrics for Nginx server.

### Benchmarking

- [hyperfine](https://github.com/sharkdp/hyperfine) - Command-line benchmarking tool.
- [stress](https://linux.die.net/man/1/stress) - Tool to impose load on and stress test systems.

### Configuration Management

- [dotbot](https://github.com/anishathalye/dotbot) - Tool that bootstraps your dotfiles configuration.

### Networking

- [sshfs](https://github.com/libfuse/sshfs) - Network filesystem client to connect to SSH servers.

### System Utilities

- [util-linux](https://github.com/karelzak/util-linux) - Random collection of essential Linux utilities.
- [Toybox](https://github.com/landley/toybox) - All-in-one Linux command line utilities.

### Learning Resources

- [Awesome Linux Software](https://github.com/luong-komorebi/Awesome-Linux-Software) - List of awesome Linux applications and tools.

## Database Tools

Tools for database development and administration.

- [mycli](https://github.com/dbcli/mycli) - MySQL client with auto-completion and syntax highlighting.
- [iredis](https://github.com/laixintao/iredis) - Redis client with auto-completion and syntax highlighting.
- [records](https://github.com/kennethreitz/records) - SQL for Humans. Simple and intuitive SQL library.
- [sqlfluff](https://github.com/sqlfluff/sqlfluff) - SQL linter and auto-formatter.
- [DB Browser for SQLite](https://sqlitebrowser.org/dl/) - High-quality visual tool for SQLite databases.
- [MySQL Utils](https://github.com/pinterest/mysql_utils) - MySQL management and automation utilities by Pinterest.
- [Kafka Tool](https://www.kafkatool.com/) - GUI application for managing Apache Kafka clusters.

## Container & Orchestration

Tools for container and Kubernetes operations.

- [scope](https://github.com/weaveworks/scope) - Container and Kubernetes visualization and monitoring tool.
- [OperatorHub.io](https://operatorhub.io/) - Registry for Kubernetes operators.
- [nginxconfig.io](https://github.com/digitalocean/nginxconfig.io) - Nginx configuration generator with best practices.

## Performance & Profiling

Cross-language performance analysis and profiling tools.

- See language-specific sections for detailed profiling tools
- [Performance Ninja Class](https://github.com/dendibakh/perf-ninja) - Interactive course on performance optimization

## Terminal & CLI Enhancements

Make your terminal experience better.

- [FiraCode](https://github.com/tonsky/FiraCode) - Beautiful monospaced font with programming ligatures.
- See [Shell & Terminal](#shell--terminal) section for more tools

## Security & Penetration Testing

Tools for security testing and penetration testing.

- [BlackArch Sniffer Tools](https://blackarch.org/sniffer.html) - Collection of network sniffing tools.
- Note: Use these tools only in authorized environments and for legitimate security research.

## Productivity Tools

Tools to enhance productivity and workflow.

### Certificate Management

- [certstrap](https://github.com/square/certstrap) - Tools to bootstrap CAs, certificate requests, and signed certificates.

### Chaos Engineering

- [chaosblade](https://github.com/chaosblade-io/chaosblade) - Chaos engineering experiment toolkit.
- [chaosmonkey](https://github.com/Netflix/chaosmonkey) - Resiliency tool by Netflix for random instance failures.

### Documentation & Diagramming

- [Typora](https://typora.io/#linux) - Minimal markdown editor with live preview.
- [PlantUML Guide](https://zhuanlan.zhihu.com/p/76948461) - Efficiently draw diagrams with PlantUML.
- [Mermaid](https://github.com/mermaid-js/mermaid) - Generate diagrams from text in markdown-like syntax.
- [Diagrams](https://github.com/mingrammer/diagrams) - Draw cloud architecture diagrams in Python code.
- [noteshrink](https://github.com/mzucker/noteshrink) - Convert handwritten notes to beautiful PDFs.

### File Transfer

- [croc](https://github.com/schollz/croc) - Securely transfer files between computers.

### Screenshots

- [flameshot](https://github.com/flameshot-org/flameshot) - Powerful screenshot tool for Linux.

### Password Management

- [pass](https://www.passwordstore.org/) - Standard Unix password manager.

### Icons & Resources

- [devicon](https://github.com/devicons/devicon) - Set of icons representing programming languages and development tools.

### System Frameworks

- [Zeno](https://github.com/zenustech/zeno) - Open-source node system framework.

## Web-Based Tools

Useful web-based utilities for developers.

- [iPhone/iPad File Transfer](https://docstransfer.com/) - Transfer files to iOS devices via web browser.
- [GZIP Compression Test](http://www.gidnetwork.com/tools/gzip-test.php) - Check if web pages are properly compressed.
- [GPU Ladder](https://www.mydrivers.com/zhuanti/tianti/gpu/index.html) - GPU performance comparison (Chinese).
- [NVIDIA Container Images](https://gitlab.com/nvidia/container-images/cuda) - NVIDIA CUDA Docker image templates.
- [Chinese Traditional Colors](https://colors.ichuantong.cn/) - Reference for traditional Chinese color palettes.
- [English Font Generator](http://www.akuziti.com/yw/hk.php) - Generate beautiful English fonts (Chinese).
- [Mac Software Downloads](https://www.macbl.com/) - Mac application downloads (Chinese).

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

### Guidelines

1. Search previous suggestions before making a new one to avoid duplicates.
2. Make an individual pull request for each suggestion.
3. Use the following format: `[Name](link) - Description.`
4. New categories or improvements to the existing categorization are welcome.
5. Keep descriptions short, simple, and unbiased.
6. Check your spelling and grammar.
7. Make sure your text editor is set to remove trailing whitespace.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.
