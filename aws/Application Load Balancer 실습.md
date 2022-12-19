### Elastic Load Balancer 실습

- EC2 를 만들어주자 2개를 만들것인데
![img_78.png](img_78.png)
- 기본 AMI 선택
- 네트워크 설정은 기존 보안 그룹 선택
- 보안 그룹은 ssh-http_sg 선택
- 고급 세부 정보에 사용자 데이터를 다음과 같이 입력 (웹서버를 생성하는 스크립트를 생성)
```text
#!/bin/bash
yum update -y
yum install httpd -y
systemctl enable httpd.service
systemctl start httpd.service
cd /var/www/html
echo "안녕하세요. 형기의 스터디 입니다. $(hostname -f)" > index.html
```
- 인스턴스 시작을 선택하고
![img_79.png](img_79.png)
- 모든 인스턴스 보기 를 선택 후 하나 더 만들것이다. 
- 인스턴스 시작을 선택하고,
![img_80.png](img_80.png)
![img_81.png](img_81.png)
- 2개의 인스턴스가 잘 띄워졌으니 확인해보자.
![img_82.png](img_82.png)
옳지. 잘 띄워졌다.

### 대상그룹을 선택하자.
![img_83.png](img_83.png)
![img_86.png](img_86.png)
이름을 지어주고 ( 참고로 _ 언더바 안먹힘.)
![img_85.png](img_85.png)
상태 체크를 하면, 해당 HTTP 로 웹서버를 지속적으로 체크해준다.
![img_87.png](img_87.png)
![img_88.png](img_88.png)

여기까지 대상그룹을 생성하는 실습이였고, 이제 로드밸런서를 생성해보자.
![img_89.png](img_89.png)
![img_90.png](img_90.png)
![img_91.png](img_91.png)
![img_92.png](img_92.png)

네트워크 매핑을 모두 선택
![img_93.png](img_93.png)

보안그룹 을 ssh_http 로 선택
![img_94.png](img_94.png)

로드발란서에서 어디로 라우팅 할지 선택
![img_95.png](img_95.png)

방금전에 만들어준 EC2 TG 를 선택해준다. (로드 발란서에서 트래픽이 들어오면 EC2_TG 로 보내게 됨 [ 이게 리스너])
![img_96.png](img_96.png)

애플리케이션 로드발란서가 프로비저닝 중인것을 볼 수 있다.
![img_97.png](img_97.png)

대상그룹이 생성된 것을 확인하면,
![img_98.png](img_98.png)

굳굳.

대상그룹에 대상을 보면 등록된 EC2 가 잘나오는것도 체크하자 
![img_99.png](img_99.png)

그리고 상태가 healthy 인것도 확인하자.

로드발란서에 접속하면 알아서 두개의 인스턴스에 트래픽을 적절히 분배해준다.

로드발란서 설명에 DNS 이름을 보면 주소를 복사해서 새텝에 복사 후 접속하면 
![img_100.png](img_100.png)

적절히 두개의 웹서버를 번갈아 가면서 트레픽을 분배해준다.