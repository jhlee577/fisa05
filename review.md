## 250702 파이썬 1일차
- **Situation** – 상황
    ***변수, 연산자, 데이터타입(자료의 형태)에 대한 학습***

- **Task** – 과제
아래 내용 관련 문제들 주말에 공부하기

        1. 연산자 사용 중 실제 오류가 생길 수 있는 부분
            - ( ) 괄호로 우선 연산해야 하는 것들을 꼭 묶기
        2. 얕은복사 / 깊은복사 (원본 훼손되면 안되는 경우 주의하기)
        3. 컨테이너 자료형 중 매핑형
        
- **Action** – 행동
학습 내용 복습하기

        1. 고정 소수점(Fixed Point)과 부동 소수점(Floating Point)
        2. 문자열 이스케이프 (\역슬래시)
        3. 논리연산 (우선순위 not > and > or)
        4. 컨테이너 자료형 중 시퀀스 형(list, tuple, range)
        5. 공통 연산자 (가변형 타입, 불가변형 타입 모두 동일하게 사용할 수 있는 연산자)

- **Result** – 결과
아래 내용을 이해함

        1. 동등비교연산(자료형, 값) / 완전항등연산(주소, 자료형, 값)
        2. 단락평가(Short Circuit Evalution) - 하나면 참이면 어차피 참이기 때문에 거기서 평가를 멈춤
        3. 가변형 타입(list) vs 불가변형 타입(tuple, range)




## 250703 파이썬 2일차
- **Situation** – 상황
    ***제어문[조건문, 반복문(while)]에 대한 학습***

