# Nmap Cheat Sheet

## Port Scanning Options
```
nmap -p 23 172.16.1.1
nmap -p 23-128 172.16.1.1
nmap -pT:23,45,249 -pU:110,82 172.16.1.1
nmap -p 172.16.1.1
nmap --top-ports 20 172.16.1.1
nmap -F 172.16.1.1
nmap -r 172.16.1.1
```

## Host Discovery
```
nmap -SL 172.16.1.1-5
nmap -PS 172.16.1.1-5
nmap -PA 172.16.1.1-5
nmap -PU 172.16.1.1-5
nmap -PY 172.16.1.1-5
nmap -PR 172.16.1.1-5
nmap -PE -PP -PM 172.16.1.1
nmap -n 172.16.1.1
```

## Scan Types
```
nmap -sS 172.16.1.1
nmap -sT 172.16.1.1
nmap -sU 172.16.1.1
nmap -sY 172.16.1.1
nmap -sZ 172.16.1.1
nmap -sA 172.16.1.1
nmap -sW 172.16.1.1
nmap -sN 172.16.1.1
nmap -sF 172.16.1.1
nmap -sX 172.16.1.1
nmap -sL 172.16.1.1
```

## Version Detection
```
nmap -sV 172.16.1.1
nmap -sV --version-intensity 0 172.16.1.1
nmap -sV --version-intensity 9 172.16.1.1
nmap -sV --version-all 172.16.1.1
nmap -sV --version-light 172.16.1.1
nmap -A 172.16.1.1
```

## Nmap Script Engine (NSE)
```
nmap --script test-script 172.16.1.1/24
nmap -sV --script=all
nmap --script script-db
nmap --script-args
nmap --script-help="Test Script"
```

## Firewall Evasion
```
nmap -f 172.16.1.1
nmap -mtu [MTU] 172.16.1.1
nmap -D RND:10 172.16.1.1
nmap -S 172.16.1.1
nmap -g 80 172.16.1.1
nmap -proxies proxy1 URL proxy2 URL
nmap -spoof-mac 0
nmap -randomize-hosts 172.16.1.1
nmap -badsum 172.16.1.1
```

## Output Options
```
nmap -oN scan1.txt 172.16.1.1
nmap -oX scan.xml 172.16.1.1
nmap -oG scan.grep.txt 172.16.1.1
nmap -oA scan 172.16.1.1
```

## Target Examples
```
nmap 172.16.1.1
nmap 172.16.1.1-15
nmap 172.16.1.1,3,4,8
nmap 172.16.1.0/24
nmap -iL scan.txt 172.16.1.0/24
nmap --exclude 172.16.1.1
```

## Scan Options
```
nmap -sP 172.16.1.1
nmap -PN 172.16.1.1
nmap -PE 172.16.1.1
nmap -PP 172.16.1.1
nmap -PM 172.16.1.1
nmap -PS 172.16.1.1
nmap -PA 172.16.1.1
nmap -PU 172.16.1.1
nmap -PY 172.16.1.1
nmap -PR 172.16.1.1
nmap -traceroute 172.16.1.1
```

## Timing Templates
```
nmap -T0 172.16.1.1
nmap -T1 172.16.1.1
nmap -T2 172.16.1.1
nmap -T3 172.16.1.1
nmap -T4 172.16.1.1
nmap -T5 172.16.1.1
```
