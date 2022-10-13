# JDBC 라이브러리 구현하기
## 1단계 - JDBC 라이브러리 구현하기
- `UserDaoTest`의 모든 테스트 케이스가 통과한다.
- `UserDao`가 아닌 `JdbcTemplate` 클래스에서 JDBC와 관련된 처리를 담당하고 있다.

## 2단계 - 리팩터링 힌트
- 개발자는 SQL문 작성, 매개변수 설정에만 집중할 수 있도록 한다.
- 불필요한 중복을 줄이고 람다를 활용하여 코드량을 줄인다.

## 3단계 - Transaction 적용하기
- 트랜잭션 롤백이 적용되어 `UserServiceTest` 클래스의 `testTransactionRollback()` 테스트 케이스가 통과한다.
- 트랜잭션 서비스와 애플리케이션 서비스가 분리되었다.
