# AWS Certified Cloud Practitioner (CLF-C02) 모의 고사

---

# 문제 1

한 스타트업은 자체 서버를 구매하지 않고 필요할 때마다 컴퓨팅 자원을 사용하고, 사용한 만큼만 비용을 지불하고 싶어 한다.

AWS Cloud의 어떤 특징을 가장 잘 설명하는가?

A. High Availability

B. Pay-as-you-go Pricing

C. Fault Tolerance

D. Dedicated Host

---

## 정답

✅ **B**

---

## 풀이

AWS의 가장 큰 장점은 **Pay-as-you-go(사용한 만큼 지불)** 입니다.

필요할 때 EC2를 생성하고 사용이 끝나면 종료하면 그 시간만큼만 과금됩니다.

---

### 오답

A

고가용성

C

장애 허용

D

전용 물리 서버

---

### 시험 포인트

**Pay-as-you-go = AWS의 대표적인 비용 모델**

---

# 문제 2

한 회사는 연말 쇼핑 시즌 동안 평소보다 15배 많은 사용자가 접속한다.

자동으로 서버 수를 늘렸다가 사용자가 줄어들면 다시 서버를 줄이는 AWS Cloud의 특징은?

A. Scalability

B. Elasticity

C. Durability

D. Agility

---

## 정답

✅ **B**

---

## 풀이

Elasticity는

> 필요한 순간 자동으로 확장하고,
> 사용량이 줄면 자동으로 축소하는 특징이다.

AWS Auto Scaling이 대표적인 예이다.

---

### 오답

Scalability

→ 단순히 용량을 늘릴 수 있는 능력

Elasticity

→ 자동 증가 + 자동 감소

---

### 시험 포인트

**Elasticity = 자동**

---

# 문제 3

다음 중 AWS Global Infrastructure를 구성하는 요소가 아닌 것은?

A. Region

B. Availability Zone

C. Edge Location

D. Rack

---

## 정답

✅ **D**

---

## 풀이

AWS Global Infrastructure

* Region
* AZ
* Edge Location
* Local Zone

Rack은 AWS 고객이 관리하는 개념이 아니다.

---

# 문제 4

AWS Shared Responsibility Model에서 고객(Customer)이 책임지는 것은?

A. 데이터 암호화

B. 물리적 서버 관리

C. 데이터센터 건물 관리

D. 하드웨어 교체

---

## 정답

✅ **A**

---

## 풀이

고객 책임

* IAM
* 데이터
* 암호화
* 운영체제 패치(EC2)

AWS 책임

* 서버
* 네트워크
* 데이터센터
* 전원

---

### 시험 암기

Security **IN** the Cloud → 고객

Security **OF** the Cloud → AWS

---

# 문제 5

Well-Architected Framework의 6가지 기둥(Pillar)에 포함되지 않는 것은?

A. Reliability

B. Sustainability

C. Cost Optimization

D. Virtualization

---

## 정답

✅ **D**

---

## 풀이

6 Pillars

* Operational Excellence
* Security
* Reliability
* Performance Efficiency
* Cost Optimization
* Sustainability

---

# 문제 6

한 회사는 여러 AWS 계정을 중앙에서 관리하려고 한다.

가장 적합한 서비스는?

A. IAM

B. Organizations

C. CloudTrail

D. Config

---

## 정답

✅ **B**

---

## 풀이

Organizations

* 여러 계정 관리
* SCP 적용
* 통합 결제

---

# 문제 7

AWS에서 사용자(User), 그룹(Group), 역할(Role), 정책(Policy)을 관리하는 서비스는?

A. IAM

B. Shield

C. GuardDuty

D. Inspector

---

## 정답

✅ **A**

---

## 풀이

IAM은 AWS의 인증(Authentication)과 권한 부여(Authorization)를 담당하는 핵심 서비스입니다.

---

# 문제 8

EC2 인스턴스가 S3에 접근할 수 있도록 자격 증명을 안전하게 제공하려고 한다.

가장 적절한 방법은?

A. Access Key를 코드에 저장

B. IAM Role 연결

C. Root 계정 사용

D. IAM 사용자 비밀번호 저장

---

## 정답

✅ **B**

---

## 풀이

