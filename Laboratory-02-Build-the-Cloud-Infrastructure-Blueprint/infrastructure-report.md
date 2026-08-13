# Operating System
cat /etc/os-release | grep -E "^(NAME|VERSION)="

# Kernel Version
uname -r

# CPU Model
lscpu | grep "Model name" | cut -d':' -f2 | xargs

# Number of CPU Cores
nproc

# Total RAM
free -h | grep Mem | awk '{print $2}'

# Disk Capacity
df -h --total | grep total | awk '{print $2}'

# Mounted File Systems
df -hT | grep -v "^tmpfs" | grep -v "^devtmpfs"

# Hostname
hostname

# IP Address
ip -4 addr show | grep -oP '(?<=inet\s)\d+(\.\d+){3}' | grep -v "127.0.0.1" | head -1
