# 현 회사의 기술 Nuxt 와 트랜디한 Next 로 진입할수 있는지에 대한 생각을 공유하면서 ...

KG 프로님의 의견 : 

```text
어제 형기 프로님이 리액트(넥스트) 전환 가능성이 있냐고 물어보셨는데, 갑자기 궁금해서 투표 하나 올려봅니다 ㅎㅎ 

여기 계신 프로님들은 리액트(넥스트)로 전환하길 원하시나요 아니면 뷰(넉스트)를 계속 쓰길 원하시나요?

사실상 전환 가능성이 거의 없다고 생각하지만 ㅠㅠ, 그래도 직접 개발에 참여하고 있는 FE 구성원들의 의견이 궁금하네요.

개인적인 생각이 반영된 각각 스택의 장단점을 간략히 적어보겠습니다.

리액트(NextJS)
장점1 - 압도적인 커뮤니티, 방대한 라이브러리, 한글 문서 풍부, FE의 메인스트림
장점2 - 사실상 F/E 진영은 Vercel이 주도적으로 끌고 가고 있는데, 그 Vercel이 뒤를 든든하게 받쳐주고 있는 Next
장점3 - FE 개발자 인력 수급에서 크게 영향을 끼치는 요소는 "부트캠프가 어떤 기술스택을 사용하느냐"인데, 대부분 React를 많이 가르치지 Vue를 가르치는 부트캠프는 거의 없음. React 개발자 구하기가 압도적으로 쉬우며, 이직시에도 리액트 기술스택이 유리
단점1 - 뷰에 비해 상대적으로 높은 러닝커브
다만 이 부분은 Vue3의 Composition API의 도입과 React Hooks 
때문에 약간 옛날 이야기 같기도 함

뷰 (NuxtJS)
=== 기본적으로 리액트의 장점이 뷰의 단점, 리액트의 단점이 뷰의 장점과 링크 됨 ===
장점1 - 낮은 러닝커브. Options API는 초등학생도 웹 개발을 가능하게 해줄 정도로 직관적이고 간단함.
반론: 그러나 Vue3에서는 Composition API 도입으로 상대적으로 러닝커브가 올라갔음. Options API도 호환은 되나 점점 deprecated 될 듯
장점2 - 좋은 개발자경험(DX)을 가짐. Nuxt3 올라가면서 나온 Nuxt DevTools는 아주 좋은 툴체인중 하나. Vue 진영에서 개발된 Vite, Nuxt 모두 개발자 경험 극대화를 하나의 목표로 삼고 있음
장점3 - FE의 프론티어인 리액트가 먼저 새로운 기술을 내놓으면, 뷰 진영에서는 그걸 다듬어서 적용시키기 때문에 아무래도 좀 더 보완된 소스코드가 올라갈 가능성
단점1 - 점점 작아지는 생태계와 커뮤니티. Svelete의 부상과 리액트의 아성사이에 낀 Vue. 포지션이 굉장히 애매해짐. 소, 중규모 신규 프로젝트에서는 스벨트를 안쓸 이유가 없고, 대규모 프로젝트나 레거시 프로젝트는 리액트가 대다수. 실제로 npm trends에서 비교해보면 vue vs react는 차치하더라도 nextjs vs nuxtjs는 사용자 수가 압도적으로 차이가 남. 트러블슈팅시에도 nuxt는 자료가 많이 없음..
단점2 - 단점1의 파급효과로, 채용시장에서 Vue의 입지가 작아지고 있고 인력수급이 원활하지 않음

대략 이렇게 적어봤는데 관련해서 장단점 추가할게 있으면 같이 말해봐도 좋을 것 같네요 ㅎㅎ 최대한 중립적으로 써보려고 했는데 좀 리액트에 편향되게 작성된 것 같아요. 그럼에도 Vue + Nuxt는 굉장히 훌륭하고 좋은 프로젝트라고 생각합니다. 주 메인테이너인 Evan You도 대단한 사람이구요.
```

# 음... 살짝 나.. 폭주하면서 이야기 한걸까 ??
- https://astro.build/blog/2023-web-framework-performance-report/
- FE 진영의 세계적인 기술 인기투표 를 보면서, 기회가 된다면 저 중에 당당히 인기있는 기술로 product 를 만들어 보고싶네..
- 그리고 슬며시, 조심스럽게 여쭤본다는게 기술덕후 에게 말을 건넸고 
- 효과는 대단했다...