EC2 → S3 접근 시에는 **IAM Role**을 사용해야 합니다. Access Key를 코드에 저장하는 것은 보안상 권장되지 않습니다.

---

### 시험 포인트

EC2 → S3 = IAM Role

---

# 문제 9

AWS API 호출 기록을 저장하여 누가 언제 어떤 작업을 수행했는지 감사(Audit)하려고 한다.

가장 적합한 서비스는?

A. CloudWatch

B. CloudTrail

C. Config

D. Inspector

---

## 정답

✅ **B**

---

## 풀이

CloudTrail은 AWS API 호출 내역을 기록하는 감사 서비스입니다.

---

# 문제 10

AWS 리소스의 구성(Configuration) 변경 내역을 추적하고 규정 준수 여부를 확인하는 서비스는?

A. Config

B. CloudTrail

C. CloudWatch

D. SNS

---

## 정답

✅ **A**

---

## 풀이

AWS Config는 리소스의 설정 변경을 기록하고, 규정 준수 여부를 지속적으로 평가합니다.

---

# 문제 11

웹 애플리케이션을 SQL Injection 및 XSS 공격으로부터 보호하려고 한다.

가장 적절한 서비스는?

A. Shield

B. WAF

C. GuardDuty

D. Inspector

---

## 정답

✅ **B**

---

## 풀이

AWS WAF는 웹 애플리케이션 계층(Layer 7)의 공격을 차단하는 웹 방화벽입니다.

---

# 문제 12

AWS 계정에서 비정상적인 API 호출과 악성 활동을 탐지하려고 한다.

가장 적합한 서비스는?

A. Inspector

B. GuardDuty

C. CloudTrail

D. Config

---

## 정답

✅ **B**

---

## 풀이

GuardDuty는 머신러닝과 위협 인텔리전스를 활용하여 비정상적인 활동과 잠재적 보안 위협을 탐지합니다.

---

# 문제 13

DDoS 공격으로부터 AWS 리소스를 보호하는 기본 서비스는?

A. WAF

B. Shield Standard

C. IAM

D. Macie

---

## 정답

✅ **B**

---

## 풀이

Shield Standard는 대부분의 AWS 고객에게 기본 제공되며, 일반적인 DDoS 공격으로부터 보호합니다.

---

# 문제 14

Amazon EC2의 가장 적절한 설명은?

A. 객체 스토리지

B. 가상 서버

C. NoSQL 데이터베이스

D. CDN

---

## 정답

✅ **B**

---

## 풀이

EC2(Elastic Compute Cloud)는 AWS에서 제공하는 가상 서버 서비스입니다.

---

# 문제 15

EC2 인스턴스의 수를 트래픽에 따라 자동으로 늘리거나 줄이는 서비스는?

A. Auto Scaling

B. Route 53

C. Lambda

D. CloudFormation

---

## 정답

✅ **A**

---

## 풀이

Auto Scaling은 수요 변화에 따라 EC2 인스턴스 수를 자동으로 조정하여 성능과 비용을 최적화합니다.

---

# 문제 16

여러 EC2 인스턴스로 들어오는 요청을 자동으로 분산하는 서비스는?

A. CloudFront

B. Elastic Load Balancer

C. Route 53

D. API Gateway

---

## 정답

✅ **B**

---

## 풀이

Elastic Load Balancer(ELB)는 트래픽을 여러 EC2 인스턴스에 분산하여 가용성과 확장성을 높입니다.

---

# 문제 17

서버를 관리하지 않고 이벤트가 발생할 때만 코드를 실행하는 서비스는?

A. ECS

B. EC2

C. Lambda

D. EKS

---

## 정답

✅ **C**

---

## 풀이

AWS Lambda는 대표적인 서버리스(FaaS) 서비스로, 이벤트 기반으로 코드를 실행하며 서버 관리가 필요 없습니다.

---

# 문제 18

이미지, 동영상, 백업 파일과 같은 객체 데이터를 저장하는 서비스는?

A. EBS

B. EFS

C. S3

D. FSx

---

## 정답

✅ **C**

---

## 풀이

Amazon S3는 객체(Object) 스토리지 서비스로, 높은 내구성과 확장성을 제공합니다.

---

