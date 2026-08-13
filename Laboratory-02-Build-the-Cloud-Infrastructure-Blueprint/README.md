# Technical Documentation
# Cloud Infrastructure Laboratory


## Mission Overview


The laboratory task has been created to provide practical experience with the parts of cloud infrastructure using a Linux-based cloud environment. KillerCoda platform has been utilized to replicate the scenario of cloud engineering where participants can research, report, and study the primary foundational components of cloud computing. The mission connects theory and practice and allows participants to work in a real-time cloud server environment while helping them with accomplishing structured investigative processes.


## Objectives


The main goals of this laboratory were the following:


1. **Study the Cloud Server Environment**
   - Check and describe the operating system, kernel version, CPU specifications, memory, storage, and network configurations of Linux-based cloud instance


2. **Define Cloud Infrastructure Parts**
   - Identify and categorize the compute, storage, networking, and OS resources within the environment
   - Understand the operational role of every component in cloud computing


3. **Make Comparisons Between the Leading Cloud Providers**
   - Research and analyze similar services offered by AWS, Microsoft Azure, and Google Cloud
   - Investigate the pros and cons of the existing providers

4. **Acquisition of Technical Documentation Skills**
   - Produce a proper structuring of markdown documentation according to acceptable standards
   - Arrange findings in an understandable, business-like way for team members to review them

5. **Using Linux Administration Skills**
   - Perform system information commands to achieve vital information on the infrastructure
   - Browse through and check the Linux filesystem arrangement

## Components of Cloud Infrastructure

### Computing Resources
The lab environment implemented the use of virtualized computing resources.
- **CPU**: Virtual processors having the required number of cores and processing capacity
- **Purpose**: Giving information certain amount of processing
- **Significance**: The infrastructure serves as a basis of cloud computing capabilities
- **KillerCoda Context**: The infrastructure contains isolated computing capabilities that can be analyzed further using `lscpu`, `nproc`, and `/proc/cpuinfo`

### Storage Resources
The storage infrastructure that was investigated included:
- **Disk Storage**: Virtual block storage with a set capacity (GB/TB)
- **File Systems**: Mounted file systems with different formats (ext4, xfs, etc.)
- **Purpose**: Offers permanent and temporary storage of data for programs and users
- **Importance**: Allows the retention of data, implementing backup strategies, scalable storage solutions
- **KillerCoda Context**: Temporary storage that resets at the end of each session, studied using `df -h`, `lsblk`, `mount` commands  

### Networking Resources
Network configuration consisted of:
- **Virtual Network Interfaces**: Ethernet interfaces with assigned IP addresses
- **Network Connectivity**: Internet access for package downloads and outside communication
- **Purpose**: Provides means of communication between services, users and external systems
- **Importance**: Important for connectivity, load balancing, security groups, and high availability
- **KillerCoda Context**: Secluded virtual network with specified IP addressing, researched using `ip addr show`, `ping`, and `hostname -I`

### Operating System
The Linux operating system consists of:
- **Distribution**: Type of Linux distribution (Ubuntu, CentOS, Alpine, etc.)
- **Kernel Version**: The version of Linux kernel with the version number applicable to it
- **Purpose**: Manages the hardware and provides system service functions for application running
- **Importance**: Acts as an interface between hardware and software and ensures security, as well as resource management
- **KillerCoda Context**: Complete Linux environment accessible through CLI, as seen in `/etc/os-release`, `uname -r`, and other

## Tools Used


### Cloud Platform
- **KillerCoda**: Practical cloud-based Linux terminal environment
- **Browser terminal**: Way of using command line

### Command Line Tools
- **System Information**: `lscpu`, `nproc`, `cat`, `free`, `df`, `lsblk`
- **Network Tools**: `ip`, `ping`, `hostname`, `curl`, `wget`
- **File Management Tools**: `ls`, `cd`, `mkdir`, `touch`, `nano`, `vi`
- **Text Processing Tools**: `grep`, `awk`, `cut`, `sed`, `xargs`
- **Documentation Tools**: `echo`, `cat > file.md`, `nano`, `vim`


## Challenges Encountered 
1. Provider Documentation Navigation: The challenge lies in the process of locating equivalent services that are available across different three cloud provider documentation systems, which vary in their structure and layout.
2. Markdown Table Formatting: The challenge here is that the comparison table needs to be constructed accurately in markdown, requiring it to have multiple columns and lengthy service names.
3. System Information Collection: The challenge lies in the task of collecting relevant system information using a single command in an easy-to-understand manner.
4. Ephemeral Environment Constraints: Due to the temporary nature of the KillerCoda system, capturing documentation and investigation findings must be done quickly.

## List of Linux Commands

### Commands to Know the Status of Your System
```bash
# Get Operating System and Kernel information
cat /etc/os-release
uname -r
hostnamectl


# Get CPU information
lscpu
nproc
cat /proc/cpuinfo | grep "model name" | head -1


# Get Memory status
free -h
cat /proc/meminfo | grep MemTotal


# Get Storage Information of your system
df -h
df -hT
lsblk
du -sh /* 2>/dev/null | sort -hr | head -10


