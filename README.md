# Awesome Sysadmin

[![](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![](https://github.com/awesome-foss/awesome-sysadmin/actions/workflows/ci.yml/badge.svg)](https://github.com/awesome-foss/awesome-sysadmin/issues/416)

**一个精心策划的极其优秀的自由和开源系统管理员资源列表。** 如果你希望添加软件，请阅读 [Pull Request 模板](./.github/PULL_REQUEST_TEMPLATE.md)，并考虑[捐赠](https://github.com/n1trux/awesome-donations)给你经常使用的 FLOSS 项目。如果你有时间，也请考虑为修复置顶的 [issues](https://github.com/awesome-foss/awesome-sysadmin/issues) 做出贡献。

--------------------

## Table of contents

- [Software](#software)
  - [Automation](#automation)
  - [Backups](#backups)
  - [Build and software organization tools](#build-and-software-organization-tools)
  - [ChatOps](#chatops)
  - [Cloud Computing](#cloud-computing)
  - [Code Review](#code-review)
  - [Configuration Management](#configuration-management)
  - [Configuration Management Database](#configuration-management-database)
  - [Continuous Integration & Continuous Deployment](#continuous-integration--continuous-deployment)
  - [Control Panels](#control-panels)
  - [Databases](#databases)
  - [Deployment Automation](#deployment-automation)
  - [Diagramming](#diagramming)
  - [Distributed Filesystems](#distributed-filesystems)
  - [DNS - Control Panels & Domain Management](#dns---control-panels--domain-management)
  - [DNS - Servers](#dns---servers)
  - [Editors](#editors)
  - [Identity Management](#identity-management)
  - [Identity Management - LDAP](#identity-management---ldap)
  - [Identity Management - Single Sign-On (SSO)](#identity-management---single-sign-on-sso)
  - [Identity Management - Tools and web interfaces](#identity-management---tools-and-web-interfaces)
  - [IT Asset Management](#it-asset-management)
  - [Log Management](#log-management)
  - [Mail Clients](#mail-clients)
  - [Metrics & Metric Collection](#metrics--metric-collection)
  - [Miscellaneous](#miscellaneous)
  - [Monitoring](#monitoring)
  - [Network Configuration Management](#network-configuration-management)
  - [PaaS](#paas)
  - [Packaging](#packaging)
  - [Project Management](#project-management)
  - [Queuing](#queuing)
  - [Remote Desktop Clients](#remote-desktop-clients)
  - [Router](#router)
  - [Service Discovery](#service-discovery)
  - [Software Containers](#software-containers)
  - [Status Pages](#status-pages)
  - [Troubleshooting](#troubleshooting)
  - [Version control](#version-control)
  - [Virtualization](#virtualization)
  - [VPN](#vpn)
  - [Web](#web)
- [List of Licenses](#list-of-licenses)
- [External links](#external-links)
- [Communities / Forums](#communities--forums)
- [Repositories](#repositories)
- [Websites](#websites)
- [License](#license)

--------------------

## 软件

### 自动化

**[`^        返回顶部        ^`](#awesome-sysadmin)**

构建自动化。

- [Apache Ant](https://ant.apache.org/) - 自动化构建工具，类似于 make，是一个库和命令行工具，其任务是驱动在构建文件中描述的目标和扩展点，这些目标和扩展点彼此依赖。([源码](https://github.com/apache/ant)) `Apache-2.0` `Java`
- [Apache Maven](https://maven.apache.org/) - 主要用于 Java 的构建自动化工具。一个软件项目管理和理解工具。基于项目对象模型（POM）的概念，Maven 可以从一处信息管理项目的构建、报告和文档。([源码](https://github.com/apache/maven)) `Apache-2.0` `Java`
- [Bazel](https://www.bazel.io/) - 一个快速、可扩展、多语言且可扩展的构建系统。由 Google 使用。([源码](https://github.com/bazelbuild/bazel/)) `Apache-2.0` `Java`
- [Bolt](https://www.puppet.com/community/open-source/bolt) - 可用于运行一次性任务、脚本以自动化部分节点的配置和管理，也可用于超越脚本并使其可共享。([源码](https://github.com/puppetlabs/bolt)) `Apache-2.0` `Ruby`
- [GNU Make](https://www.gnu.org/software/make/) - 最流行的自动化构建工具之一，适用于多种用途。make 控制从源文件生成可执行文件和其他非源文件。([源码](https://git.savannah.gnu.org/cgit/make.git)) `GPL-3.0` `C`
- [Gradle](https://gradle.org/) - 另一种构建自动化系统。([源码](https://github.com/gradle/gradle)) `Apache-2.0` `Groovy/Java`
- [Rake](https://ruby.github.io/rake/) - 类似于 Make 的构建自动化工具，用 Ruby 编写并可扩展。([源码](https://github.com/ruby/rake)) `MIT` `Ruby`

### 备份

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[备份](https://en.wikipedia.org/wiki/Backup) 软件。

_另见：[Restic 的 Linux 备份软件列表](https://github.com/restic/others)_

- [Backupninja](https://0xacab.org/liberate/backupninja) - 轻量级、可扩展的元备份系统，提供集中方式配置和协调多种备份工具。`GPL-2.0` `Shell`
- [Backrest](https://garethgeorge.github.io/backrest/) - restic 备份的 Web UI 和编排器。([源码](https://github.com/garethgeorge/backrest)) `GPL-3.0` `Docker/Go`
- [Bareos](https://www.bareos.org/) - 跨网络备份解决方案，可对所有主流操作系统的数据进行保存、归档和恢复。([源码](https://github.com/bareos/bareos)) `AGPL-3.0` `C++/C`
- [Barman](https://pgbarman.org) - PostgreSQL 的备份和恢复管理器。([源码](https://github.com/EnterpriseDB/barman)) `GPL-3.0` `Python`
- [BorgBackup](https://www.borgbackup.org/) - 支持去重、压缩和认证加密的归档工具。([源码](https://github.com/borgbackup/borg)) `BSD-3-Clause` `Python`
- [Burp](https://burp.grke.org/) - 网络备份和恢复程序。([源码](https://github.com/grke/burp)) `AGPL-3.0` `C`
- [Dar](http://dar.linux.free.fr/) - Disk ARchive，功能丰富、健壮的归档和备份软件，类似 tar。([源码](https://github.com/Edrusb/DAR)) `GPL-2.0` `C++`
- [Duplicati](https://www.duplicati.com) - 备份客户端，可将加密、增量、压缩的备份安全地存储到云存储服务和远程文件服务器。([源码](https://github.com/duplicati/duplicati)) `LGPL-2.1` `C#`
- [Duplicity](https://duplicity.gitlab.io/) - 使用 rsync 算法的加密高效带宽备份工具。([源码](https://gitlab.com/duplicity/duplicity)) `GPL-2.0` `Python`
- [Proxmox Backup Server](https://www.proxmox.com/en/proxmox-backup-server) - 企业级、客户端-服务器架构的备份解决方案，可备份虚拟机、容器和物理主机。([源码](https://git.proxmox.com/?p=proxmox-backup.git;a=tree)) `GPL-3.0` `Rust`
- [rclone](https://rclone.org/) - 命令行程序，用于在不同云存储提供商之间同步文件和目录。([源码](https://github.com/rclone/rclone)) `MIT` `Go`
- [Rdiff-backup](https://rdiff-backup.net/) - 反向增量备份工具，可通过网络或本地使用。([源码](https://github.com/rdiff-backup/rdiff-backup)) `GPL-2.0` `Python`
- [Restic](https://restic.net/) - 简单、快速、可验证、安全且高效的远程备份工具。([源码](https://github.com/restic/restic)) `BSD-2-Clause` `Go`
- [Rsnapshot](https://rsnapshot.org/) - 基于 rsync 的文件系统快照工具。([源码](https://github.com/rsnapshot/rsnapshot)) `GPL-2.0` `Perl`
- [Shield](https://github.com/starkandwayne/shield) - 数据库系统备份与恢复的可插拔架构。`MIT` `Go`
- [UrBackup](https://www.urbackup.org/) - 面向 Windows、MacOS 和 Linux 的开源客户端/服务器网络备份。([源码](https://github.com/uroni/urbackup_backend)) `AGPL-3.0` `C/C++`


### 构建与软件组织工具

**[`^        返回顶部        ^`](#awesome-sysadmin)**

构建与软件组织工具。

- [EasyBuild](https://easybuild.io/) - EasyBuild 以高效的方式为高性能计算（HPC）系统构建软件和模块文件。([源码](https://github.com/easybuilders/easybuild-easyconfigs)) `GPL-2.0` `Python`
- [Environment Modules](https://cea-hpc.github.io/modules/) - Environment Modules 通过 modulefiles 动态修改用户环境。([源码](https://github.com/cea-hpc/modules)) `GPL-2.0` `Tcl`
- [Lmod](https://www.tacc.utexas.edu/research-development/tacc-projects/lmod) - 基于 Lua 的模块系统，轻松处理 MODULEPATH 层级问题。([源码](https://github.com/TACC/Lmod)) `MIT` `Lua`
- [Spack](https://spack.io/) - 灵活的软件包管理器，支持多版本、多配置、多平台和多编译器。([源码](https://github.com/spack/spack)) `MIT/Apache-2.0` `Python`


### ChatOps

**[`^        返回顶部        ^`](#awesome-sysadmin)**

对话驱动的开发与管理。

_另见: [/r/chatops](https://old.reddit.com/r/chatops)_

- [Eggdrop](https://www.eggheads.org/) - 最早的 IRC 机器人，仍在积极开发中。([源码](https://github.com/eggheads/eggdrop)) `GPL-2.0` `C`
- [Errbot](https://errbot.io/) - 基于插件的聊天机器人，易于部署、扩展和维护。([源码](https://github.com/errbotio/errbot)) `GPL-3.0` `Python`
- [Hubot](https://hubot.github.com/) - 可定制的自动化机器人。([源码](https://github.com/hubotio/hubot)) `MIT` `Nodejs`


### 云计算

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[云计算](https://en.wikipedia.org/wiki/Cloud_computing) 指计算机系统资源（尤其是数据存储和计算能力）的按需可用性，无需用户直接管理。

**请访问 [Cloud Native Software Landscape](https://landscape.cncf.io/?group=projects-and-products&view-mode=card)**



### 代码评审

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[代码评审](https://en.wikipedia.org/wiki/Code_review) 是一种软件质量保证活动，主要通过查看和阅读源代码的部分内容来检查程序。

**请访问 [awesome-selfhosted/Software Development - Project Management](https://awesome-selfhosted.net/tags/software-development---project-management.html)**



### 配置管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[配置管理（CM）](https://en.wikipedia.org/wiki/Configuration_management) 是一种系统工程流程，用于在产品整个生命周期内建立和维护其性能、功能和物理属性与其需求、设计和操作信息的一致性。

- [Ansible](https://www.ansible.com/) - 提供配置管理、应用部署等功能的自动化工具。([源码](https://github.com/ansible/ansible)) `GPL-3.0` `Python`
- [CFEngine](https://cfengine.com/) - 用于大规模计算机系统自动配置和维护的配置管理系统。([源码](https://github.com/cfengine/core)) `GPL-3.0` `C`
- [Chef](https://www.chef.io/products/chef-infra) - 使用纯 Ruby DSL 编写系统配置“食谱”的配置管理工具。([源码](https://github.com/chef/chef)) `Apache-2.0` `Ruby`
- [cloud-init](https://cloud-init.io/) - 自动化配置虚拟机、云实例或网络中机器的初始化工具。([源码](https://github.com/canonical/cloud-init)) `GPL-3.0/Apache-2.0` `Python`
- [Puppet](https://www.puppet.com/) - 软件配置管理工具，包含描述系统配置的声明式语言。([源码](https://github.com/puppetlabs/puppet)) `Apache-2.0` `Ruby/C`
- [Rudder](https://www.rudder.io/) - 基于 CFEngine 的可扩展动态配置管理系统，支持补丁、安全与合规。([源码](https://github.com/Normation/rudder)) `GPL-3.0` `Scala`
- [Salt](https://docs.saltproject.io/) - 事件驱动的 IT 自动化、远程任务执行和配置管理软件。([源码](https://github.com/saltstack/salt)) `Apache-2.0` `Python`


### 配置管理数据库

**[`^        返回顶部        ^`](#awesome-sysadmin)**

配置管理数据库（CMDB）软件。

_相关：[IT 资产管理](#it-asset-management)_

- [Collins](https://tumblr.github.io/collins/) - Tumblr 的基础设施事实与知识源。([源码](https://github.com/tumblr/collins)) `Apache-2.0` `Docker/Scala`
- [i-doit](https://www.i-doit.org/) - IT 文档与 CMDB。`AGPL-3.0` `PHP`
- [iTop](https://www.combodo.com/itop-193) - 完整的 ITIL Web 服务管理工具。([源码](https://sourceforge.net/projects/itop/files/)) `AGPL-3.0` `PHP`
- [netbox](https://netbox.dev/) - IP 地址管理（IPAM）和数据中心基础设施管理（DCIM）工具。([演示](https://demo.netbox.dev/), [源码](https://github.com/netbox-community/netbox)) `Apache-2.0` `Python`


### 持续集成与持续部署

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[持续集成](https://en.wikipedia.org/wiki/Continuous_integration)/[持续部署](https://en.wikipedia.org/wiki/Continuous_deployment) 软件。

- [Buildbot](https://buildbot.net/) - 基于 Python 的持续集成工具包。([源码](https://github.com/buildbot/buildbot)) `GPL-2.0` `Python`
- [CDS](https://ovh.github.io/cds/) - 企业级持续交付与 DevOps 自动化开源平台。([源码](https://github.com/ovh/cds)) `BSD-3-Clause` `Go`
- [Concourse](https://concourse-ci.org/) - 以流水线为一等公民、每一步都容器化的 CI 工具。([演示](https://ci.concourse-ci.org/), [源码](https://github.com/concourse/concourse)) `Apache-2.0` `Go`
- [drone](https://drone.io/) - 基于 Docker、用 Go 编写的持续交付平台。([源码](https://github.com/drone/drone)) `Apache-2.0` `Go`
- [Factor](https://www.factor.io/) - 以编程方式定义和运行工作流，连接配置管理、源码管理、构建、CI/CD 和通信工具。([源码](https://github.com/factor-io/factor)) `MIT` `Ruby`
- [GitLab CI](https://about.gitlab.com/solutions/continuous-integration/) - GitLab 内置的全功能 CI/CD 解决方案。([源码](https://gitlab.com/gitlab-org/gitlab-foss)) `MIT` `Ruby`
- [GoCD](https://www.go.cd/) - 持续交付服务器。([源码](https://github.com/gocd/gocd)) `Apache-2.0` `Java/Ruby`
- [Jenkins](https://jenkins-ci.org/) - 持续集成服务器。([源码](https://github.com/jenkinsci/jenkins/)) `MIT` `Java`
- [Laminar](https://laminar.ohwg.net) - 快速、轻量、简单且灵活的持续集成。([源码](https://github.com/ohwgiles/laminar)) `GPL-3.0` `C++`
- [PHP Censor](https://github.com/php-censor/php-censor) - 面向 PHP 项目的自托管持续集成服务器。`BSD-2-Clause` `PHP`
- [Strider](https://strider-cd.github.io/) - 开源持续部署/持续集成平台。([源码](https://github.com/Strider-CD/strider)) `MIT` `Nodejs`
- [Terrateam](https://terrateam.io) - 针对 Terraform 和 OpenTofu 工作流的 GitOps 优先自动化平台，支持自托管运行器。([源码](https://github.com/terrateamio/terrateam)) `MPL-2.0` `OCaml/Docker`
- [werf](https://werf.io/) - 用于构建 Docker 镜像并通过 GitOps 部署到 Kubernetes 的开源 CI/CD 工具。([源码](https://github.com/werf/werf)) `Apache-2.0` `Go`
- [Woodpecker](https://woodpecker-ci.org/) - Drone 的社区分支，使用 Docker 容器。([源码](https://github.com/woodpecker-ci/woodpecker)) `Apache-2.0` `Go`


### 控制面板

**[`^        返回顶部        ^`](#awesome-sysadmin)**

Web 托管与服务器或服务控制面板。

- [Ajenti](https://ajenti.org/) - Linux 和 BSD 的控制面板。([源码](https://github.com/ajenti/ajenti)) `MIT` `Python/Shell`
- [Cockpit](https://cockpit-project.org/) - 服务器的 Web 图形界面。([源码](https://github.com/cockpit-project/cockpit)) `LGPL-2.1` `C`
- [Froxlor](https://froxlor.org/) - 轻量级服务器管理软件，支持 Nginx 和 PHP-FPM。([源码](https://github.com/Froxlor/Froxlor/)) `GPL-2.0` `PHP`
- [HestiaCP](https://hestiacp.com/) - Web 服务器控制面板（VestaCP 分支）。([演示](https://demo.hestiacp.com:8083/login/), [源码](https://github.com/hestiacp/hestiacp)) `GPL-3.0` `PHP/Shell/Other`
- [ISPConfig](https://www.ispconfig.org) - 通过浏览器直接管理 Linux 服务器。([源码](https://git.ispconfig.org/ispconfig/ispconfig3)) `BSD-3-Clause` `PHP`
- [Sentora](https://sentora.org/) - Linux、BSD 的开源 Web 托管控制面板（ZPanel 分支）。([源码](https://github.com/sentora/sentora-core)) `GPL-3.0` `PHP`
- [Virtualmin](https://www.virtualmin.com/) - Linux 和 BSD 系统的强大灵活的 Web 托管控制面板。([源码](https://github.com/virtualmin)) `GPL-3.0` `Shell/Perl/Other`
- [Webmin](https://www.webmin.com/) - Unix 系统管理的 Web 界面。([源码](https://github.com/webmin/webmin)) `BSD-3-Clause` `Perl`


### 数据库

**[`^        返回顶部        ^`](#awesome-sysadmin)**

数据库服务器。

**请访问 [dbdb.io - Database of Databases](https://dbdb.io/)**

_另见：[awesome-selfhosted/Database Management](https://awesome-selfhosted.net/tags/database-management.html)_



### 部署自动化

**[`^        返回顶部        ^`](#awesome-sysadmin)**

支持服务器部署的工具和脚本。

- [Capistrano](https://capistranorb.com/) - 通过 SSH（基于 rake）同时、顺序或滚动方式将应用部署到任意数量的机器。([源码](https://github.com/capistrano/capistrano)) `MIT` `Ruby`
- [CloudSlang](https://www.cloudslang.io/) - 基于流程的编排工具，用于管理已部署应用，支持 Docker。([源码](https://github.com/CloudSlang/score)) `Apache-2.0` `Java`
- [CloudStack](https://cloudstack.apache.org/) - 用于创建、管理和部署基础设施云服务的云计算软件。([源码](https://github.com/apache/cloudstack)) `Apache-2.0` `Java/Python`
- [Cobbler](https://cobbler.github.io/) - Linux 安装服务器，可快速搭建网络安装环境。([源码](https://github.com/cobbler/cobbler)) `GPL-2.0` `Python`
- [Fabric](https://www.fabfile.org/) - 用于简化通过 SSH 部署应用或系统管理任务的 Python 库和 CLI 工具。([源码](https://github.com/fabric/fabric)) `BSD-2-Clause` `Python`
- [Genesis](https://github.com/starkandwayne/genesis) - 多环境 BOSH 部署的模板框架。`MIT` `Perl`
- [munki](https://www.munki.org/munki/) - 基于 Web 服务器的软件包及元数据仓库，便于 macOS 管理员管理软件安装。([源码](https://github.com/munki/munki)) `Apache-2.0` `Python`
- [Overcast](https://andrewchilds.github.io/overcast/) - 跨云服务商部署虚拟机，并通过 SSH 并行运行命令和脚本。([源码](https://github.com/andrewchilds/overcast)) `MIT` `Nodejs`


### 绘图

**[`^        返回顶部        ^`](#awesome-sysadmin)**

用于创建网络、流程等图表的工具。

- [Diagrams.net](https://app.diagrams.net/) - 又名 [Draw.io](https://app.diagrams.net/)。易用的图表 UI，内置丰富模板。([源码](https://github.com/jgraph/drawio)) `Apache-2.0` `JavaScript/Docker`
- [Kroki](https://kroki.io) - 基于文本描述生成图表的 API。([源码](https://github.com/yuzutech/kroki)) `MIT` `Java`
- [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/) - 具有独特简洁语法的 JavaScript 绘图模块，可集成到 Grafana 等多种工具。([源码](https://github.com/mermaid-js/mermaid-live-editor)) `MIT` `Nodejs/Docker`


### 分布式文件系统

**[`^        返回顶部        ^`](#awesome-sysadmin)**

网络分布式文件系统。

_另见：[awesome-selfhosted/File Transfer - Object Storage & File Servers](https://awesome-selfhosted.net/tags/file-transfer---object-storage--file-servers.html)_

- [Ceph](https://ceph.com/en/) - 分布式对象、块和文件存储平台。([源码](https://github.com/ceph/ceph)) `LGPL-3.0` `C++`
- [DRBD](https://linbit.com/drbd/) - 分布式复制存储系统，作为 Linux 内核驱动实现。([源码](https://github.com/LINBIT/drbd)) `GPL-2.0` `C`
- [GlusterFS](https://www.gluster.org/) - 软件定义的分布式存储，可扩展到数 PB，支持对象、块和文件存储接口。([源码](https://github.com/gluster/glusterfs)) `GPL-2.0/LGPL-3.0` `C`
- [Hadoop Distributed Filesystem (HDFS)](https://hadoop.apache.org/) - 提供高吞吐量访问应用数据的分布式文件系统。([源码](https://github.com/apache/hadoop)) `Apache-2.0` `Java`
- [JuiceFS](https://juicefs.com/) - 基于 Redis 和 S3 构建的分布式 POSIX 文件系统。([源码](https://github.com/juicedata/juicefs)) `Apache-2.0` `Go`
- [Kubo](https://github.com/ipfs/kubo) - IPFS 的实现，一个全球、版本化、点对点的文件系统，旨在连接所有计算设备。`Apache-2.0/MIT` `Go`
- [LeoFS](https://leo-project.net) - 高可用、分布式、最终一致性的对象/Blob 存储。([源码](https://github.com/leo-project/leofs)) `Apache-2.0` `Erlang`
- [Lustre](https://www.lustre.org/) - 并行分布式文件系统，常用于大规模集群计算。([源码](https://git.whamcloud.com/?p=fs/lustre-release.git;a=summary)) `GPL-2.0` `C`
- [Minio](https://min.io/) - 高性能、兼容 S3 的对象存储，适用于大规模 AI/ML、数据湖和数据库工作负载。([源码](https://github.com/minio/minio)) `AGPL-3.0` `Go`
- [MooseFS](https://moosefs.com/) - 容错的网络分布式文件系统。([源码](https://github.com/moosefs/moosefs)) `GPL-2.0` `C`
- [OpenAFS](https://www.openafs.org/) - 支持只读副本和多操作系统的分布式网络文件系统。([源码](https://git.openafs.org/?p=openafs.git;a=summary)) `IPL-1.0` `C`
- [Openstack Swift](https://docs.openstack.org/developer/swift/) - 高可用、分布式、最终一致性的对象/Blob 存储。([源码](https://opendev.org/openstack/swift)) `Apache-2.0` `Python`
- [Perkeep](https://perkeep.org/) - 一组用于建模、存储、搜索、共享和同步数据的开源格式、协议和软件（前身为 Camlistore）。([源码](https://github.com/perkeep/perkeep)) `Apache-2.0` `C`
- [TahoeLAFS](https://tahoe-lafs.org/trac/tahoe-lafs) - 安全、去中心化、容错的点对点分布式数据存储和文件系统。([源码](https://github.com/tahoe-lafs/tahoe-lafs)) `GPL-2.0` `Python`
- [XtreemFS](https://www.xtreemfs.org/) - 面向联合 IT 基础设施的分布式、复制和容错文件系统。([源码](https://github.com/xtreemfs/xtreemfs)) `BSD-3-Clause` `Java`


### DNS - 控制面板与域名管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

DNS 服务器控制面板、Web 界面和域名管理工具。

_相关：[DNS - 服务器](#dns---servers)_

_另见：[awesome-selfhosted/DNS](https://awesome-selfhosted.net/tags/dns.html)_

- [Atomia DNS](https://github.com/atomia/atomiadns/) - DNS 管理系统。`ISC` `Perl`
- [Designate](https://wiki.openstack.org/wiki/Designate) - OpenStack 的 DNSaaS 服务。([源码](https://opendev.org/openstack/designate)) `Apache-2.0` `Python`
- [DNSControl](https://stackexchange.github.io/dnscontrol/) - 使用简单 DSL 同步多个提供商的 DNS。([源码](https://github.com/StackExchange/dnscontrol)) `MIT` `Go/Docker`
- [DomainMOD](https://domainmod.org) - 在中心位置管理你的域名和其他互联网资产。([源码](https://github.com/domainmod/domainmod)) `GPL-3.0` `PHP`
- [nsupdate.info](https://www.nsupdate.info/) - 动态 DNS 服务。([演示](https://www.nsupdate.info/account/register/), [源码](https://github.com/nsupdate-info/nsupdate.info)) `BSD-3-Clause` `Python`
- [octoDNS](https://github.com/github/octodns) - DNS 即代码 - 管理多提供商 DNS 的工具。`MIT` `Python`
- [Poweradmin](https://www.poweradmin.org/) - PowerDNS 服务器的 Web 控制面板。([源码](https://github.com/poweradmin/poweradmin)) `GPL-3.0` `PHP`
- [SPF Toolbox](https://spftoolbox.com) - 用于查询 SPF、MX、Whois 等 DNS 记录的应用。([源码](https://github.com/charlesabarnes/SPFtoolbox)) `MIT` `PHP`


### DNS - 服务器

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[DNS](https://en.wikipedia.org/wiki/Name_server) 服务器。

_相关：[DNS - 控制面板与域名管理](#dns---控制面板与域名管理)_

_另见：[awesome-selfhosted/DNS](https://awesome-selfhosted.net/tags/dns.html)_

- [Bind](https://www.isc.org/bind/) - 多功能、经典、完整的名称服务器软件。([源码](https://gitlab.isc.org/isc-projects/bind9)) `MPL-2.0` `C`
- [CoreDNS](https://coredns.io/) - 灵活的 DNS 服务器。([源码](https://github.com/coredns/coredns)) `Apache-2.0` `Go`
- [djbdns](https://cr.yp.to/djbdns.html) - 一组 DNS 应用，包括 tinydns。([源码](https://salsa.debian.org/debian/djbdns)) `CC0-1.0` `C`
- [dnsmasq](https://www.thekelleys.org.uk/dnsmasq/doc.html) - 为小型网络提供 DNS、DHCP、路由通告和网络引导等基础设施。([源码](https://thekelleys.org.uk/gitweb/?p=dnsmasq.git;a=tree)) `GPL-2.0` `C`
- [Knot](https://www.knot-dns.cz/) - 高性能权威 DNS 服务器。([源码](https://gitlab.nic.cz/knot/knot-dns)) `GPL-3.0` `C`
- [NSD](https://www.nlnetlabs.nl/projects/nsd/about/) - 以速度、可靠性、稳定性和安全性为目标开发的权威 DNS 名称服务器。([源码](https://github.com/NLnetLabs/nsd)) `BSD-3-Clause` `C`
- [PowerDNS Authoritative Server](https://doc.powerdns.com/authoritative/) - 支持多种后端的多功能名称服务器。([源码](https://github.com/PowerDNS/pdns)) `GPL-2.0` `C++`
- [Unbound](https://nlnetlabs.nl/projects/unbound/about/) - 支持验证、递归和缓存的 DNS 解析器。([源码](https://github.com/NLnetLabs/unbound)) `BSD-3-Clause` `C`
- [Yadifa](https://www.yadifa.eu/) - 由 .eu 从零开发，简洁、小巧、轻量且符合 RFC 的名称服务器实现。([源码](https://github.com/yadifa/yadifa)) `BSD-3-Clause` `C`


### 编辑器

**[`^        返回顶部        ^`](#awesome-sysadmin)**

开源代码编辑器。

- [Atom Community](https://github.com/atom-community/atom) - [atom](https://github.com/atom/atom) 的分支，来自 Github 的可定制文本编辑器。`MIT` `JavaScript`
- [Brackets](https://brackets.io/) - 面向网页设计师和前端开发者的代码编辑器。([源码](https://github.com/brackets-cont/brackets)) `MIT` `JavaScript`
- [Eclipse](https://www.eclipse.org/) - 用 Java 编写、可扩展插件系统的 IDE。([源码](https://git.eclipse.org/c/)) `EPL-1.0` `Java`
- [Geany](https://www.geany.org/) - 基于 GTK2 的文本编辑器。([源码](https://github.com/geany/geany)) `GPL-2.0` `C/C++`
- [GNU Emacs](https://www.gnu.org/software/emacs/) - 可扩展、可定制的文本编辑器及更多功能。([源码](https://github.com/emacs-mirror/emacs)) `GPL-3.0` `C`
- [Haroopad](http://pad.haroopress.com/) - 支持实时预览的 Markdown 编辑器。([源码](https://github.com/rhiokim/haroopad)) `GPL-3.0` `JavaScript`
- [jotgit](https://github.com/jdleesmiller/jotgit) - 基于 Git 的实时协作代码编辑。`MIT` `Nodejs`
- [KDevelop](https://www.kdevelop.org/) - KDE 团队开发的 IDE。([源码](https://invent.kde.org/kdevelop/kdevelop)) `GFDL-1.2` `C++`
- [Micro](https://micro-editor.github.io/) - 现代直观的终端文本编辑器。([源码](https://github.com/zyedidia/micro)) `MIT` `Go`
- [Nano](https://nano-editor.org) - 易用、可定制的文本编辑器。([源码](https://git.savannah.gnu.org/cgit/nano.git/tree/)) `GPL-3.0` `C`
- [Notepad++](https://notepad-plus-plus.org/) - GPLv2 多语言编辑器，支持 Windows 语法高亮。([源码](https://github.com/notepad-plus-plus/notepad-plus-plus)) `GPL-2.0` `C++`
- [TextMate](https://macromates.com/) - OS X 图形化文本编辑器。([源码](https://github.com/textmate/textmate/)) `GPL-3.0` `C++`
- [Vim](https://www.vim.org) - 高度可配置的文本编辑器，提升编辑效率。([源码](https://github.com/vim/vim)) `Vim` `C`
- [VSCodium](https://vscodium.com/) - 基于 [微软 VS Code](https://code.visualstudio.com/) 的开源跨平台可扩展代码编辑器，去除了非自由部分。([源码](https://github.com/VSCodium/vscodium)) `MIT` `TypeScript`


### 身份管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[身份管理](https://en.wikipedia.org/wiki/Identity_management)（IdM），也称为身份与访问管理（IAM 或 IdAM），是一套政策和技术框架，确保生态系统内或与企业连接的正确用户拥有对技术资源的适当访问权限。

**请访问 [身份管理 - LDAP](#identity-management---ldap)、[身份管理 - 工具与 Web 界面](#identity-management---tools-and-web-interfaces)、[身份管理 - 单点登录 SSO](#identity-management---single-sign-on-sso)**



### 身份管理 - LDAP

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[轻量级目录访问协议（LDAP）](https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol) 是一种开放、中立、行业标准的应用协议，用于通过 IP 网络访问和维护分布式目录信息服务。

- [389 Directory Server](https://www.port389.org/) - 企业级开源 LDAP 服务器，适用于 Linux。([源码](https://github.com/389ds/389-ds-base)) `GPL-3.0` `C`
- [Apache Directory Server](https://directory.apache.org/apacheds/) - 可扩展、可嵌入的目录服务器，兼容 LDAPv3，支持 Kerberos 5、变更密码协议、触发器、存储过程、队列和视图。([源码](https://github.com/apache/directory-server)) `Apache-2.0` `Java`
- [FreeIPA](https://www.freeipa.org/) - 集成安全信息管理解决方案，结合 Linux（Fedora）、389 Directory Server、Kerberos、NTP、DNS 和 Dogtag 证书系统（Web 界面和命令行管理工具）。([源码](https://pagure.io/freeipa)) `GPL-3.0` `Python/C/JavaScript`
- [FreeRADIUS](https://freeradius.org/) - 多协议策略服务器（radiusd），实现 RADIUS、DHCP、BFD 和 ARP 及相关客户端/PAM 库/Apache 模块。([源码](https://github.com/FreeRADIUS/freeradius-server)) `GPL-2.0` `C`
- [lldap](https://github.com/nitnelave/lldap) - 轻量级（简化版）LDAP 实现，带有简单直观的 Web 界面和 GraphQL 支持。`GPL-3.0` `Rust`
- [OpenLDAP](https://www.openldap.org/) - 轻量级目录访问协议的开源实现（服务器、库和客户端）。([源码](https://git.openldap.org/openldap/openldap)) `OLDAP-2.8` `C`


### 身份管理 - 单点登录（SSO）

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[单点登录（SSO）](https://en.wikipedia.org/wiki/Single_sign-on) 是一种认证方案，允许用户使用单一身份登录多个相关但独立的软件系统。

- [Authelia](https://www.authelia.com/) - Web 应用的单点登录多因素门户。([源码](https://github.com/authelia/authelia)) `Apache-2.0` `Go`
- [Authentik](https://goauthentik.io/) - 灵活的身份提供者，支持多种协议（OAuth 2.0、SAML、LDAP 和 Radius）。([源码](https://github.com/goauthentik/authentik)) `MIT` `Python`
- [KeyCloak](https://www.keycloak.org) - 开源身份与访问管理。([源码](https://github.com/keycloak/keycloak)) `Apache-2.0` `Java`


### 身份管理 - 工具与 Web 界面

**[`^        返回顶部        ^`](#awesome-sysadmin)**

身份管理系统的各种工具和 Web 界面。

- [BounCA](https://bounca.org/) - 个人 SSL 密钥/证书颁发机构 Web 工具，用于创建自签名证书。([源码](https://gitlab.com/bounca/bounca/)) `Apache-2.0` `Python`
- [easy-rsa](https://github.com/OpenVPN/easy-rsa) - 用于构建和管理 PKI CA 的 Bash 脚本。`GPL-2.0` `Shell`
- [Fusion Directory](https://www.fusiondirectory.org) - 基于 OpenLDAP 的企业目录和服务管理。([源码](https://github.com/fusiondirectory/fusiondirectory)) `GPL-2.0` `PHP`
- [LDAP Account Manager (LAM)](https://www.ldap-account-manager.org/lamcms/) - 用于管理 LDAP 目录中条目（如用户、组、DHCP 设置）的 Web 前端。([源码](https://github.com/LDAPAccountManager/lam/)) `GPL-3.0` `PHP`
- [Libravatar](https://www.libravatar.org/) - 向其他网站分发头像（个人资料图片）的服务。([源码](https://git.linux-kernel.at/oliver/ivatar/)) `AGPL-3.0` `Python`
- [Pomerium](https://www.pomerium.io/) - 受 BeyondCorp 启发的身份与上下文感知访问代理。([源码](https://github.com/pomerium/pomerium)) `Apache-2.0` `Docker/Go`
- [Samba](https://www.samba.org/) - Active Directory 和 CIFS 协议实现。([源码](https://download.samba.org/pub/samba/)) `GPL-3.0` `C`
- [Smallstep Certificates](https://smallstep.com/certificates/) - 私有证书颁发机构（X.509 & SSH）及相关自动化证书管理工具。([源码](https://github.com/smallstep/certificates)) `Apache-2.0` `Go`
- [ZITADEL](https://zitadel.com/) - 云原生身份与访问管理解决方案，提供安全认证、授权和身份管理平台。([源码](https://github.com/zitadel/zitadel)) `Apache-2.0` `Go/Docker/K8S`


### IT 资产管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

IT [资产管理](https://en.wikipedia.org/wiki/Asset_management) 软件。

- [GLPI](https://www.glpi-project.org/) - 信息资源管理器，带有额外的管理界面。([源码](https://github.com/glpi-project/glpi)) `GPL-3.0` `PHP`
- [OCS Inventory NG](https://ocsinventory-ng.org/) - 适用于 IT 部门所有设备的资产管理与部署解决方案。([源码](https://github.com/OCSInventory-NG)) `GPL-2.0` `PHP/Perl`
- [OPSI](https://www.opsi.org) - Linux 和 Windows 的硬件/软件清单、客户端管理、部署和补丁。([源码](https://github.com/opsi-org/)) `GPL-3.0/AGPL-3.0` `OVF/Python`
- [RackTables](https://racktables.org/) - 数据中心和机房资产管理，如硬件资产、网络地址、机架空间、网络配置等文档化。([演示](https://www.racktables.org/demo.php), [源码](https://github.com/RackTables/racktables)) `GPL-2.0` `PHP`
- [Ralph](https://ralph.allegro.tech/) - 适用于大型数据中心和小型局域网的资产管理、DCIM 和 CMDB 系统。([演示](https://github.com/allegro/ralph#live-demo), [源码](https://github.com/allegro/ralph)) `Apache-2.0` `Python/Docker`
- [Snipe IT](https://snipeitapp.com/) - 资产与许可证管理软件。([源码](https://github.com/snipe/snipe-it)) `AGPL-3.0` `PHP`


### 日志管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

日志管理工具：收集、解析、可视化等。

- [Fluentd](https://www.fluentd.org/) - 统一日志层的数据收集器。([源码](https://github.com/fluent/fluentd)) `Apache-2.0` `Ruby`
- [Flume](https://flume.apache.org/) - 高效收集、聚合和传输大量日志数据的分布式、可靠服务。([源码](https://github.com/apache/flume)) `Apache-2.0` `Java`
- [GoAccess](https://goaccess.io/) - 实时 Web 日志分析器和交互式查看器，可在终端或浏览器中运行。([源码](https://github.com/allinurl/goaccess)) `MIT` `C`
- [Loki](https://grafana.com/oss/loki/) - 日志聚合系统，设计用于存储和查询所有应用和基础设施的日志。([源码](https://github.com/grafana/loki)) `AGPL-3.0` `Go`
- [rsyslog](https://www.rsyslog.com/) - 超快的日志处理系统。([源码](https://github.com/rsyslog/rsyslog)) `GPL-3.0` `C`


### 邮件客户端

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[邮件客户端](https://en.wikipedia.org/wiki/Email_client)，又称邮件阅读器或消息用户代理（MUA），是用于访问和管理用户电子邮件的计算机程序。

- [aerc](https://aerc-mail.org/) - 以纯文本和开发者功能为重点的终端邮件客户端。([源码](https://git.sr.ht/~rjarry/aerc)) `MIT` `Go`
- [Claws Mail](http://www.claws-mail.org/) - 基于 GTK+ 的老牌邮件客户端（及新闻阅读器）。([源码](https://git.claws-mail.org/?p=claws.git;a=tree)) `GPL-3.0` `C`
- [ImapSync](http://imapsync.lamiral.info/) - 简单的 IMAP 邮箱迁移工具，可将邮箱复制到其他服务器。([源码](https://github.com/imapsync/imapsync)) `NLPL` `Perl`
- [Mutt](http://www.mutt.org/) - 小巧但功能强大的文本邮件客户端。([源码](https://gitlab.com/muttmua/mutt)) `GPL-2.0` `C`
- [Sylpheed](https://sylpheed.sraoss.jp/en/) - Claws Mail 的前身，仍在开发的轻量级邮件客户端。([源码](https://github.com/sylpheed-mail/sylpheed)) `GPL-2.0` `C`
- [Thunderbird](https://www.thunderbird.net/) - 免费、易于设置和自定义的邮件应用。([源码](https://hg.mozilla.org/comm-central/file)) `MPL-2.0` `C/C++`


### 指标与指标采集

**[`^        返回顶部        ^`](#awesome-sysadmin)**

指标采集与展示软件。

_相关：[数据库](#databases)、[监控](#monitoring)_

- [Beats](https://www.elastic.co/beats/) - 单一用途的数据收集器，将数据从数百或数千台机器发送到 Logstash 或 Elasticsearch。([源码](https://github.com/elastic/beats)) `Apache-2.0` `Go`
- [Collectd](https://collectd.org/) - 系统统计信息收集守护进程。([源码](https://github.com/collectd/collectd)) `MIT` `C`
- [Diamond](https://github.com/python-diamond/Diamond) - 收集系统指标并发布到 Graphite（及其他）的守护进程。`MIT` `Python`
- [Grafana](https://grafana.com/) - Graphite 和 InfluxDB 的仪表盘与图形编辑器。([源码](https://github.com/grafana/grafana)) `AGPL-3.0` `Go`
- [Graphite](https://graphite.readthedocs.org/en/latest/) - 可扩展的图形服务器。([源码](https://github.com/graphite-project/graphite-web)) `Apache-2.0` `Python`
- [RRDtool](https://oss.oetiker.ch/rrdtool/) - 行业标准、高性能的时间序列数据记录与绘图系统。([源码](https://github.com/oetiker/rrdtool-1.x)) `GPL-2.0` `C`
- [Statsd](https://github.com/etsy/statsd/) - 监听计数器、定时器等统计信息的守护进程，通过 UDP 或 TCP 接收并聚合后发送到后端服务。`MIT` `Nodejs`
- [tcollector](http://opentsdb.net/docs/build/html/user_guide/utilities/tcollector.html) - 从本地采集器收集数据并推送到 OpenTSDB。([源码](https://github.com/OpenTSDB/tcollector/)) `LGPL-3.0/GPL-3.0` `Python`
- [Telegraf](https://github.com/influxdata/telegraf) - 插件驱动的服务器代理，用于采集、处理、聚合和写入指标。`MIT` `Go`


### 杂项

**[`^        返回顶部        ^`](#awesome-sysadmin)**

未归入其他分类的软件。

- [Chocolatey](https://chocolatey.org/) - Windows 的包管理器。([源码](https://github.com/chocolatey/choco)) `Apache-2.0` `C#/PowerShell`
- [Clonezilla](https://clonezilla.org/) - 分区和磁盘镜像/克隆程序。([源码](https://clonezilla.org/downloads/src/)) `GPL-2.0` `Perl/Shell/Other`
- [DadaMail](https://dadamailproject.com/) - 用 Perl 编写的邮件列表管理器。([源码](https://sourceforge.net/projects/dadamail/files/)) `GPL-2.0` `Perl`
- [Fog](https://www.fogproject.org/) - 克隆/镜像解决方案与救援套件。([源码](https://github.com/FOGProject/fogproject)) `GPL-3.0` `PHP/Shell`
- [phpList](https://www.phplist.org/) - 邮件通讯与邮件营销软件。([源码](https://github.com/phpList/phplist3)) `AGPL-3.0` `PHP`


### 监控

**[`^        返回顶部        ^`](#awesome-sysadmin)**

监控软件。

_相关：[指标与指标采集](#metrics--metric-collection)_

- [Adagios](http://adagios.org/) - 基于 Web 的 Nagios 配置与监控界面（替代标准界面），并提供 REST 接口。([源码](https://github.com/opinkerfi/adagios)) `AGPL-3.0` `Docker/Python`
- [Alerta](https://alerta.io/) - 分布式、可扩展且灵活的监控系统。([源码](https://github.com/alerta/alerta)) `Apache-2.0` `Python`
- [Beszel](https://beszel.dev/) - 轻量级服务器监控平台，支持 Docker 统计、历史数据和告警功能。([源码](https://github.com/henrygd/beszel)) `MIT` `Go`
- [Bloonix](https://bloonix-monitoring.org/) - 监控解决方案，帮助企业保障高可用性和性能。([源码](https://github.com/bloonix)) `GPL-3.0` `Perl`
- [Cacti](https://www.cacti.net) - 基于 Web 的网络监控与绘图工具。([源码](https://github.com/Cacti/cacti)) `GPL-2.0` `PHP`
- [cadvisor](https://github.com/google/cadvisor) - 分析运行中容器的资源使用和性能特征。`Apache-2.0` `Go`
- [checkmk](https://checkmk.com/) - 应用、服务器和网络的综合监控解决方案。([源码](https://github.com/Checkmk/checkmk)) `GPL-2.0` `Python/PHP`
- [dashdot](https://github.com/MauriceNino/dashdot) - 面向小型私有服务器的简单现代服务器仪表盘。([演示](https://dash.mauz.dev/)) `MIT` `Nodejs/Docker`
- [EdMon](https://github.com/Edraens/EdMon) - 命令行监控应用，帮助检查主机和服务可用性，支持通知。`MIT` `Java`
- [eZ Server Monitor](https://www.ezservermonitor.com) - 轻量级简单的 Linux 仪表盘监控，提供 Web 和 Bash 应用。([源码](https://github.com/shevabam/ezservermonitor-web)) `GPL-3.0` `PHP/Shell`
- [glances](https://nicolargo.github.io/glances/) - 开源、跨平台的实时监控工具，支持 CLI 和 Web 仪表盘，多种导出选项。([源码](https://github.com/nicolargo/glances)) `GPL-3.0` `Python`
- [Healthchecks](https://healthchecks.io/docs/self_hosted/) - 针对定时任务、后台服务和计划任务的监控。([源码](https://github.com/healthchecks/healthchecks)) `BSD-3-Clause` `Python`
- [Icinga](https://www.icinga.com/) - Nagios 分支，功能已超越原版，支持集群监控。([源码](https://github.com/Icinga/icinga2)) `GPL-2.0` `C++`
- [LibreNMS](https://www.librenms.org) - 功能丰富的网络监控系统，支持多种设备。([源码](https://github.com/librenms/librenms)) `GPL-3.0` `PHP`
- [Linux Dash](https://github.com/afaqurk/linux-dash) - 针对 GNU/Linux 机器的低开销 Web 监控仪表盘。`MIT` `Nodejs/Go/Python/PHP`
- [Monit](https://mmonit.com/monit/#home) - 管理和监控 Unix 系统的小工具。([源码](https://bitbucket.org/tildeslash/monit/src/master/)) `AGPL-3.0` `C`
- [Munin](https://munin-monitoring.org/) - 网络资源监控工具。([源码](https://github.com/munin-monitoring/munin)) `GPL-2.0` `Perl/Shell`
- [Naemon](https://www.naemon.org/) - 基于 Nagios 4 内核的网络监控工具，性能增强并有新特性。([源码](https://github.com/naemon/naemon-core)) `GPL-2.0` `C`
- [Nagios](https://www.nagios.org/) - 计算机系统、网络和基础设施监控软件。([源码](https://github.com/NagiosEnterprises/nagioscore)) `GPL-2.0` `C`
- [Netdata](https://www.netdata.cloud/) - 分布式、实时的系统与应用性能健康监控，支持 Linux、FreeBSD 和 MacOS。([源码](https://github.com/netdata/netdata)) `GPL-3.0` `C`
- [NetXMS](https://www.netxms.org/) - 开源网络与基础设施监控和管理。([源码](https://github.com/netxms/netxms)) `LGPL-3.0/GPL-3.0` `Java/C++/C`
- [Observium Community Edition](http://www.observium.org/) - 网络监控与管理平台，提供实时网络健康与性能洞察。`QPL-1.0` `PHP`
- [openITCOCKPIT Community Edition](https://openitcockpit.io/) - 监控套件，支持与 Naemon、Checkmk、Grafana 等无缝集成。([演示](https://demo.openitcockpit.io/), [源码](https://github.com/it-novum/openITCOCKPIT)) `GPL-3.0` `deb/Docker`
- [Performance Co-Pilot](http://pcp.io) - 轻量级、分布式系统性能分析框架。([源码](https://github.com/performancecopilot/pcp)) `LGPL-2.1/GPL-2.0` `C`
- [PHP Server Monitor](https://www.phpservermonitor.org/) - 开源服务器和网站监控工具。([源码](https://github.com/phpservermon/phpservermon)) `GPL-3.0` `PHP`
- [PhpSysInfo](https://phpsysinfo.github.io/phpsysinfo/) - 可自定义的 PHP 脚本，优雅展示系统信息。([源码](https://github.com/phpsysinfo/phpsysinfo)) `GPL-2.0` `PHP`
- [Prometheus](https://prometheus.io/) - 服务监控系统与时序数据库。([源码](https://github.com/prometheus/prometheus)) `Apache-2.0` `Go`
- [Riemann](https://riemann.io/) - 灵活快速的事件处理器，支持复杂事件/指标分析。([源码](https://github.com/riemann/riemann)) `EPL-1.0` `Java`
- [rtop](https://github.com/rapidloop/rtop) - 基于 SSH 的交互式远程系统监控工具。`MIT` `Go`
- [ruptime](https://github.com/alexmyczko/ruptime) - 经典系统状态服务器。`AGPL-3.0` `Shell`
- [Scrutiny](https://github.com/AnalogJ/scrutiny) - 硬盘 S.M.A.R.T 监控 Web UI，支持历史趋势与真实故障阈值。`MIT` `Go`
- [Sensu](https://sensu.io/) - 针对弹性基础设施和分布式应用的监控工具。([源码](https://github.com/sensu/sensu-go)) `MIT` `Go`
- [Status](https://github.com/dani3l0/Status) - 适合小型家庭服务器的简单轻量系统监控工具，带美观 Web 界面。([演示](https://status.enshittification.social/)) `MIT` `Python`
- [Thruk](https://www.thruk.org/) - 多后端监控 Web 界面，支持 Naemon、Nagios、Icinga 和 Shinken。([源码](https://github.com/sni/Thruk)) `GPL-1.0` `Perl`
- [Wazuh](https://wazuh.com/) - 统一 XDR 与 SIEM，保护终端和云工作负载。([源码](https://github.com/wazuh/wazuh)) `GPL-2.0` `C`
- [Zabbix](https://www.zabbix.com/) - 企业级网络与应用监控软件。([源码](https://git.zabbix.com/projects/ZBX/repos/zabbix/browse)) `GPL-2.0` `C`


### 打包

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[包管理器](https://en.wikipedia.org/wiki/Package_manager)或包管理系统是一组自动化安装、升级、配置和卸载计算机程序的软件工具，以一致的方式管理计算机上的软件。

- [aptly](https://www.aptly.info/) - Debian 仓库管理的瑞士军刀。([源码](https://github.com/aptly-dev/aptly)) `MIT` `Go`
- [fpm](https://fpm.readthedocs.io/en/latest/) - 多格式通用包创建工具。([源码](https://github.com/jordansissel/fpm)) `MIT` `Ruby`
- [omnibus-ruby](https://github.com/chef/omnibus) - 跨平台轻松为项目创建全栈安装包。`Apache-2.0` `Ruby`
- [tito](https://github.com/dgoodwin/tito) - 为基于 git 的项目构建 RPM 包。`GPL-2.0` `Python`


### 项目管理

**[`^        返回顶部        ^`](#awesome-sysadmin)**

基于 Web 的项目管理和缺陷跟踪系统。

**请访问 [awesome-selfhosted/Project Management](https://awesome-selfhosted.net/tags/software-development---project-management.html)**



### 队列

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[消息队列](https://en.wikipedia.org/wiki/Message_queue)和[消息中间件](https://en.wikipedia.org/wiki/Message_broker)软件，通常用于进程间通信（IPC）或同一进程内线程间通信。

_另见：[Cloud Native Landscape - Streaming & Messaging](https://landscape.cncf.io/?group=projects-and-products&view-mode=card#app-definition-and-development--streaming-messaging)_

- [ActiveMQ](https://activemq.apache.org/) - Java 消息中间件。([源码](https://github.com/apache/activemq)) `Apache-2.0` `Java`
- [BeanstalkD](https://beanstalkd.github.io/) - 简单快速的工作队列。([源码](https://github.com/beanstalkd/beanstalkd)) `MIT` `C`
- [Gearman](http://gearman.org/) - 快速多语言队列/作业处理平台。([源码](https://github.com/gearman/gearmand)) `BSD-3-Clause` `C++`
- [NSQ](https://nsq.io/) - 实时分布式消息平台。([源码](https://github.com/nsqio/nsq)) `MPL-2.0` `Go`
- [ZeroMQ](https://zeromq.org/) - 轻量级队列系统。([源码](https://github.com/zeromq)) `GPL-3.0` `C++`


### 远程桌面客户端

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[远程桌面](https://en.wikipedia.org/wiki/Remote_desktop_software)客户端软件。

_另见：[awesome-selfhosted/Remote Access](https://awesome-selfhosted.net/tags/remote-access.html)_

- [Remmina](https://www.remmina.org/) - 功能丰富的 Linux 及类 Unix 远程桌面应用。([源码](https://gitlab.com/Remmina/Remmina)) `GPL-2.0` `C`
- [Tiger VNC](https://tigervnc.org/) - 高性能多平台 VNC 客户端和服务器。([源码](https://github.com/TigerVNC/tigervnc)) `GPL-2.0` `C++`
- [X2go](https://wiki.x2go.org/doku.php) - 基于 NoMachine/NX 协议的 Linux 远程桌面软件。([源码](https://code.x2go.org/gitweb)) `GPL-2.0` `Perl`


### 路由器

**[`^        返回顶部        ^`](#awesome-sysadmin)**

用于管理[路由器](https://en.wikipedia.org/wiki/Router_(computing))硬件的软件。

- [DD-WRT](https://dd-wrt.com/) - 基于 Linux 的无线路由器和接入点固件，最初为 Linksys WRT54G 设计。([源码](https://svn.dd-wrt.com/)) `GPL-2.0` `C`
- [OpenWrt](https://openwrt.org/) - 基于 Linux 的路由器，支持 Mesh 网络、Snort IPS、AQM 等多种功能。([源码](https://git.openwrt.org/openwrt/openwrt.git)) `GPL-2.0` `C`
- [OPNsense](https://opnsense.org/) - 基于 FreeBSD 的开源防火墙和路由器，支持流量整形、负载均衡和 VPN。([源码](https://github.com/opnsense)) `BSD-2-Clause` `C/PHP`
- [pfSense CE](https://www.pfsense.org/) - 基于 FreeBSD 的免费网络防火墙发行版，内核定制并集成第三方自由软件包。([源码](https://github.com/pfsense/pfsense)) `Apache-2.0` `Shell/PHP/Other`


### 服务发现

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[服务发现](https://en.wikipedia.org/wiki/Service_discovery) 是指在计算机网络中自动检测设备和服务的过程。

- [Consul](https://www.consul.io/) - Consul 是一个用于服务发现、监控和配置的工具。([源码](https://github.com/hashicorp/consul)) `MPL-2.0` `Go`
- [etcd](https://etcd.io/) - 分布式 K/V 存储，通过 SSL PKI 认证和 REST HTTP API 提供共享配置与服务发现。([源码](https://github.com/coreos/etcd)) `Apache-2.0` `Go`
- [ZooKeeper](https://zookeeper.apache.org/) - ZooKeeper 是一个集中式服务，用于维护配置信息、命名、分布式同步和组服务。([源码](https://github.com/apache/zookeeper)) `Apache-2.0` `Java/C++`


### 软件容器

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[操作系统级](https://en.wikipedia.org/wiki/OS-level_virtualization)虚拟化。

- [Docker Compose](https://docs.docker.com/compose/) - 定义和运行多容器 Docker 应用。([源码](https://github.com/docker/compose)) `Apache-2.0` `Go`
- [Docker Swarm](https://docs.docker.com/engine/swarm/) - 管理 Docker 引擎集群。([源码](https://github.com/moby/swarmkit)) `Apache-2.0` `Go`
- [Docker](https://www.docker.com/) - 为开发者和系统管理员构建、发布和运行分布式应用的平台。([源码](https://www.docker.com/community/open-source/)) `Apache-2.0` `Go`
- [LXC](https://linuxcontainers.org/lxc/) - Linux 内核容器特性的用户空间接口。([源码](https://github.com/lxc/lxc)) `GPL-2.0` `C`
- [LXD](https://linuxcontainers.org/lxd/) - 容器“管理器”，为 LXC 提供更好的用户体验。([源码](https://github.com/lxc/lxd)) `Apache-2.0` `Go`
- [OpenVZ](https://openvz.org) - Linux 的基于容器的虚拟化。([源码](https://src.openvz.org/projects/OVZ)) `GPL-2.0` `C`
- [Podman](https://podman.io) - 无守护进程的容器引擎，支持以 root 或 rootless 模式运行。可直接 `alias docker=podman`。([源码](https://github.com/containers/podman)) `Apache-2.0` `Go`
- [Portainer Community Edition](https://www.portainer.io/) - 简单易用的 Docker 管理界面。([源码](https://github.com/portainer/portainer)) `Zlib` `Go`
- [systemd-nspawn](https://www.freedesktop.org/software/systemd/man/systemd-nspawn.html) - 轻量级、类似 chroot 的环境，可直接在 systemd 下运行操作系统或命令。([源码](https://github.com/systemd/systemd)) `GPL-2.0` `C`


### 状态页

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[运行时间](https://en.wikipedia.org/wiki/Uptime)是衡量系统可靠性的指标，通常以机器可用时间的百分比表示。

**请访问 [awesome-selfhosted/Status / Uptime Pages](https://awesome-selfhosted.net/tags/status--uptime-pages.html)**


### 故障排查

**[`^        返回顶部        ^`](#awesome-sysadmin)**

故障排查工具。

- [grml](https://grml.org) - 含强大 CLI 工具的可启动 Debian Live CD。([源码](https://github.com/grml/)) `GPL-3.0` `Shell`
- [mitmproxy](https://mitmproxy.org/) - 用于拦截、查看和修改网络流量的 Python 工具，排查网络问题非常有用。([源码](https://github.com/mitmproxy/mitmproxy)) `MIT` `Python`
- [mtr](https://www.bitwizard.nl/mtr/) - 集合 traceroute 和 ping 的网络工具。([源码](https://github.com/traviscross/mtr)) `GPL-2.0` `C`
- [Sysdig](https://www.sysdig.com/) - 捕获 Linux 实例的系统状态和活动，并进行保存、过滤和分析。([源码](https://github.com/draios/sysdig)) `Apache-2.0` `Docker/Lua/C`
- [Wireshark](https://www.wireshark.org/) - 世界领先的网络协议分析器。([源码](https://gitlab.com/wireshark/wireshark)) `GPL-2.0` `C`


### 版本控制

**[`^        返回顶部        ^`](#awesome-sysadmin)**

软件版本管理与修订控制。

- [Darcs](https://darcs.net/) - 跨平台版本控制系统，类似 git、mercurial 或 svn，但采用完全不同的思路：关注变更而非快照。（[源码](https://darcs.net/releases/)）`GPL-2.0` `Haskell`
- [Fossil](https://www.fossil-scm.org/) - 分布式版本控制，内置 Wiki 和缺陷跟踪。（[源码](https://www.fossil-scm.org/home/dir?ci=trunk)）`BSD-2-Clause` `C`
- [Git](https://git-scm.com/) - 分布式修订控制和源码管理（SCM），强调速度。（[源码](https://github.com/git/git)）`GPL-2.0` `C`
- [Mercurial](https://www.mercurial-scm.org/) - 分布式源码控制管理工具。（[源码](https://repo.mercurial-scm.org/hg/file/tip)）`GPL-2.0` `Python/C/Rust`
- [Subversion](https://subversion.apache.org/) - 客户端-服务器修订控制系统。（[源码](https://svn.apache.org/repos/asf/subversion/trunk/)）`Apache-2.0` `C`


### 虚拟化

**[`^        返回顶部        ^`](#awesome-sysadmin)**

虚拟化软件。

- [Ganeti](https://www.ganeti.org/) - 基于 KVM 和 Xen 的集群虚拟服务器管理工具。（[源码](https://github.com/ganeti/ganeti)）`BSD-2-Clause` `Python/Haskell`
- [KVM](https://www.linux-kvm.org) - Linux 内核虚拟化基础设施。（[源码](https://git.kernel.org/pub/scm/virt/kvm/kvm.git/)）`GPL-2.0/LGPL-2.0` `C`
- [OpenNebula](https://opennebula.org/) - 构建和管理企业云，支持虚拟化服务、容器化应用和无服务器计算。（[源码](https://github.com/OpenNebula/one)）`Apache-2.0` `C++`
- [oVirt](https://www.ovirt.org/) - 管理虚拟机、存储和虚拟网络。（[源码](https://github.com/oVirt)）`Apache-2.0` `Java`
- [Packer](https://www.packer.io/) - 从单一源配置为多平台创建一致的机器镜像的工具。（[源码](https://github.com/hashicorp/packer)）`MPL-2.0` `Go`
- [Proxmox VE](https://www.proxmox.com/proxmox-ve) - 虚拟化管理解决方案。（[源码](https://git.proxmox.com/)）`GPL-2.0` `Perl/Shell`
- [QEMU](https://www.qemu.org/) - 通用机器模拟器和虚拟化器。（[源码](https://gitlab.com/qemu-project/qemu)）`LGPL-2.1` `C`
- [Vagrant](https://www.vagrantup.com/) - 构建完整开发环境的工具。（[源码](https://github.com/hashicorp/vagrant)）`BUSL-1.1` `Ruby`
- [VirtualBox](https://www.virtualbox.org/) - Oracle 公司出品的虚拟化产品。（[源码](https://www.virtualbox.org/browser/vbox)）`GPL-3.0/CDDL-1.0` `C++`
- [XCP-ng](https://www.xcp-ng.org/) - 基于 Xen Source 和 Citrix® Hypervisor（前 XenServer）的虚拟化平台。（[源码](https://github.com/xcp-ng)）`GPL-2.0` `C`
- [Xen](https://www.xenproject.org/) - 适用于 32/64 位 Intel / AMD（IA 64）和 PowerPC 970 架构的虚拟机监控器。（[源码](https://xenbits.xenproject.org/gitweb/?p=xen.git;a=tree;hb=HEAD)）`GPL-2.0` `C`


### VPN

**[`^        返回顶部        ^`](#awesome-sysadmin)**

VPN 软件。

- [DefGuard](https://defguard.net/) - 真正的企业级 WireGuard，支持 MFA/2FA 和 SSO。（[源码](https://github.com/DefGuard)）`Apache-2.0` `Rust`
- [Dockovpn](https://dockovpn.io) - 即开即用的无状态 Docker 化 OpenVPN 服务器，启动时间小于 2 秒。（[源码](https://github.com/dockovpn/dockovpn)）`GPL-2.0` `Docker`
- [Firezone](https://www.firezone.dev/) - 基于 WireGuard 的 VPN 服务器和防火墙。（[源码](https://github.com/firezone/firezone)）`Apache-2.0` `Docker`
- [Gluetun VPN client](https://github.com/qdm12/gluetun) - 多 VPN 提供商的 Docker VPN 客户端，支持 OpenVPN/WireGuard、DNS over TLS，内置代理。（`MIT` `docker`）
- [Headscale](https://github.com/juanfont/headscale) - [Tailscale](https://tailscale.com) 的自托管分支，跨平台客户端，易用，内置（实验性）监控工具。`BSD-3-Clause` `Go`
- [Nebula](https://github.com/slackhq/nebula) - 注重性能、简洁和安全的可扩展 P2P VPN。`MIT` `Go`
- [ocserv](https://www.infradead.org/ocserv/) - 兼容 Cisco AnyConnect 的 VPN 服务器。（[源码](https://gitlab.com/ocserv/ocserv)）`GPL-2.0` `C`
- [OpenVPN](https://community.openvpn.net) - 使用 SSL/TLS 进行密钥交换的自定义安全协议。（[源码](https://github.com/OpenVPN/openvpn)）`GPL-2.0` `C`
- [SoftEther](https://www.softether.org/) - 多协议软件 VPN，功能强大。（[源码](https://github.com/SoftEtherVPN/SoftEtherVPN/)）`Apache-2.0` `C`
- [sshuttle](https://github.com/sshuttle/sshuttle) - “穷人版”VPN。`LGPL-2.1` `Python`
- [strongSwan](https://www.strongswan.org/) - Linux 下完整的 IPsec 实现。（[源码](https://github.com/strongswan/strongswan)）`GPL-2.0` `C`
- [WireGuard](https://www.wireguard.com/) - 基于椭圆曲线和公钥加密的高速 VPN。（[源码](https://www.wireguard.com/repositories/)）`GPL-2.0` `C`


### Web

**[`^        返回顶部        ^`](#awesome-sysadmin)**

[Web 服务器](https://en.wikipedia.org/wiki/Web_server)与[反向代理](https://en.wikipedia.org/wiki/Reverse_proxy)。

**请访问 [awesome-selfhosted/Web Servers](https://awesome-selfhosted.net/tags/web-servers.html)**


--------------------

## 许可证列表

**[`^        返回顶部        ^`](#awesome-sysadmin)**

- `AGPL-3.0` - [GNU Affero General Public License 3.0](https://spdx.org/licenses/AGPL-3.0.html)
- `Apache-2.0` - [Apache, Version 2.0](https://spdx.org/licenses/Apache-2.0.html)
- `BSD-2-Clause` - [BSD 2-clause "Simplified"](https://spdx.org/licenses/BSD-2-Clause.html)
- `BSD-3-Clause` - [BSD 3-Clause "New" or "Revised"](https://spdx.org/licenses/BSD-3-Clause.html)
- `BUSL-1.1` - [Business Source License 1.1](https://spdx.org/licenses/BUSL-1.1.html)
- `CC0-1.0` - [Public Domain/Creative Common Zero 1.0](https://spdx.org/licenses/CC0-1.0.html)
- `CDDL-1.0` - [Common Development and Distribution License 1.0](https://spdx.org/licenses/CDDL-1.0.html)
- `EPL-1.0` - [Eclipse Public License 1.0](https://spdx.org/licenses/EPL-1.0.html)
- `GFDL-1.2` - [GNU Free Documentation License 1.2](https://spdx.org/licenses/GFDL-1.2.html)
- `GPL-1.0` - [GNU General Public License 1.0](https://spdx.org/licenses/GPL-1.0.html)
- `GPL-2.0` - [GNU General Public License 2.0](https://spdx.org/licenses/GPL-2.0.html)
- `GPL-3.0` - [GNU General Public License 3.0](https://spdx.org/licenses/GPL-3.0.html)
- `IPL-1.0` - [IBM Public License v1.0](https://spdx.org/licenses/IPL-1.0.html)
- `ISC` - [ISC License](https://spdx.org/licenses/ISC.html)
- `LGPL-2.0` - [GNU Lesser General Public License v2](https://spdx.org/licenses/LGPL-2.0.html)
- `LGPL-2.1` - [GNU Lesser General Public License v2.1](https://spdx.org/licenses/LGPL-2.1.html)
- `LGPL-3.0` - [GNU Lesser General Public License v3](https://spdx.org/licenses/LGPL-3.0.html)
- `MIT` - [MIT License](https://spdx.org/licenses/MIT.html)
- `MPL-2.0` - [Mozilla Public License](https://spdx.org/licenses/MPL-2.0.html)
- `NLPL` - [No Limit Public License](https://spdx.org/licenses/NLPL.html)
- `OLDAP-2.8` - [Open LDAP Public License v2.8](https://spdx.org/licenses/OLDAP-2.8.html)
- `QPL-1.0` - [Q Public License 1.0](https://spdx.org/licenses/QPL-1.0.html)
- `Vim` - [Vim License](https://spdx.org/licenses/Vim.html)
- `Zlib` - [zlib License](https://spdx.org/licenses/Zlib.html)


--------------------

## 外部链接

## 社区 / 论坛

- [ArsTechnica OpenForum](https://arstechnica.com/civis/) - 附属于大型新闻网站的 IT 论坛。
- [Reddit](https://www.reddit.com) - 超大型论坛系统。
  - [/r/Linux](https://www.reddit.com/r/linux) - 有关 Linux 的新闻和信息。
  - [/r/LinuxQuestions](https://www.reddit.com/r/linuxquestions)
  - [/r/SysAdmin](https://www.reddit.com/r/sysadmin/)
- [Spiceworks Community](https://community.spiceworks.com/start) - 企业 IT 新闻与小型文章的综合社区。
- [StackExchange Network](https://stackexchange.com/sites#technology) - 问答社区网络。
  - [Server Fault](https://serverfault.com/) - 面向系统和网络管理员的 StackExchange 社区。

## 软件仓库

*软件包仓库。*

- [AlternativeTo](https://alternativeto.net) - 查找你熟悉软件的替代品并发现新软件。
- [deb.sury.org](https://deb.sury.org/) - Debian 和 Ubuntu 的 LAMP 更新包仓库。
- [ElRepo](https://elrepo.org/tiki/tiki-index.php) - 企业 Linux（RHEL、CentOS 等）的社区仓库。
- [EPEL](https://fedoraproject.org/wiki/EPEL) - RHEL 及兼容系统（CentOS、Scientific Linux）的仓库。
- [IUS](https://ius.io/) - 为企业 Linux 发行版提供部分软件新版本 RPM 包的社区项目。
- [Remi](http://rpms.famillecollet.com/) - RHEL/Centos/Fedora 的 LAMP 更新包仓库。
- [Software Collections](https://www.softwarecollections.org) - [Red Hat Software Collections](https://access.redhat.com/documentation/en/red-hat-software-collections/) 的社区发布，提供 CentOS/Scientific Linux 6.x 的 Ruby、Python 等更新包。

## 网站

- [Cloud Native Software Landscape](https://landscape.cncf.io/?group=projects-and-products&view-mode=card) - 云计算相关软件与工具的汇总。
- [ArchWiki](https://wiki.archlinux.org/) - Arch Linux Wiki，内容详实，适用于其他发行版。
- [Gentoo Wiki](https://wiki.gentoo.org/) - Gentoo Linux Wiki，详细介绍 Linux 组件。
- [Awesome SysAdmin @ LibHunt](https://sysadmin.libhunt.com) - 系统管理员工具箱，基于本列表整理。
- [Ops School](https://www.opsschool.org) - 帮助你成为运维工程师的综合性学习项目。
- [Digital Ocean 教程](https://www.digitalocean.com/community/tutorials) - 6000+ 篇关于应用、工具、系统管理主题的基础教程。

------------------

## 许可证

![cc license](http://i.creativecommons.org/l/by-sa/4.0/88x31.png)

本作品采用 [知识共享署名-相同方式共享 4.0 国际许可协议](http://creativecommons.org/licenses/by-sa/4.0/) 进行许可。