# 문제 19

관계형 데이터베이스(RDB)를 관리형으로 제공하는 서비스는?

A. DynamoDB

B. Redshift

C. RDS

D. ElastiCache

---

## 정답

✅ **C**

---

## 풀이

Amazon RDS는 MySQL, PostgreSQL, MariaDB, Oracle, SQL Server 등의 관계형 데이터베이스를 관리형으로 제공합니다.

---

# 문제 20

다음 중 AWS의 NoSQL 데이터베이스 서비스는?

A. Aurora

B. PostgreSQL

C. DynamoDB

D. RDS for MySQL

---

## 정답

✅ **C**

---

## 풀이

Amazon DynamoDB는 완전관리형 NoSQL 데이터베이스로, 높은 성능과 자동 확장 기능을 제공합니다.

Aurora와 RDS는 관계형 데이터베이스 서비스입니다.

---

## 문제 21

한 회사는 VPC 내부의 EC2 인스턴스가 인터넷에서 직접 접근되지 않도록 구성하면서도, 운영체제 업데이트를 위해 인터넷에는 접속할 수 있도록 하려고 한다.

가장 적절한 서비스는?

A. Internet Gateway

B. NAT Gateway

C. Route 53

D. Elastic IP

---

### 정답

✅ **B**

### 풀이

Private Subnet의 EC2는 인터넷에서 직접 접근되면 안 됩니다. 하지만 외부 저장소(예: 패키지 저장소)에 접속하여 업데이트를 수행해야 하는 경우 **NAT Gateway**를 사용합니다.

### 오답

* **A. Internet Gateway** → Public Subnet에서 인터넷 연결을 제공합니다.
* **C. Route 53** → DNS 서비스입니다.
* **D. Elastic IP** → 고정 공인 IP입니다.

### 시험 포인트

> **Private Subnet → NAT Gateway → Internet**

---

# 문제 22

