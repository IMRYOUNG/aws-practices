## 02. 가상인프라구축 - ch03. 가상서버 EC2

### 01. 가상화와 EC2
1. Hypervisor : type1(HVM, PVM) , type2
2. AMI 
3. instance


### 02. 가상 서버 시작
1. EC2 인스턴스 생성
2. 가상 서버 시작


### 03. 가상 서버 운영
1. ssh : 가상 서버 접속 
    '''bash
    $ ssh -i mykey.pem ec2-user@[public ip]
    '''

2. 가성 서버 모니터링
3. 가상 서버 상태변경
4. 가상 서버 크기 변경


### 04. 네트워크 설정
1. Security Group : 방화벽 : 아파치 웹서버 운영
    '''bash
    # yum install -y httpd
    # systemctl enable httpd
    # service httpd [start|stop|restart]
    '''
2. Elastic IP(고정 IP) : 아파치 웹서버 접속
3. Network Interface 추가 : 2개의 고정 IP로 2개의 웹사이트를 운영
4.