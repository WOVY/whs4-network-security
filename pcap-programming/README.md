# tcp_sniffer

PCAP API를 활용하여 TCP 패킷의 Ethernet/IP/TCP 헤더 및 HTTP 페이로드를 출력하는 패킷 스니퍼입니다.

## 의존성 설치

```bash
sudo apt install libpcap-dev
```

## 빌드

```bash
gcc -o tcp_sniffer tcp_sniffer.c -lpcap
```

## 실행

```bash
sudo ./tcp_sniffer
```

## 테스트 방법

**서버 (Ubuntu)**
```bash
nc -lp 8080
```

**클라이언트 (Windows)**
```bash
curl http://[우분투 IP]:8080/
```

## 실행 환경

- OS : Ubuntu (VMware)
- 인터페이스 : ens33
- 클라이언트 : Windows curl