도메인 이름([www.example.com)을](http://www.example.com%29을) AWS 리소스로 연결하는 서비스는?

A. CloudFront

B. Route 53

C. ELB

D. CloudWatch

---

### 정답

✅ **B**

### 풀이

Route 53은 AWS의 관리형 DNS 서비스로 도메인 이름을 IP 주소나 AWS 리소스로 연결합니다.

---

# 문제 23

전 세계 사용자에게 이미지와 동영상을 빠르게 제공하려고 한다.

가장 적합한 서비스는?

A. S3

B. CloudFront

C. EBS

D. Glacier

---

### 정답

✅ **B**

### 풀이

CloudFront는 CDN(Content Delivery Network) 서비스로, 전 세계 엣지 로케이션을 통해 콘텐츠를 빠르게 전달합니다.

### 오답

* S3 → 객체 저장
* EBS → 블록 스토리지
* Glacier → 장기 보관

---

# 문제 24

다음 중 블록 스토리지(Block Storage)는?

A. S3

B. EFS

C. EBS

D. FSx

---

### 정답

✅ **C**

### 풀이

EBS는 EC2에 연결하는 블록 스토리지입니다.

### 암기

* S3 = Object
* EBS = Block
* EFS = File

---

# 문제 25

여러 EC2 인스턴스가 동시에 접근할 수 있는 파일 스토리지는?

A. S3

B. EBS

C. EFS

D. Glacier

---

### 정답

✅ **C**

### 풀이

Amazon EFS는 NFS 기반의 공유 파일 시스템으로 여러 EC2 인스턴스에서 동시에 사용할 수 있습니다.

---

# 문제 26

거의 접근하지 않는 데이터를 가장 저렴하게 장기 보관하려고 한다.

가장 적합한 서비스는?

A. S3 Standard

B. Glacier Deep Archive

C. EBS

D. EFS

---

### 정답

✅ **B**

### 풀이

Glacier Deep Archive는 장기 보관용으로 가장 저렴하지만 복구 시간이 오래 걸립니다.

---

# 문제 27

완전관리형 NoSQL 데이터베이스는?

A. Aurora

B. PostgreSQL

C. DynamoDB

D. Oracle

---

### 정답

✅ **C**

### 풀이

DynamoDB는 AWS의 대표적인 NoSQL 데이터베이스입니다.

---

# 문제 28

MySQL과 호환되면서 더 높은 성능과 자동 복구 기능을 제공하는 AWS 데이터베이스는?

A. RDS

B. Aurora

C. Redshift

D. DynamoDB

---

### 정답

✅ **B**

### 풀이

Aurora는 MySQL 및 PostgreSQL과 호환되며, 일반 MySQL보다 높은 성능과 가용성을 제공합니다.

---

# 문제 29

데이터 웨어하우스(Data Warehouse) 서비스는?

A. DynamoDB

B. Aurora

C. Redshift

D. ElastiCache

---

### 정답

✅ **C**

### 풀이

Redshift는 OLAP 분석용 데이터 웨어하우스 서비스입니다.

---

# 문제 30

애플리케이션의 응답 속도를 높이기 위해 메모리 캐시를 사용하려고 한다.

가장 적합한 서비스는?

A. ElastiCache

B. CloudTrail

C. Athena

D. Inspector

---

### 정답

✅ **A**

### 풀이

ElastiCache는 Redis 또는 Memcached 기반의 인메모리 캐시 서비스입니다.

---

# 문제 31

Docker 컨테이너를 AWS에서 실행하려고 한다.

AWS의 컨테이너 오케스트레이션 서비스는?

A. Lambda

B. ECS

C. S3

D. CloudFront

---

### 정답

✅ **B**

### 풀이

Amazon ECS는 AWS의 관리형 컨테이너 오케스트레이션 서비스입니다.

---

# 문제 32

Kubernetes 기반으로 컨테이너를 운영하려고 한다.

가장 적합한 서비스는?

A. ECS

B. Lambda

C. EKS

D. EC2 Auto Scaling

---

### 정답

✅ **C**

### 풀이

Amazon EKS는 완전관리형 Kubernetes 서비스입니다.

---

# 문제 33

컨테이너는 실행하지만 서버를 직접 관리하고 싶지 않다.

가장 적합한 서비스는?

A. EC2

B. ECS on EC2

C. Fargate

D. Lightsail

---

### 정답

✅ **C**

### 풀이

AWS Fargate는 서버리스 컨테이너 실행 환경입니다.

### 암기

> Fargate = Lambda의 컨테이너 버전이라고 생각하면 이해하기 쉽습니다.

---

# 문제 34

REST API를 생성하고 관리하는 서비스는?

A. API Gateway

B. Route53

C. CloudFormation

D. SNS

---

### 정답

✅ **A**

### 풀이

API Gateway는 REST API 및 HTTP API를 생성·관리하는 서비스입니다.

---

# 문제 35

이벤트가 발생하면 자동으로 Lambda를 실행하려고 한다.

가장 적합한 서비스는?

A. EventBridge

B. Route53

C. IAM

D. Shield

---

### 정답

✅ **A**

### 풀이

EventBridge는 다양한 AWS 서비스와 SaaS의 이벤트를 감지하여 Lambda, Step Functions 등을 실행합니다.

---

# 문제 36

여러 Lambda 함수를 순서대로 실행해야 한다.

가장 적합한 서비스는?

A. Auto Scaling

B. Step Functions

C. Route53

D. Config

---

### 정답

✅ **B**

### 풀이

Step Functions는 여러 작업을 워크플로 형태로 연결하고 순서를 제어합니다.

---

# 문제 37

AWS 예상 비용을 계산하는 서비스는?

A. Cost Explorer

B. Pricing Calculator

C. Budgets

D. CUR

---

### 정답

✅ **B**

### 풀이

Pricing Calculator는 새로운 시스템 구축 전 예상 비용을 산정하는 데 사용합니다.

---

# 문제 38

현재까지 실제 발생한 비용과 사용량을 분석하는 서비스는?

A. Pricing Calculator

B. Cost Explorer

C. IAM

D. Route53

---

### 정답

✅ **B**

### 풀이

Cost Explorer는 실제 사용 비용을 분석하고 시각화합니다.

---

# 문제 39

예산을 초과할 것 같을 때 이메일 알림을 보내는 서비스는?

A. CUR

B. Budgets

C. Trusted Advisor

D. CloudTrail

---

### 정답

✅ **B**

### 풀이

AWS Budgets는 예산을 설정하고 임계값에 도달하면 알림을 보냅니다.

---

# 문제 40

24시간 기술 지원, Trusted Advisor 전체 검사, TAM(Technical Account Manager)을 제공하는 지원 플랜은?

A. Basic

B. Developer

C. Business

D. Enterprise

---

### 정답

✅ **D**

### 풀이

Enterprise Support는 최고 수준의 지원 플랜으로, 전담 TAM과 전략적 기술 지원을 제공합니다.

### 오답

* **Basic** → 무료 기본 지원
* **Developer** → 개발 환경 중심
* **Business** → 24×7 기술 지원 제공하지만 TAM은 포함되지 않음
* **Enterprise** → TAM 포함, 대규모 운영 환경에 적합


# 문제 41

한 회사는 사용자의 로그인 정보를 안전하게 관리하고, 웹 및 모바일 애플리케이션의 회원 가입과 로그인을 쉽게 구현하려고 한다.

가장 적합한 AWS 서비스는?

A. IAM

B. Amazon Cognito

C. AWS Organizations

D. AWS Directory Service

### 정답

✅ **B**

### 풀이

Amazon Cognito는 애플리케이션 사용자 인증(회원가입, 로그인, 소셜 로그인, MFA 등)을 제공합니다.

**오답**

* A: IAM은 AWS 리소스 접근 권한 관리
* C: Organizations는 AWS 계정 관리
* D: Directory Service는 Microsoft AD 연동

**시험 포인트**

> IAM = AWS 사용자
> Cognito = 애플리케이션 사용자

---

# 문제 42

여러 AWS 계정에 동일한 보안 정책을 적용하고 특정 서비스를 사용하지 못하도록 제한하려고 한다.

가장 적합한 기능은?

A. IAM Policy

B. SCP(Service Control Policy)

C. Security Group

D. NACL

### 정답

✅ **B**

### 풀이

SCP는 AWS Organizations에서 계정 전체에 권한 제한을 적용합니다.

---

# 문제 43

AWS 리소스의 보안 상태를 통합적으로 확인하고 여러 보안 서비스의 결과를 한곳에서 관리하려고 한다.

가장 적합한 서비스는?

A. AWS Security Hub

B. CloudTrail

C. Config

D. GuardDuty

### 정답

✅ **A**

### 풀이

Security Hub는 GuardDuty, Inspector, Macie 등의 보안 결과를 통합하여 보여줍니다.

---

# 문제 44

EC2 인스턴스의 운영체제 및 애플리케이션 취약점을 검사하려고 한다.

가장 적합한 서비스는?

A. Inspector

B. Macie

C. Shield

D. WAF

### 정답

✅ **A**

---

# 문제 45

Amazon S3에 저장된 개인정보(PII)를 자동으로 탐지하려고 한다.

가장 적합한 서비스는?

A. GuardDuty

B. Inspector

C. Macie

D. Config

### 정답

✅ **C**

---

# 문제 46

AWS 규정 준수 보고서(SOC, ISO, PCI DSS 등)를 다운로드하려고 한다.

가장 적합한 서비스는?

A. Artifact

B. Trusted Advisor

C. Config

D. CloudTrail

### 정답

✅ **A**

---

# 문제 47

AWS 사용 환경에서 비용 절감, 성능 향상, 보안 개선 사항을 추천받고 싶다.

가장 적합한 서비스는?

A. AWS Trusted Advisor

B. CloudWatch

C. EventBridge

D. Athena

### 정답

✅ **A**

---

# 문제 48

애플리케이션에서 서로 다른 컴포넌트 간 비동기 메시지 전달이 필요하다.

가장 적합한 서비스는?

A. Amazon SQS

B. Amazon EC2

C. Amazon RDS

D. AWS Config

### 정답

✅ **A**

### 시험 포인트

SQS = 메시지 큐

---

# 문제 49

하나의 메시지를 여러 애플리케이션에 동시에 전달하려고 한다.

가장 적합한 서비스는?

A. SNS

B. SQS

C. EventBridge

D. Lambda

### 정답

✅ **A**

### 암기

SNS = Publish / Subscribe

---

# 문제 50

EC2 인스턴스에서 CPU 사용률이 80% 이상일 때 관리자에게 알림을 보내려고 한다.

가장 적합한 서비스는?

A. CloudWatch

B. Config

C. CloudTrail

D. Inspector

### 정답

✅ **A**

---

# 문제 51

한 회사는 AWS 리소스를 코드로 정의하여 동일한 인프라를 반복적으로 배포하려고 한다.

가장 적합한 서비스는?

A. CloudFormation

B. CloudWatch

C. IAM

D. CloudTrail

### 정답

✅ **A**

---

# 문제 52

회사는 EC2 인스턴스를 3년 동안 계속 사용할 예정이다.

가장 비용 효율적인 과금 옵션은?

A. On-Demand

B. Spot

C. Reserved Instance

D. Dedicated Host

### 정답

✅ **C**

---

# 문제 53

배치 작업을 실행하며, 작업이 중단되어도 다시 실행할 수 있는 환경이다.

가장 비용이 저렴한 EC2 옵션은?

A. On-Demand

B. Spot Instance

C. Reserved Instance

D. Dedicated Instance

### 정답

✅ **B**

---

# 문제 54

다음 중 서버리스(Serverless) 서비스만으로 구성된 것은?

A. EC2 + RDS

B. Lambda + API Gateway + DynamoDB

C. ECS + EBS

D. EC2 + S3

### 정답

✅ **B**

---

# 문제 55

Amazon S3의 가장 중요한 특징은?

A. Block Storage

B. Object Storage

C. File Storage

D. Relational Database

### 정답

✅ **B**

---

# 문제 56

AWS에서 전 세계적으로 가장 많은 리전(Region)을 운영하는 이유는 무엇인가?

A. 서버 판매

B. 낮은 지연 시간과 재해 복구

C. 인터넷 속도 증가

D. 운영체제 제공

### 정답

✅ **B**

---

# 문제 57

AWS Lambda의 과금 기준은?

A. CPU 개수

B. 실행 시간과 호출 횟수

C. 메모리 용량만

D. 디스크 크기

### 정답

✅ **B**

---

# 문제 58

EC2 인스턴스에 영구적으로 연결되는 블록 스토리지는?

A. S3

B. EBS

C. Glacier

D. EFS

### 정답

✅ **B**

---

# 문제 59

CloudFront가 사용하는 AWS 글로벌 인프라 구성 요소는?

A. Availability Zone

B. Region

C. Edge Location

D. Local Zone

### 정답

✅ **C**

---

# 문제 60

회사는 AWS 비용이 갑자기 증가한 원인을 분석하려고 한다.

가장 적합한 서비스는?

A. AWS Budgets

B. Cost Explorer

C. Pricing Calculator

D. Trusted Advisor

### 정답

✅ **B**

---

# 문제 61

AWS에서 예산 초과 전에 이메일 알림을 받으려면?

A. Cost Explorer

B. AWS Budgets

C. CUR

D. Trusted Advisor

### 정답

✅ **B**

---

# 문제 62

다음 중 AWS의 책임(Security of the Cloud)은?

A. IAM 사용자 생성

B. 운영체제 패치(EC2)

C. 데이터센터 보안

D. S3 버킷 정책 설정

### 정답

✅ **C**

---

# 문제 63

애플리케이션이 여러 AWS 서비스의 이벤트를 연결하여 자동화된 워크플로를 구성하려고 한다.

가장 적합한 조합은?

A. EventBridge + Step Functions

B. IAM + Config

C. Route 53 + CloudFront

D. EBS + EFS

### 정답

✅ **A**

---

# 문제 64

다음 중 AWS Well-Architected Framework의 핵심 목표와 가장 거리가 먼 것은?

A. 비용 최적화

B. 운영 우수성

C. 보안

D. 서버 직접 구매

### 정답

✅ **D**

---

# 문제 65

다음 중 AWS Cloud의 가장 큰 장점으로 가장 적절한 것은?

A. 모든 서버를 직접 설치해야 한다.

B. 필요한 만큼만 리소스를 사용하고 비용을 지불할 수 있다.

C. 모든 서비스가 무료이다.

D. 항상 하나의 리전만 사용할 수 있다.

### 정답

✅ **B**

