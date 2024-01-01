# Spock 란

- Groovy 언어를 이용하여 테스트 코드를 작성할 수 있는 프레임워크이며
- JUnit 과 비교하여 코드를 더 간결하게 작성 가능
  - Groovy 언어는 동적 타입 프로그래밍 언어로 JVM 위에서 동작하며 Java문법과 유사

```text
def "address 파라미터 값이 nul1이면, nequestAddresssearch 소드는 NULl을 로팅한다. "O) {
wonyong,
given:
def address = nUll
when:
def result : KakaoApiResponseDto = kakao^ddressSearchService.requestAddressSearch(address)
then:
result == null
```
- 테스트 메소드 이름을 문자열로 작성할 수 있으며 given, when, then 코드 블록을 명확히 구분
- Junit 의 경우 주석으로 블록을 구분했었고, 메소드 이름 또한 제약사항이 많이 존재


- 테스트 클래스는 Groovy 클래스로 생성하고, Specification 클래스를 상속 받는다.
- feature(테스트 메서드는) def를 이용하여 함수로 선언하며, 하나 이상 블록이 존재해야 함
- given 블록 : 테스트에 필요한 값을 준비한다.
- when 블록 : 테스트할 코드를 실행한다.
- then 블록 : when과 함께 사용하며 예외 및 결과 값을 검증한다.
- expect 블록 : then과 같으며 when을 필요로 하지 않기 때문에 간단한 테스트 및 where와
같이 사용된다.
- where 블록 : 데이터가 다르고 로직이 동일한 경우 동일한 테스트에 대한 중복 코드 제거 가능