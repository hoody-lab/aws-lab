# AWS Cognito

- 웹 및 모바일 앱에 대한 인증과 권한 부여, 사용자 관리 제공
- 기존의 아이디, 패스워드 방식 이외에도 여러 회사의 소셜 로그인 기능을 제공하는 서비스

## 사용자 풀(user pool)

- **사용자의 가입과 로그인을 제공**하는 사용자 저장소
- 사용자에 대한 정보를 가지고 있는 저장소 같은 역할을 한다.
- 여러 방법의 로그인 또는 회원가입을 지원한다.
- 성공적으로 사용자 인증 과정이 완료되면, Cognito는 JSON 형식의 웹 토큰(JWT)를 발행하며, **이 토큰을 사용해 특정 API에 대한 접근 보안 등 자격 증명을 수행하거나 AWS의 자격 증명으로 교환한다.**

## 자격 증명 풀(Identity Pool)

- 사용자 풀에 저장된 정보를 바탕으로 회원가입 또는 로그인에 성공한 사용자에게 **AWS 서비스에 액세스할 수 있는 권한을 부여한다.**
- 특정 사용자의 고유한 자격 증명을 만들고, 사용자에게 AWS 인프라에 대한 접근 권한을 부여할 수 있다.
- 자격 증명 풀을 이용하면 다른 AWS 서비스에 직접 접근하거나 API Gateway를 통해 서비스에 접근하도록 정의하는 권한을 가진 임시 AWS 자격 증명을 생성할 수 있다.

## 참고 자료

- [https://velog.io/@w1nu/쉽게-풀어쓴-AWS-Cognito-기초-이론](https://velog.io/@w1nu/%EC%89%BD%EA%B2%8C-%ED%92%80%EC%96%B4%EC%93%B4-AWS-Cognito-%EA%B8%B0%EC%B4%88-%EC%9D%B4%EB%A1%A0)
- https://yoo11052.tistory.com/178