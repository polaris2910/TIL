# TIL

다른 조들의 발표를 시청하고 만들어둔 카드게임에 추가 기능을 넣기 위해 다양한 시도 진행

TIL 강의 듣고 뒤늦게 TIL시작

카드게임 광고삽입 구현중 버그 발생. ZDK 미인식 문제로 다음과 같은 방법으로 시도
1.ZDK설치 경로 수동 지정
2.AD스크립트와 버튼 스크립트 수정 시도
3. 마지막으로 라이브러리 폴더 삭제 후 재시행 하는 방법이 성공하여 버그 해결

이후 강의 복습 진행, 추가 기능을 구현하려 했지만 코드 공부가 부족해 일부 성공하지 못함\
성공한 추가기능 - BGM변경, 이미지 변경
시도한 추가기능- 카드가 돌아가며 배열되기, 모드 제작

7/7

C# 학습 시작

| **이스케이프 시퀀스** | **설명** |
| --- | --- |
| **`\'`** | 작은따옴표(') 삽입 |
| **`\"`** | 큰따옴표(") 삽입 |
| **`\\`** | 역슬래시() 삽입 |
| **`\n`** | 새 줄(줄바꿈) 삽입 |
| **`\r`** | 현재 줄 맨 앞으로 이동 |
| **`\t`** | 탭 삽입 |
| **`\b`** | 백스페이스 삽입 |

| **자료형** | **.NET 데이타 타입** | **크기 (바이트)** | **범위** |
| --- | --- | --- | --- |
| sbyte | System.SByte | 1 | -128 ~ 127 |
| byte | System.Byte | 1 | 0 ~ 255 |
| short | System.Int16 | 2 | -32,768 ~ 32,767 |
| ushort | System.UInt16 | 2 | 0 ~ 65,535 |
| **int** | System.Int32 | 4 | -2,147,483,648 ~ 2,147,483,647 |
| uint | System.UInt32 | 4 | 0 ~ 4,294,967,295 |
| **long** | System.Int64 | 8 | -9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807 |
| ulong | System.UInt64 | 8 | 0 ~ 18,446,744,073,709,551,615 |
| **float** | System.Single | 4 | ±1.5 × 10^-45 ~ ±3.4 × 10^38 |
| **double** | System.Double | 8 | ±5.0 × 10^-324 ~ ±1.7 × 10^308 |
| decimal | System.Decimal | 16 | ±1.0 × 10^-28 ~ ±7.9 × 10^28 |
| **char** | System.Char | 2 | 유니코드 문자 |
| **string** | System.String |  | 유니코드 문자열 |
| **bool** | System.Boolean | 1 | true 또는 false |

---

산술 연산자 (Arithmetic Operators)
| 연산자 | 의미           | 예시             |
|--------|----------------|------------------|
| `+`    | 덧셈           | `a + b`          |
| `-`    | 뺄셈           | `a - b`          |
| `*`    | 곱셈           | `a * b`          |
| `/`    | 나눗셈         | `a / b`          |
| `%`    | 나머지         | `a % b`          |

---

할당 연산자 (Assignment Operators)
| 연산자 | 의미              | 예시          |
|--------|-------------------|---------------|
| `=`    | 대입              | `a = b`       |
| `+=`   | 더한 후 대입      | `a += b`      |
| `-=`   | 뺀 후 대입        | `a -= b`      |
| `*=`   | 곱한 후 대입      | `a *= b`      |
| `/=`   | 나눈 후 대입      | `a /= b`      |
| `%=`   | 나머지 후 대입    | `a %= b`      |

---

비교 연산자 (Comparison Operators)
| 연산자 | 의미           | 예시           |
|--------|----------------|----------------|
| `==`   | 같다           | `a == b`       |
| `!=`   | 같지 않다      | `a != b`       |
| `>`    | 크다           | `a > b`        |
| `<`    | 작다           | `a < b`        |
| `>=`   | 크거나 같다    | `a >= b`       |
| `<=`   | 작거나 같다    | `a <= b`       |

---

논리 연산자 (Logical Operators)
| 연산자 | 의미                  | 예시                   |
|--------|-----------------------|------------------------|
| `&&`   | 논리 AND              | `a && b`               |
| `||`   | 논리 OR               | `a || b`               |
| `!`    | 논리 NOT              | `!a`                   |

---

비트 연산자 (Bitwise Operators)
| 연산자 | 의미         | 예시         |
|--------|--------------|--------------|
| `&`    | 비트 AND     | `a & b`      |
| `|`    | 비트 OR      | `a | b`      |
| `^`    | 비트 XOR     | `a ^ b`      |
| `~`    | 비트 보수    | `~a`         |
| `<<`   | 왼쪽 시프트  | `a << 2`     |
| `>>`   | 오른쪽 시프트| `a >> 2`     |

---

증감 연산자 (Increment/Decrement)
| 연산자 | 의미           | 예시       |
|--------|----------------|------------|
| `++`   | 1 증가         | `a++`, `++a` |
| `--`   | 1 감소         | `a--`, `--a` |

---

조건 연산자 (Ternary / Null / 기타)
| 연산자     | 의미                                 | 예시                      |
|------------|--------------------------------------|---------------------------|
| `?:`       | 삼항 조건 연산자                     | `a > b ? x : y`           |
| `??`       | null 병합 연산자                     | `a ?? b`                  |
| `??=`      | null 병합 할당 연산자                 | `a ??= b`                 |
| `is`       | 형식 검사                            | `obj is string`           |
| `as`       | 형식 변환                            | `obj as string`           |
| `=>`       | 람다 식                              | `(x) => x + 1`            |
| `..`       | 범위 연산자 (C# 8.0 이상)            | `1..5`                    |
| `^`        | 인덱스 연산자 (뒤에서 n번째)         | `arr[^1]`                 |

---

형변환 연산자 (Type Conversion)
| 키워드    | 의미         | 예시              |
|-----------|--------------|-------------------|
| `(타입)`  | 명시적 변환  | `(int)3.14`       |
| `is`      | 형식 체크    | `x is int`        |
| `as`      | 형식 변환    | `x as string`     |


외울것이 너무 많다. 

틱텍토 게임 어떻게 시도해야할지 감이 안잡힌다.

과제 틱텍토 만들기에서 배열은 만들고 그 배열을 인식하는 방법을 모르겠다. 검색해서  row, col 을 알아내서 사용했다.
다시 하라하면 안보고는 못할거닽다. 암기해야한다.

7/8 3장의 상속을 이용하면 아이템 리스트를 잘 만들 수 있을거 같다. 시도해보자
3장의 강의를 들었지만 과제진행이 막혔다. 어떻게 접근해야할지 감이 안잡힌다.
과제스킵
7/8
오늘은 과제를 많이 진행했다.
 if (int.TryParse(say, out int selectedIndex) &&
     selectedIndex >= 0 && selectedIndex < Village.storeList.Count)
로 리스트의 사항을 숫자로 끌어 오는 방법 활용
7/10
반복적인 암기중

7/16
진행한 프로젝트 코드
회피율 구현,
몬스터와 플레이어 동시 작용하게 하고싶음-> 던전에 Dodge 클레스 생성해서 불러와 해결
장비 장착 해제 구현
분명 다른분이 코드에 넣어놨는데 왜 작동을 안하지???->아 순서가 잘못되있구나->해결

다른사람의 코드를 읽는데 시간이 오래걸린다. 해결방법이 없을까

코딩에서 같은 코드여도 효과가 반대로 작용하는 일이 일어난다.
90%이상의 확률로 소환되지 않음 과 10%확률로 소환은 코딩에서는 다른 말이라고 한다.

강의 1-4 진행중 오브잭트 베치에서 오브젝트 사이에 공간이 발생하는 현상 발생
오브잭트를 지정하는 과정에서 크기,위치를 실수했던 현황발견
크기,위치를 재지정해여 문제 해결

갑자기 빠르게 떨어져서 뭔가 했더니
 velocity.y *= flapforce;//이미 아래로 -이동속도를 얻고 있어서 값을 곱하면 더 빨라진다.
 velocity.y += flapforce;//+로 변경

Q .OnTriggerExit2D 명령어는 구역을 빠져나와야 작동하는데 Player에는 기둥에 닿았을때 게임오버되는 명령어가 들어있습니다. 서로 충돌해서 작동하지 않을거같은데 어떻게 작동하는 건가요?
A Player의 OnCollisionEnter2D는 Obstacle의 자녀인 top, Bottom 오브젝트의 콜라이더와 연결되있으며 Obstacle에 들어있는 OnTriggerExit2D명령어는 Obstacle의 콜라이더와 작동하기에 별개의 콜라이더로 판정됩니다.
튜터님의 질문으로 이해

Q빌드를 했는데 파란화면밖에 출력되지 않습니다. 무슨문제일까요?
A빌드 셋팅에서 씬을 추가하지 않았기에 생기는 문제입니다. 씬을 다시 확인해보세요.
씬을 잘 확인하기

7/23

this.transform.GetChild(childCount - i).gameObject;
//겟차일드는 자식 오브젝트에게 접근하는 기능, 오브젝트로 가서 다시 메쉬 등을 변경하도록 하는것이.gameObject

7/24


<img width="672" height="667" alt="image" src="https://github.com/user-attachments/assets/b2fbe2b8-4ecd-48bc-a701-34d247043395" />

OnTriggerExit2D OnTriggerEnter2D는 트리거를 작동시켰을 경우 작동하는 함수
OnTriggerStay는 비비고있을때 작동하는 함수
변수를 줄이려면 bool값을 만들고 뒤의 두 함수로 끄고 키게해서 관리하는게 안전하다.

Text Meshi pro는 컴포넌트로 찾거나 3d에 들어가있다.

GetComponentInChildren-->하나만 가져온다.
GetComponentsInChildren-->배열을 가져온다.

클레스->형태가 없음
인스텐스-> 형태가 있다.
메서드->클레스 안에 생성
클레스를 인스턴스로 지정해서 관리->객체지향

화살을 발사했는데 발사가 안되는 현상 발생
원인 규명을 위해 중단점을 잡아 문제가 되는곳을 검색해 수리 시도
찾아봤지만 원인을 찾지 못해서 튜터님께 도움을 청했다,
원인: 강의자료의 로테이트를 포지션으로 잘못 보아 포지션을 잘못 적용함+스크립트의 추가수치를 수정하지 않아 색이 투명하게 나오게됨

고블린 제작중 고블린이 화살에 맞아도 화살이 파괴되지 않음.
원인-고블린의 오브젝트 포지션이 비틀려 있어 이미지가 다른 위치에 생성됨

### 7/29 
Ref 는 변수를 바꾸지 않고 사용한다.

### 7/30
UI HP바를 어떻게 만들면 좋을까
UI슬라이더 기능이 있다! 편하다!

업적기능 제작
소리도 넣어봤다.

### 8/1
- 발생 문제 -1
- HP바 구현 문제
- 기존 접근→ HP바를 UIimage로 제작후 이미지타입을 이용해 게이지처럼 보이도록 시도
- HP바 UI를 이미지로 제작하려는데 이미지가 깨지는 현상 발생
### 해결
- HP바의 제작 방식 변경
- UIimage가 아닌 Slider기능을 이용해 이미지를 사용하지 않고 HP바 제작. 기능을 구현하였다.

발생문제 -2
백그라운드 스프라이트 사이 실금 발생
기존 접근 -> transform을 조정해 -32x 좌표로 배경이 도착시 +32좌표로 이동하는 방식으로 루프
백그라운드의 스프라이트 사이사이 실금이 생기는 현상 발행
해결
이동 매커니즘 변경
배경 좌표 도달시 64x좌표 만큼 이동하는 방식으로 변경


