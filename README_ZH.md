<div align="center">

# Awesome Engineering Toolbox [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

精心整理的软件工程师和开发者工具、框架、库和资源集合。本列表专注于实用的、生产级别的工具，能够提升你的开发工作流程和工程效率。

[English Version](README.md) • [贡献指南](#贡献指南)

</div>

---

## 目录

- [开发指南](#开发指南)
- [学习资源](#学习资源)
- [HTTP/HTTPS/gRPC 工具](#httphttpsgrpc-工具)
- [网络工具](#网络工具)
- [编程语言专用工具](#编程语言专用工具)
  - [C/C++](#cc)
  - [Go](#go)
  - [Python](#python)
  - [Rust](#rust)
- [Linux 系统工具](#linux-系统工具)
- [数据库工具](#数据库工具)
- [容器与编排](#容器与编排)
- [性能分析与调优](#性能分析与调优)
- [终端与命令行增强](#终端与命令行增强)
- [安全与渗透测试](#安全与渗透测试)
- [生产力工具](#生产力工具)
- [在线工具](#在线工具)

---

## 开发指南

软件开发最佳实践的重要资源。

- [如何选择开源许可证](https://choosealicense.com/) - 帮助你为项目选择合适许可证的指南。
- [语义化版本规范](https://semver.org/spec/v2.0.0.html) - 简单的版本号管理规则。
- [如何维护更新日志](https://keepachangelog.com/en/1.1.0/) - 维护有用的变更日志的指南。
- [Git 飞行规则](https://github.com/k88hudson/git-flight-rules) - Git 使用中遇到问题时的应对指南。
- [VSCode 调试指南](https://code.visualstudio.com/docs/editor/debugging) - VSCode 官方调试文档。

## 学习资源

成为更优秀工程师的高质量教育材料。

- [计算机教育中缺失的一课](https://missing-semester-cn.github.io/) - 掌握命令行、版本控制、文本编辑等技能。
- [高性能浏览器网络](https://hpbn.co/) - 网络协议和性能优化的综合指南。
- [Linux 内核源代码](https://elixir.bootlin.com/linux/latest/source) - 在线浏览 Linux 内核源代码。
- [Linux 内核图解](https://makelinux.github.io/kernel/) - Linux 内核内部结构的交互式图表。
- [CNCF 云原生全景图](https://landscape.cncf.io/) - 云原生生态系统的全面视图。
- [性能优化实战课](https://github.com/dendibakh/perf-ninja) - 学习性能分析和优化技术。
- [现代 CPU 性能分析与调优](https://github.com/dendibakh/perf-book) - CPU 性能深度指南。
- [Linux 追踪技术工作坊](https://github.com/goldshtn/linux-tracing-workshop) - 学习 Linux 追踪和性能分析工具。
- [Linux 服务器管理](https://github.com/livialima/linuxupskillchallenge) - 为期一月的 Linux 管理学习挑战。

## HTTP/HTTPS/gRPC 工具

用于 HTTP/HTTPS/gRPC 开发、测试和运维的工具。

### 请求与检查

- [httpstat](https://github.com/davecheney/httpstat) - 简化的 curl 统计信息。类似 `curl -v` 但带有颜色和更好的可视化。
- [wuzz](https://github.com/asciimoo/wuzz) - 交互式 HTTP 检查和调试命令行工具。
- [httping](https://www.vanheusden.com/httping/) - HTTP 请求的 ping 工具。测量延迟和可用性。

### 负载测试与基准测试

- [vegeta](https://github.com/tsenart/vegeta) - HTTP 负载测试工具，支持恒定请求速率。非常适合 API 压力测试。
- [hey](https://github.com/rakyll/hey) - 现代 HTTP 基准测试工具。ApacheBench (ab) 的优秀替代品。
- [wrk](https://github.com/wg/wrk) - 能产生显著负载的现代 HTTP 基准测试工具。多线程设计，支持事件通知机制。
- [Page Speed Insights](https://pagespeed.web.dev/) - 分析和优化 Web 应用性能。

### 测试与自动化

- [httprunner](https://github.com/httprunner/httprunner) - API/UI 测试框架，插件丰富、扩展性强。
- [goreplay](https://github.com/buger/goreplay) - 捕获并重放真实 HTTP 流量，用真实数据持续测试系统。

### gRPC 工具

- [grpcurl](https://github.com/fullstorydev/grpcurl) - 与 gRPC 服务器交互的命令行工具。gRPC 版的 curl。
- [ghz](https://github.com/bojand/ghz) - gRPC 基准测试和负载测试工具，提供详细统计信息。
- [grpc-tools](https://github.com/bradleyjkemp/grpc-tools) - gRPC 调试工具套件。gRPC 版的 Fiddler/Charles。

### 流量重放

- [tcpreplay](https://github.com/appneta/tcpreplay) - 用于编辑和重放 tcpdump/Wireshark 捕获的网络流量的工具套件。

## 网络工具

用于网络开发、监控和故障排查的综合工具集。

### 网络监控与诊断

- [gping](https://github.com/orf/gping) - 带图形的 ping 工具。实时可视化 ping 统计信息。
- [tcpprobe](https://github.com/mehrdadrad/tcpprobe) - 现代 TCP 性能观测工具。
- [nethogs](https://github.com/raboof/nethogs) - 按进程分组的网络带宽监控。网络版的 top。
- [iftop](http://www.ex-parrot.com/pdw/iftop) - 显示网络接口上主机对之间的带宽使用情况。

### 网络基础设施

- [netstat](https://linux.die.net/man/8/netstat) - 打印网络连接、路由表、接口统计等信息。
  ```bash
  sudo netstat -alnpt | grep ':$PORT'
  ```
- [ss](https://man7.org/linux/man-pages/man8/ss.8.html) - Socket 统计工具。比 netstat 更快，显示更多 TCP 信息。
  ```bash
  sudo ss -anpt | grep ':$PORT'
  ```
- [nmap](https://nmap.org/) - 网络发现和安全审计工具。
  ```bash
  sudo nmap -sT -O $TARGET_IP
  ```

### 性能测试与基准测试

- [iperf3](https://github.com/esnet/iperf) - 主动测量 IP 网络最大可达带宽的工具。
- [ntttcp](https://github.com/microsoft/ntttcp-for-linux) - 多线程 Linux 网络吞吐量基准测试工具。
- [netperf](https://github.com/HewlettPackard/netperf) - TCP/UDP/SOCKETS 协议的网络性能基准测试。
- [ethr](https://github.com/microsoft/ethr) - 微软出品的综合网络性能测量工具。支持 TCP、UDP、HTTP、HTTPS。

### 网络模拟

- [tc (netem)](https://man7.org/linux/man-pages/man8/tc-netem.8.html) - 用于测试协议的网络模拟。模拟延迟、丢包、重复和损坏。

### 网络代理

- [anyproxy](http://anyproxy.io/) - 带 Web 界面的 HTTP/HTTPS 流量代理，用于调试。

## 编程语言专用工具

### C/C++

C/C++ 工程的开发工具、库和资源。

#### 开发库

- [cpp-httplib](https://github.com/yhirose/cpp-httplib) - 单头文件 C++ HTTP/HTTPS 服务器和客户端库。
- [libunwind](http://download.savannah.gnu.org/releases/libunwind/) - 可移植且高效的 C 编程接口，用于确定调用链。

#### 性能分析

- [gperftools](https://github.com/gperftools/gperftools) - Google 出品的高性能多线程 malloc() 和性能分析工具。
  - [堆分析器](https://gperftools.github.io/gperftools/heapprofile.html) - 堆内存分析。
  - [堆检查器](https://gperftools.github.io/gperftools/heap_checker.html) - 内存泄漏检测。
  - [CPU 分析器](https://gperftools.github.io/gperftools/cpuprofile.html) - CPU 性能分析。
- [Valgrind](http://valgrind.org/) - 构建动态分析工具的框架。检测内存管理和线程 bug。

#### 学习资源

- [C++ 核心指南](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) - Bjarne Stroustrup 领导的协作成果。
- [Awesome C++](https://github.com/fffaraz/awesome-cpp) - 精选的 C/C++ 框架、库和资源列表。
- [Awesome Modern C++](https://github.com/rigtorp/awesome-modern-cpp) - 现代 C++ 资源集合。
- [现代 C++ 教程](https://github.com/changkun/modern-cpp-tutorial) - 现代 C++ 特性（C++11/14/17/20）讲解。
- [现代 C++ 项目模板](https://github.com/filipdutescu/modern-cpp-template) - 包含 CMake、CI/CD 和测试的现代 C++ 项目模板。
- [CMake 示例](https://github.com/ttroy50/cmake-examples) - 常见用例的实用 CMake 示例。
- [C++ 速查表](https://github.com/gibsjose/cpp-cheat-sheet) - C++ 语法、数据结构和算法参考。
- [Seastar 异步编程](http://docs.seastar.io/master/tutorial.html) - 高性能异步编程框架。

### Go

Go 开发的工具和资源。

#### 官方资源

- [Go 官方网站（中国）](https://golang.google.cn/) - Go 官方中国区网站。
- [Go 模块代理（中国）](https://goproxy.io/) - 中国区 Go 模块代理，加快下载速度。

#### 开发工具

- [g](https://github.com/voidint/g) - Go 版本管理工具。轻松切换 Go 版本。
- [delve](https://github.com/go-delve/delve) - Go 编程语言调试器。
- [goleak](https://github.com/uber-go/goleak) - Uber 出品的 Goroutine 泄漏检测器。
- [gcvis](https://github.com/davecheney/gcvis) - 实时可视化 Go GC 追踪数据。
- [go-spew](https://github.com/davecgh/go-spew) - Go 数据结构的深度美化打印器。
- [kuberesolver](https://github.com/sercand/kuberesolver) - 带 Kubernetes 解析器的 gRPC 负载均衡器。

#### 学习资源

- [Go 性能优化手册](https://github.com/dgryski/go-perfbook) - Go 性能优化思考。
- [Go HTTP/2 测试服务器](https://http2.golang.org/) - 在线 HTTP/2 测试服务器。

#### 实用工具

- [JSON 转 Go 结构体](http://json2struct.mervine.net/) - 将 JSON 转换为 Go 结构体定义。

### Python

Python 开发的工具和资源。

#### 性能分析

- [scalene](https://github.com/plasma-umass/scalene) - 高性能 CPU、GPU 和内存分析器，带 AI 驱动的优化建议。
- [pycallgraph](https://github.com/gak/pycallgraph) - 为 Python 程序创建调用图。

#### 学习资源

- [Matplotlib 速查表](https://github.com/matplotlib/cheatsheets) - Matplotlib 官方速查表。

### Rust

- [Rust in Databend](https://github.com/wubx/rust-in-databend) - 通过真实数据库工程学习 Rust。
- [树莓派 OS 开发（Rust）](https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials) - 学习用 Rust 编写嵌入式操作系统。

## Linux 系统工具

Linux 系统管理和开发的必备工具。

### 系统监控

- [glances](https://github.com/nicolargo/glances) - 现代系统监控工具。功能更丰富的 top/htop 替代品。
- [gtop](https://github.com/aksakalli/gtop) - 终端系统监控仪表板，界面精美。
- [iotop](http://guichaz.free.fr/iotop/) - I/O 监控的 top 工具。
- [noti](https://github.com/variadico/noti) - 监控进程并在完成时触发通知。

### 性能分析

- [perf](http://www.brendangregg.com/perf.html) - Linux 性能分析工具。官方内核性能分析器。
- [perf-tools](https://github.com/brendangregg/perf-tools) - Brendan Gregg 的非官方 Linux perf 工具。
- [fio](https://github.com/axboe/fio) - 灵活的 I/O 测试和基准测试工具。
- [BCC](https://github.com/iovisor/bcc) - 基于 BPF 的 Linux I/O 分析、网络和监控工具。

### 进程管理

- [goreman](https://github.com/mattn/goreman) - Go 编写的 Foreman 克隆。管理基于 Procfile 的应用。
- [foreman](https://github.com/ddollar/foreman) - 管理基于 Procfile 的应用。

### 文件与目录工具

- [fd](https://github.com/sharkdp/fd) - 简单、快速、用户友好的 find 替代品。
- [ripgrep](https://github.com/BurntSushi/ripgrep) - Rust 编写的极快 grep 替代品。
- [fzf](https://github.com/junegunn/fzf) - 命令行模糊查找器。
- [duf](https://github.com/muesli/duf) - 更好的 df 替代品，彩色输出。
- [dust](https://github.com/bootandy/dust) - 更直观的 du 替代品。
- [nnn](https://github.com/jarun/nnn) - 快速、功能丰富的终端文件管理器。
- [broot](https://github.com/Canop/broot) - 查看和导航目录树的新方式。

### Shell 与终端

- [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) - 令人愉快的 Zsh 配置管理框架。
- [Oh My Zsh 主题](https://github.com/ohmyzsh/ohmyzsh/wiki/themes) - Oh My Zsh 主题集合。
- [kitty](https://sw.kovidgoyal.net/kitty/) - 快速、功能丰富、基于 GPU 的终端模拟器。
- [mosh](https://mosh.org/) - 移动 Shell。支持间歇性连接的远程终端。
- [tldr](https://github.com/tldr-pages/tldr) - 简化的社区驱动的 man 手册。
- [shellcheck](https://www.shellcheck.net/) - Shell 脚本静态分析工具。

### 调试与开发

- [pwndbg](https://github.com/pwndbg/pwndbg) - 让 GDB 调试更简单的插件。
- [OpenGrok](https://github.com/oracle/opengrok/wiki/How-to-setup-OpenGrok) - 快速强大的源代码搜索和交叉引用引擎。

### 日志分析

- [lnav](https://github.com/tstack/lnav) - 高级日志文件导航和分析器。
- [ngxtop](https://github.com/lebinh/ngxtop) - Nginx 服务器的实时指标。

### 基准测试

- [hyperfine](https://github.com/sharkdp/hyperfine) - 命令行基准测试工具。
- [stress](https://linux.die.net/man/1/stress) - 对系统施加负载和压力测试的工具。

### 配置管理

- [dotbot](https://github.com/anishathalye/dotbot) - 引导配置文件的工具。

### 网络工具

- [sshfs](https://github.com/libfuse/sshfs) - 连接到 SSH 服务器的网络文件系统客户端。

### 系统实用工具

- [util-linux](https://github.com/karelzak/util-linux) - 基本 Linux 实用工具的随机集合。
- [Toybox](https://github.com/landley/toybox) - 一体化 Linux 命令行实用工具。

### 学习资源

- [Awesome Linux Software](https://github.com/luong-komorebi/Awesome-Linux-Software) - Linux 应用程序和工具列表。

## 数据库工具

数据库开发和管理工具。

- [mycli](https://github.com/dbcli/mycli) - 带自动补全和语法高亮的 MySQL 客户端。
- [iredis](https://github.com/laixintao/iredis) - 带自动补全和语法高亮的 Redis 客户端。
- [records](https://github.com/kennethreitz/records) - 人性化的 SQL。简单直观的 SQL 库。
- [sqlfluff](https://github.com/sqlfluff/sqlfluff) - SQL 代码检查和自动格式化工具。
- [DB Browser for SQLite](https://sqlitebrowser.org/dl/) - 高质量的 SQLite 数据库可视化工具。
- [MySQL Utils](https://github.com/pinterest/mysql_utils) - Pinterest 的 MySQL 管理和自动化工具。
- [Kafka Tool](https://www.kafkatool.com/) - 管理 Apache Kafka 集群的 GUI 应用。

## 容器与编排

容器和 Kubernetes 运维工具。

- [scope](https://github.com/weaveworks/scope) - 容器和 Kubernetes 可视化监控工具。
- [OperatorHub.io](https://operatorhub.io/) - Kubernetes Operator 注册中心。
- [nginxconfig.io](https://github.com/digitalocean/nginxconfig.io) - Nginx 配置生成器，遵循最佳实践。

## 性能分析与调优

跨语言的性能分析和调优工具。

- 详细的分析工具请查看各语言专用章节
- [性能优化实战课](https://github.com/dendibakh/perf-ninja) - 性能优化互动课程

## 终端与命令行增强

让你的终端体验更出色。

- [FiraCode](https://github.com/tonsky/FiraCode) - 带编程连字的优美等宽字体。
- 更多工具请查看 [Shell 与终端](#shell-与终端) 章节

## 安全与渗透测试

安全测试和渗透测试工具。

- [BlackArch 嗅探工具](https://blackarch.org/sniffer.html) - 网络嗅探工具集合。
- 注意：仅在授权环境中使用这些工具，用于合法的安全研究。

## 生产力工具

提升生产力和工作流程的工具。

### 证书管理

- [certstrap](https://github.com/square/certstrap) - 引导 CA、证书请求和签名证书的工具。

### 混沌工程

- [chaosblade](https://github.com/chaosblade-io/chaosblade) - 混沌工程实验工具包。
- [chaosmonkey](https://github.com/Netflix/chaosmonkey) - Netflix 出品的弹性测试工具，用于随机实例故障。

### 文档与图表

- [Typora](https://typora.io/#linux) - 带实时预览的极简 Markdown 编辑器。
- [PlantUML 指南](https://zhuanlan.zhihu.com/p/76948461) - 用 PlantUML 高效绘制图表。
- [Mermaid](https://github.com/mermaid-js/mermaid) - 用类 Markdown 语法从文本生成图表。
- [Diagrams](https://github.com/mingrammer/diagrams) - 用 Python 代码绘制云架构图。
- [noteshrink](https://github.com/mzucker/noteshrink) - 将手写笔记转换为精美 PDF。

### 文件传输

- [croc](https://github.com/schollz/croc) - 计算机之间安全传输文件。

### 截图

- [flameshot](https://github.com/flameshot-org/flameshot) - Linux 强大的截图工具。

### 密码管理

- [pass](https://www.passwordstore.org/) - 标准的 Unix 密码管理器。

### 图标与资源

- [devicon](https://github.com/devicons/devicon) - 代表编程语言和开发工具的图标集。

### 系统框架

- [Zeno](https://github.com/zenustech/zeno) - 开源节点系统框架。

## 在线工具

对开发者有用的在线实用工具。

- [iPhone/iPad 文件传输](https://docstransfer.com/) - 通过 Web 浏览器传输文件到 iOS 设备。
- [GZIP 压缩测试](http://www.gidnetwork.com/tools/gzip-test.php) - 检查网页是否正确压缩。
- [显卡天梯图](https://www.mydrivers.com/zhuanti/tianti/gpu/index.html) - GPU 性能对比。
- [NVIDIA 容器镜像](https://gitlab.com/nvidia/container-images/cuda) - NVIDIA CUDA Docker 镜像模板。
- [中国传统颜色](https://colors.ichuantong.cn/) - 中国传统色彩参考。
- [英文字体生成器](http://www.akuziti.com/yw/hk.php) - 生成精美英文字体。
- [Mac 软件下载](https://www.macbl.com/) - Mac 应用程序下载。

---

## 贡献指南

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。

### 指南

1. 在提出新建议之前，请先搜索以前的建议，避免重复。
2. 每个建议单独提交一个 Pull Request。
3. 使用以下格式：`[名称](链接) - 描述。`
4. 欢迎新的分类或改进现有分类。
5. 保持描述简短、简洁和中立。
6. 检查拼写和语法。
7. 确保文本编辑器设置为删除尾随空格。

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

在法律允许的范围内，贡献者已放弃本作品的所有版权和相关或邻接权。
