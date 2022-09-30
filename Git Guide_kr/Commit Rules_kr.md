# 커밋 메시지가 왜 필요한가?

- 팀원들과의 커뮤니케이션
- 과거 기록의 편리한 추적
- 이슈를 함께 작성하면서 이슈와 관련된 진행 상황을 확인할 수 있습니다.

# 커밋 메시지 작성하는 방법
```
Type(타입): Subject(제목)

Body(본문)

Footer(바닥글)
```
## 타입은 무엇을 의미하나요?

- `Feat` - 새로운 기능 추가
- `Fix` - 버그 수정
- `Build` - 빌드 관련 파일 수정
- `Ci` - CI관련 설정 수정
- `Docs` - 문서 (문서 추가, 수정, 삭제)
- `Style` - 스타일 (코드 형식, 세미콜론 추가: 비즈니스 로직에 변경 없는 경우)
- `Refactor` - 코드 리팩토링
- `Test` - 테스트 (테스트 코드 추가, 수정, 삭제: 비즈니스 로직에 변경 없는 경우)
- `Chore` - 기타 변경사항 (빌드 스크립트 수정 등)

## 제목을 작성하는 방법

- 제목은 `50자를` 넘기지 않고, 마침표를 붙이지 않습니다.
- 제목에는 `commit 타입을 함께` 작성합니다.
-` 과거 시제를 사용하지 않고 명령조`로 작성합니다.
- 제목과 본문은 `한 줄 띄워 분리`합니다.
- 제목의 첫 글자는 `반드시 대문자`로 씁니다.
- 제목이나 본문에 `이슈 번호`(가 있다면) 붙여야 합니다.

예시) 
~~~
Feat: New recognition function added
~~~

## 본문을 작성하는 방법

- `선택 사항`이기에 모든 commit에 본문 내용을 작성할 필요는 없습니다.
- 한 줄에 `72자를` 넘기면 안 됩니다.
- 어떻게(How)보다 `무엇을, 왜`(What, Why)에 맞춰 작성합니다.
- 설명뿐만 아니라, commit의 이유를 작성할 때에도 씁니다.

예시)
~~~
New recognition function added
    -Reader.Js:  Added recognition function due to user requirements
~~~

## 꼬리말을 작성하는 방법

- `선택 사항`이므로 모든 commit에 꼬리말을 작성할 필요는 없습니다.
- `Issue tracker ID`를 작성할 때 사용합니다.
- `해결`: 이슈 해결 시 사용
- `관련`: 해당 commit에 관련된 이슈 번호
- `참고`: 참고할 이슈가 있는 경우 사용
 
예시)
~~~
Resolutuin : #issues number
~~~

## 실습하기
~~~
Fead: New recognition function added

New recognition function added
    -Reader.Js: Added recognition function due to user requirements

Resolutuin : #1234
~~~

## 커밋 메시지로 이슈 자동으로 닫기
> 깃허브는 커밋 메시지에 특정 키워드를 사용하면 이슈가 자동으로 종료되는 기능을 탑재하고 있습니다.   
예약어는 커밋 메시지 어느 위치는 사용 할 수 있습니다.

에시)
~~~
Keyword #issues number
~~~

### 자동 닫기 키워드 리스트

- close
- closes
- closed
- fix
- fixes
- fixed
- resolve
- resolves
- resolved

다함께 Commit 메시지 Rule에 맞는 문화를 함께 정착시켜요~~


Writer - jh park  
Email - jhparkintlot@gmail.com  
Instagram - jh_parkland  
[Homepage](https://www.jhpark.org/)