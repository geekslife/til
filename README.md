# Today I Leanred

## [Agile](agile.md)

## [Spring](java/pring.md)

## [Database](java/database.md)

## AWS

### [Projects on AWS](https://aws.amazon.com/getting-started/projects/)

- [Build a Serverless Web Application](https://aws.amazon.com/getting-started/projects/build-serverless-web-app-lambda-apigateway-s3-dynamodb-cognito?trk=gs_card): 깔끔하게 정리된 튜토리얼. 강추 S3, Cognito, API GW, Lambda, Dynamo, CloudWatch 를 이용한 웹서비스 구축 연습
- [Publish Amazon SNS Messages Privately](https://aws.amazon.com/getting-started/projects/publish-sns-message-privately-vpc-ec2-cloudformation-lambda/?trk=gs_card): **VPC** 에서 SNS로 연결하고 Pub하면,  VPC외부의 Lambda와 CloudWatch로 Sub 되는 시나리오 연습
- [Set Up a CI/CD Pipeline on AWS](https://aws.amazon.com/getting-started/projects/set-up-ci-cd-pipeline/): S3 -> EC2 배포를 **CodeDeploy** 를 이용해 셋업해본다.
- [Launch a LAMP Stack Web App](https://aws.amazon.com/getting-started/projects/launch-lamp-web-app/): 다른 프로젝트에 비해 설명이 불친절하고 제대로 동작하지 않아 실패.. 이보다는 Serverless Web App 쪽을 추천해야할 듯

### Amazon RDS

- [Amazon Aurora를 통한 고성능 데이터베이스 운용하기](https://www.youtube.com/watch?v=870L5VLgkj0)

### VPC

* default VPC에 대해서
  - 한참 버벅였었는데. 이제는 항상 VPC 를 이용해야 하고. 이 때 생성되는 것이 기본 VPC 다. 기본 VPC는 인터넷 게이트웨이가 기본적으로 만들어져 있음. 라우팅 테이블도 인터넷 게이트웨이가 설정되어 있기 때문에 퍼블릭 서브넷임.
  - EC2 를 만들어보면, security group 의 기본 inbound 가 0.0.0.0/22 라서 ssh 가 잘 먹는 것임.
* VPC 구성요소
  - VPC 는 가상 사설망으로 서브넷을 구성한다. 기본으로는 /16 을 쓴다.
  - 인스턴스에서 외부에 접속하기 위해서는..
 

- RDS에 Public accessibility 옵션 설정 여부에 따라 End

### Security
* [Creating Your First IAM Admin User and Group](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html) : root 계정을 그대로 쓰지 말고 IAM 을 만든다