# 본격 FE 개발자 투표가 이루어 졌다. + ( 토크토크 )

KG: 익명 투표이니까 본인 의견대로 자유롭게 투표해주세요~!

YW: 논외(?) 로 여쭤볼 게 있는데요 혹시 새로 만들어질 프로젝트가 있나요??

KG: 저희는 없긴해요~ 아마 신규 프로젝트 하더라도 React쓸 일은 없을 것 같긴합니다 ㅠ

YW: 장점이 리액트가 많기는 하지만 새로 만들어질 프로젝트가 없다면 리액트 완전 전환이 어려울 것 같다는 생각이 들더라구요 ㅜ

SS: 혹.. 혹시 다들 s.. svelte는 생각은 없으신가요?

KG: 헉 사실 맘만 같아서는 스벨트로 가고싶네요 ㅋㅋㅋ

YW: 스벨트 갠적으로 욕심나긴 하는데 회사에서 꺼내면 봉기일어날것같아서.. ㅋㅋㅋㅋㅋㅋ

SS: 요즘 스벨트 보고 있긴한데, 매력적인 것 같아서요 ㅎㅎㅎㅎ

KG: 사실 전환을 해도 점진적으로 전환을 할거라 기술적으로는 가능하긴할텐데, 결국은 구성원들과 랩장님을 설득해야되겠죠 ㅎㅎ

YW: 완벽 전환이 어렵다면 뷰 + 리액트가 남아있는 상황에서... 그것 또한 2년 뒤 레거시가 될 수도 있겠단 생각이 들더라구요

새로 만들어질 프로젝트가 있다면 각 플젝 구성원들끼리 말 맞춰서 하나로 맞추는 게 맞겠다 싶어서 여쭤봤습니다 ㅎㅎ

KG: 네 개인적으로는 이 정도 규모의 회사에서 기술스택이 섞이는 건 바람직하진 않은 것 같고, 최소한 저희 랩 내에서는 통일을 하긴 해야될 것 같네요

### 짧은 10 분정도의 의견 공유 시간이였지만, 다들 의욕이 대단했다.

워밍업 이후 조금더 의견을 나누었고 기술변경 의견을 정리하니, 아래와 같은 결론이 도출되었다.

1. 구성원들만 동의한다면 결정권자 분들을 설득하는 건 시간 문제다.
2. 회사 입장에서는 결국 리소스를 들이는거라서, 최소한의 성의는 보여야 될 것이다. 점심시간 매일 30분씩 모여서 스터디를 한다든지, 업무종료 이후에 스터디하는 모습을 보이든지
3. 구성원 분들의 생각이 더욱 중요한 것 같다. 성향에 따라서는 스터디를 꺼려하시는 분들도 계실수가 있으니..

### 정리

### 찬성
- 기술도 좋아. 
- 더 좋은 품질을 위해.
- 더 많은 인재 풀을 당길 수 있어.

### 반대
- Product 의 품질 만 를 위해 변경하는건 좀...
- 더 나은 UX/UI 의 효과를 기대할 수 있는가.
- 성향의 차이

### 결론
- 우선, 다 같이 프로토타입을 만들어 보자.
- 그러기 위해선 시간 조율이 필요한데, 필연적으로 따라오는 희생 시간이 필요하다.
- 스터디 스터디 !

### 개인적인 생각
- 역시 현실적인 어려움이 많다.
- 가령 이런것? 
  - 누구에겐 돈이라는것에 희생을 하면서 까지 벌고싶지 않은데... 돈을 벌자고 강요한다던지.
  - 등등...
- TF 팀부터 시작해보는것이 최선

### 모두를 위한 기술 변경인가, 개인을 위한 기술 변경인가 ?
이 질문에 다양한 정답이 있을 것 이라고 생각한다.
너무 현실적이면서도, 보기만해도 갈증이 일어난다.

아직은 답을 내리기 힘들것 같다.

그러나, 조금더 이부분에 대해 또 고찰하게되어 주관적인 답을 내리게 될 날에 보완할 나를 기약하며.

나 자신에게 주는 무지막지하게 어려운 숙제.. 마이너 하게라도 써주겠어 ? ㅎㅎ 

### 기술을 선택하기 전에, 현재 도메인에 필요한 기술적인 한계까지 써봤는지 