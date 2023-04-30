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