
-온 프레미스 데이터 센터의 데이터와 AWS 클라우드의 스토리지를 연결하는 서비스

- 클라우드에는 Amazon Storage가 있음
-> 온프레미스 데이터센터에 애플리케이션이 구동됨

- 온 프레미스와 클라우드 인프라를 연결
-> 하이브리드 클라우드 스토리지 서비스
-> AWS에 데이터 백업, AWS 클라우드 스토리지로 파일공유

-4가지 유형의 게이트웨이 제공
(1) S3 파일게이트웨이
(2) FSx 파일게이트웨이
(3) 볼륨게이트웨이
(4) 테이프게이트웨이

- Amazon EC2에서 AMI로 배포
- 온-프레미스 로컬캐시 기능을 사용해 자주 사용하는 데이터 빠르게 접근 가능

1) S3 파일 게이트웨이
- 온프레미스와 S3간에 파일 기반 인터페이스를 제공하는 게이트웨이
- NFS, SMB 파일 공유 프로토콜을 사용하여 Amazon S3에 객체를 저장하고 검색 가능
- Active Directory 서비스와 통합하여 인증된 사용자만 액세스하도록 구성 가능
- 온프레미스의 파일 저장 공간이 부족하여

2) FSx 파일 게이트웨이
- SMB 프로토콜을 사용하여 FSx for Windows File Server 내의 파일을 저장하고 검색 가능

3) 볼륨 게이트웨이
- 온-프레미스와 S3간에 iSCSI 블록 스토리지 기반 인터페이스를 제공하는 게이트웨이
- 온-프레미스의 서버에서 S3의 블록 스토리지 볼륨을 iSCSI 디바이스로 연결 가능
- 볼륨 데이터는 S3에 저장되며 볼륨을 EBS 스냅샷으로 저장 및 AWS Backup 서비스로 백업 가능
- 두 가지 볼륨 모드
(1) 캐시 볼륨
(2) 저장 볼륨

4) 테이프 게이트웨이
- 온-프레미스와 S3간에 iSCSI VTL 인터페이스를 제공하는 게이트웨이 

5) 하드웨어 어플라이언스
- 