- **Task** – 과제
아래 내용 관련 문제들 주말에 공부하기

        1. 조건문, 반복문에서 '가독성(짧은 줄), 실행시간 짧게, 메모리 적게' 할 수 있는 코드 작성
        2. 순서도 작성하는 방법 연습하기 (https://app.code2flow.com/)(https://draw.io)
        
- **Action** – 행동
학습 내용 복습하기

        1. 간단한 if문, 다중 조건문
        2. while 문
        3. match~case문
            - ' _ ' (언더바)는 와일드카드라고 부르고 앞에 조건들을 제외한 모든 것을 포함
            - ' | ' (OR)은 또는을 의미. 둘 중에 하나라도 만족하면 참
            - ' * ' (별)은 앞에 값을 제외하고 나머지 요소들을 모두 저장하는 변수(패킹) 앞에 붙임
- match~case문
```
match 변수 or 값:
    case 값:
        실행문
```

- **Result** – 결과
아래 내용을 이해함

        1. flag 변수 - 여러개의 조건문들이 하나의 상황에 의해서 함께 제어되어야 하는 경우
        2. := (왈러스 오퍼레이터, 바다코끼리 연산자) - 할당과 리턴을 동시에 하게 해줍니다.



## 250704 파이썬 3일차
<u>개인사정으로 독학</u>
- 파이썬 기초 2 제어문 ~ 기초 3 데코레이터


## 250707 파이썬 4일차
- **Situation** – 상황
    ***함수, 문자열 출력, 정규식에 대한 학습***

- **Task** – 과제
익숙하지 않은 내용 공부하기

        1. 정규식(Regular Expression)
            1. match()
            2. search()
            3. findall()
            4. finditer()
            - 정규식 패턴 찾기 사이트: https://regex101.com/
        
- **Action** – 행동
학습 내용 복습하기

        1. List Comprehension
        - 기존 List를 사용해서 간단히 다른 리스트를 만드는 기법
        - [(변수에 적용할 수식) for (변수) in (for문이 돌아가는 범위)]
        2. 문자열 메소드
            1. split()
            2. replace()
            3. strip()
            4. join()
            5. format()

- **Result** – 결과
아래 내용을 배움

        1. p = re.compile(r"^happy", re.I)
            - 정규식에는 raw string 표기를 습관적으로 붙여주기
        2. join은 split과 반대로 iterable 객체를 string으로 만들어줌
        3. re.sub()
            - 위치를 소괄호로 분리해서 1부터 순서대로 끊어서 부르는 그루핑과 연계해서많이 사용


## 250708 파이썬 5일차
- **Situation** – 상황
    ***모듈, 패키지, 클래스 기초에 대한 학습***

- **Task** – 과제
아래 내용 관련 문제들 주말에 공부하기

        1. 예외 응용 하기
        
- **Action** – 행동
학습 내용 복습하기

        1. 예외처리
            try:
            예외가 발생할 가능성이 있는 코드
            except:
            예외가 발생할 때 실행할 코드
            else:
            잘 실행되면 실행할 코드
            finally:
            되든 안되든 반드시 실행할 코드
        2. 코드를 작성하면서 발생할 수 있는 예외 처리 방법 2가지
            1. LBYL(Look Before You Leap)
            2. EAFP(It's Easier Ask Forgiveness Than Permission)
        3. 클래스 변수, 클래스 메서드, 인스턴스 변수, 인스턴스 메서드
        4. 예외처리시 하위예외를 먼저 작성하고 상위예외를 작성
        

- **Result** – 결과
아래 내용을 배움

        1. 모듈명.변수 or 모듈명.함수() 정도까지로 import 해서 사용하는 것을 권장(어디 출신인지 안 쓰고도 해당 함수와 변수, 클래스를 불러올 수 있지만 권장안함)
        2. 객체 지향 언어와 절차 지향 언어의 차이
        
## 250709 파이썬 6일차
- **Situation** – 상황
    ***클래스에 대한 심층 학습***

- **Task** – 과제
궁금한 부분 질문하거나 직접 해결하기

        1. 클래스 변수에 다차원 리스트(중첩 리스트) 사용했을 때 인스턴스 변수만 변경하고 싶어도 원본이 훼손됨
            - 원인 : 클래스 변수의 다차원(중첩) 리스트 객체는 모든 인스턴스가 공유하기 때문
            - 해결방법 : 깊은 복사(deepcopy)
    ```
        class Car:
        color_template = ['white', 'black', ['blue', 'silver']]

        def __init__(self, model, displacement, is_domestic):
            self.model = model
            self.displacement = displacement
            self.is_domestic = is_domestic
            import copy
            self.color = copy.deepcopy(Car.color_template)
    ```
        
- **Action** – 행동
학습 내용 복습하기

        1. 생략 가능한 정보는 디폴트 파라미터에 작성한다
        즉 꼭 입력이 필요한 정보는 디폴트 값을 주지 않는다
    ```
        def __init__(self, account, name, password, balance=0)
    ```
        2. int, bool, str, float, list, tuple, range 등 파이썬 자체 제공 클래스 외에도 사용자가 직접 새로운 클래스 만들 수 있음
        (함수도 클래스로 정의되어 있음, 파이썬은 클래스가 아닌 것이 없음)

        3. 부모클래스의 __init__()을 재사용, super() 사용해서 부모클래스 호출
    ```
        def __init__(self, is_tuned: bool = False, *args, **kwargs):
            super().__init__(*args, **kwargs)
    ```

        4. @property : 동작(함수)를 값(변수)처럼 사용하게 하는 데코레이터
            @get_pw.setter : @ property 의 짝궁인 setter
    
        

- **Result** – 결과
아래 내용을 배움

        1. 맹글링 - 파이썬에서 은닉성을 변칙처럼 구현
        2. 오버로딩
            - 클래스 내의 하나의 메소드가 여러개의 기능을 처리
            - 파이썬은 오버로딩 x
            - 연산자 오버로딩이라고 매직 메소드를 이용해서 눈속임
        3. 오버라이딩
             - 메소드를 재정의(덮어쓴다)
                - 메소드 뿐 아니라 속성도 오버라이팅
            - 부모한테 물려받은 메소드를 그대로 사용하지 않겠다는 의미
                - 자식 클래스에서 부모에게 있던 메소드를 고쳐쓰는 법
                - 상속이 되어야만 재정의 할 수 있다
                - 상속받은 메소드와 동일한 이름이어야 함




    ## 250710 데이터분석 1일차
- **Situation** – 상황
    ***NumPy에 대한 학습***

- **Task** – 과제
궁금한 부분 질문하거나 직접 해결하기

        1. reshape
        배열의 총 원소 수는 그대로 유지한 채, 배열의 차원(shape) 을 새롭게 바꿈
    ```
        arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
        reshaped3 = arr.reshape(3, 1, -1)

        reshaped3.shape: (3, 1, 4)
        [[[ 1  2  3  4]]

        [[ 5  6  7  8]]

        [[ 9 10 11 12]]]

    ```

        2. np.nan, np.inf
            - Not a Number : 브로드캐스팅이 가능한, None을 의미하는 넘파이의 객체
            - infinite : 브로드캐스팅이 가능한, 결측치와는 구분된 처리하는 과정에서 잘못된 값 등을 채워넣기 위한 넘파이 객체
        
- **Action** – 행동
학습 내용 복습하기

        1. axis
            np.append(arr, values, axis)
            1. 2차원일 때
                - 행 : axis=0
                - 열 : axis=1
            2. 3차원일 때
                - 열 : axis=2
        2. 브로드캐스팅
            Numpy에서 shape가 다른 배열 간에도 산술 연산이 가능하게 하는 메커니즘
        3. 복원, 비복원 추출
            
    ```     
             a = np.array([1, 2, 3, 4, 5])
             np.random.choice(a, size=4, replace=True) #복원

    ```
    ```
             a = np.array([1, 2, 3, 4, 5])
             np.random.choice(a, 4, replace=False)#비복원
                
    ```

- **Result** – 결과
아래 내용을 배움

        1. str으로 된 자료가 있으면 나머지도 str으로 변환하기 때문에 두 번째줄 코드처럼 str으로 된 자료가 있으면 dtype으로 형변환 명시
    ```
        np.array([1.2, '2.1', 5.5]) # 형변환 주의
        np.array([1.2, '2.1', 5.5], dtype='float') # dtype으로 형변환 명시

    ```
        2. 난수를 만드는 알고리즘을 돌리는 최초의 같은 값으로 고정해서 사용
        
    ```
        import random  # 내장 파이썬

        random.seed(3) # 코드셀에 같이 넣어주시는 게 값을 실제로 윗 셀과 같도록 하는 방법
        random.randint(1, 100)

    ```
    ```
        np.random.randint(1,2) # 넘파이 min <= x < max (2 절대 안나옴)

        rng = np.random.default_rng(3) # 씨드 인스턴스
        rng.integers(low=1, high=3, size=1) # 넘파이 min <= x < max

    ```

## 250711 데이터분석 2일차
- **Situation** – 상황
    ***Pandas에 대한 학습***

- **Task** – 과제
아래 내용 관련 문제들 주말에 공부하기

        1. Grouping Analysis

        2. Melt

        3. Pivot table

        4. Function Apply


- **Action** – 행동
학습 내용 복습하기

        1. 데이터프레임(dataframe)
            - 엑셀과 같이, 인덱스(index), 변수(column), 값(value)로 이루어진 데이터 구조
            - 판다스의 특수한 자료형
            - 2차원 자료 구조, Series가 합쳐진 형태 (Series : 1차원 배열 자료 구조, 브로드캐스팅 가능, numpy로 연산되고 관리됨)

        2. 파생변수: 이미 있는 데이터를 특정 컬럼의 조건에 따라 새로 알고싶은 형태로 파생시키는 것
            - df['over25'] = df.나이 >= 25
        3. del / drop (삭제)
            - del df['over25']
            - df.drop('지역', axis=1) # axis=0 행 / axis=1 열
        4. df을 합치기 위한 명령어
            1. merge : 중복 x, 추려서 합침
            2. concat : 
                - 행 기준 pd.concat(df, data)
                - 열 기준 pd.concat((df, data), axis=1)
                - 둘 다 가지고 있는 값만 추려서 리턴 pd.concat((df, data), join='inner')
            3. join : 조건을 걸어서 합침
    
    

- **Result** – 결과
아래 내용을 배움

        1. 기본 코드
            1. data = pd.DataFrame(data)
            2. data.info()
                : 개발자가 확인해야 자료로서의 구조를 보여줌
            3. data.describe(include='all')
                : 수집된 자료들의 경향성을 보여주기 위한 대푯값
            4. data.head(1) / data.tail(1)
                : 앞의 5줄까지 출력 / 뒤에 5줄까지 출력

        2. df2 = df.copy()
            : numpy처럼 pandas의 copy()도 deepcopy
        
        3. loc은 label 값으로 접근하고 iloc은 index 기준으로 접근
            - loc 시작인덱스 : 끝인덱스
            - iloc 시작인덱스 : 끝인덱스값 + 1
        4. 열, 행 으로 동작하는 판다스를 행, 열 순서로 동작하는 넘파이의 조건으로 가져오기 위해 loc사용
