<details> 
   <summary>250702 ~ 250704 1주차</summary>

<details> 
   <summary>250702 파이썬 1일차</summary> 

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
</details>

<details> 
   <summary>250703 파이썬 2일차</summary> 

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
  </details>

<details> 
   <summary>250704 파이썬 3일차</summary> 

<u>개인사정으로 독학</u>
- 파이썬 기초 2 제어문 ~ 기초 3 데코레이터
 </details>
 
</details>


<details> 
   <summary>250707 ~ 250711 2주차</summary>
<details> 
   <summary>250707 파이썬 4일차</summary> 

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
</details>

<details> 
   <summary>250708 파이썬 5일차</summary> 

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
</details>

<details> 
   <summary>250709 파이썬 6일차</summary> 

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
</details>

<details> 
   <summary>250710 데이터분석 1일차</summary> 

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
</details>

<details> 
   <summary>250711 데이터분석 2일차</summary> 

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
</details>

</details>


<details> 
   <summary>250714 ~ 250718 3주차</summary>
   
<details> 
   <summary>250714 데이터시각화 1일차</summary> 

- **Situation** – 상황

    ***데이터분석 EDA, matplotlib, seaborn에 대한 학습***

- **Task** – 과제
아래 내용 주말까지 공부하기

        1. Box Plot( 명목형 변수 x축, 연속형 변수 y축)
            1. Five-number Summary: 5가지 주요 통계량이 시각적으로 표현됨
            2. 여러 그룹 간 데이터를 비교할 때 유용
            3. 데이터의 신뢰구간과 이상치를 빠르게 확인할 수 있음
        2. male의 iqr 범위 / female의 iqr 범위 계산해서 이상치 값 찾기 문제(male 6개, female 1개)
            - 이상치 : 1.5 * iqr(The interquartile range(3분위수-1분위수)) 을 벗어난 값
        3. Barplot, 서브플롯 그리기
        4. Scatter Plot, Count Plot, distplot, kdeplot, Violin Plot, Heatmap, Pair Plot



- **Action** – 행동
학습 내용 복습하기

        1. 질적 변수의 종류(수학적 연산결과는 아무런 의미가 없음)
            - 명목형 : 변수나 크기가 순서에 대한 의미를 부여할 수 없는 경우
            - 순서형 : 변수가 어떤 기준에 따라 순서에 의미를 부여할 수 있는 경우

        2. 양적 변수의 종류(덧셈, 뺄셈 등의 연산 가능 + 의미있음)
            - 이산형 : 변수가 취할 수 있는 값을 하나하나 셀 수 있는 경우
            - 연속형 : 변수가 구간 안의 모든 값을 가질 수 있는 경우

        3. 그래프가 여러개의 데이터를 표현할 경우, 누락된 정보가 없는지 확인해봐야함
        
        4. Histograms
            1. 양적변수(연속형 변수)를 특정 구간으로 나눠서 그 범위에 해당하는 데이터의 '빈도'를 막대그래프로 표시
            2. 양적변수의 경향성(평균 근처에 값이 몰려있는지, 얼마나 몰려있는지 같은 특징을 파악)
        
    
    

- **Result** – 결과
아래 내용을 배움

        1. EDA와 CDA
            - 탐색적 데이터 분석(EDA) : 원 데이터(Raw data)를 가지고 유연하게 데이터를 탐색하고, 데이터의 특징과 구조로부터 얻은 정보를 바탕으로 통계모형을 만드는 분석방법
            - 확증적 데이터 분석(CDA) : 가설을 설정한 후, 수집한 데이터로 가설을 평가하고 추정하는 전통적인 분석
            - 탐색적 데이터 분석(EDA: Exploratory Data Analysis)는 기술통계
            - 확증적 데이터 분석(CDA: Confirmatory Data Analysis)는 추론통계

        2. Scatter Plots(산점도)
            - 양적변수와 양적변수 사이의 상관관계를 파악 - 상관관계, 이상치의 분포
        
        3. Stack Plots
            1.횡단적 관점과 종단적 관점을 하나의 그래프에 표현할 수 있음
            2. 누적된 각 데이터의 값자체 뿐 아니라 전체 중의 비율을 함께 보고, 변화량도 확인할 수 있음
            3. 시간에 따라 변화하는 값에 사용
        4. Seaborn
            1. Matplotlib을 기반으로 다양한 색상 테마와 통계용 차트 등의 기능을 추가한 시각화 패키지
            2.함수가 쉬우며 직관적으로 결과를 확인할 수 있음
            3.seaborn은 시각화용 패키지라서 결과를 직접 보여주지 않음
</details>

<details> 
   <summary>250715 데이터시각화 2일차</summary>
   
- **Situation** – 상황

    ***데이터 분석 방법론, EDA 기초, EDA를 위한 시각화 패키지(Matplotlib, Plotly)***

- **Task** – 과제
미니 프로젝트(데이터 활용 분석 및 시각화 진행)에서 EDA 실습하기

        1. 미니 프로젝트 주제 선정 및 데이터 탐색

- **Action** – 행동
학습 내용 복습하기

        1. PLOTLY
           - 인터랙티브 그래프 생성
           - fig 객체는 기본적으로 JSON 형식으로 데이터를 그림
           - 파이썬에서 Plotly로 그림을 그리는 방법은 3가지
              1. dict 형식으로 그리는 방법
                 : 가능은 하나 섬세하게 그래프를 그리려면 복잡하여 거의 쓰이지 않음
              2. Express를 통해서 그리는 방법
                 : px를 통해 템플릿으로 그래프를 빠르게 그리기 가능 (https://plotly.com/python/plotly-express/)
              3. Graph_objects를 통해서 그리는 방법
                 : 섬세한 커스터마이징이 가능, 그래프를 겹쳐그릴 수 있음(https://plotly.com/python/reference/)

        2. Scatter Plot

        3. Line Chart
        
        4. 시계열(Time Series) 그래프

        5. Bar Charts
           - 범주형 자료에 대한 카운팅, Category나 class에 대한 비교

           - 순위형 자료에 대해 카운팅할 때

           - 여러 범주형 변수에 대한 Overlay를 확인 가능
        6. Histogram

        7. Distribution Plot

        8. Box Plot & Violin Plot

        9. 트리맵

        10. Maps
        
- **Result** – 결과
아래 내용을 배움

        1. go.Figure
           - data : 데이터에 관한 정보
           - layout : 제목, 폰트, 축, 범례 등 레이아웃 설정 정보
           - go.update_layout : fig에 레이아웃 추가 업데이트
           - go.add_trace : fig에 시각요소 추가 삽입 (subplot, map, 추가 그래프 등)
           - go.make_subplots : 다중 그래프 그리기
        2. 데이터셋 불러와서 데이터 검토하기 위한 코드
           - .info()
           - .describe(include='all')
           - .head()
           - .tail()
           - .unique()
        3. Plotly Fundamentals
           - 데이터 레이블
           - 색상 차원
           - 템플릿
           - 구성
           - 높이, 너비 및 여백 조정
           - 눈금 형식 지정
           - 글꼴, 제목, 범례 항목 및 축 제목 설정
           - 축(Axes)
           - 서브플롯(Subplots)
</details>

<details> 
   <summary>250716 ~ 250718 미니 프로젝트 및 발표(총 3일)</summary>

- **Situation** – 상황

    ***데이터 활용 분석 및 시각화 진행 (데이터를 입력받고, 해당 데이터에 적합한 방식으로 시각화한다)***

- **Task** – 과제
1. 서울시 시민행복지수 통계 데이터 전처리(출처: 서울열린데이터광장)
2. streamlit application 구현

- **Action** – 행동
1. GitHub 공용 repository 생성 및 branches 생성
2. 2020~2024년도 서울시 자치구별, 항목별 행복지수 데이터 전처리
3. Plotly로 그래프, 차트 생성(시계열 그래프, 레이더 차트)
   1. 지역별 행복도 변화량(5개년) - 항목별 꺾은선 그래프(해당 지역의 2020~2024년도 행복 지수)
   2. 원하는 자치구 행복지수 비교 - 레이더 차트를 통한 시각적 비교(항목별 5개년 평균 점수 사용)
4. 삶의 만족도 5개 항목에 대한 중요에 따른 유사한 지역 추천 시스템

- **Result** – 결과
1. GitHub : (https://github.com/beening01/happy.git)
2. Streamlit : (https://happy-disticts.streamlit.app/)
</details>

</details>


<details> 
   <summary>250721 ~ 250725 4주차</summary>

<details>
   <summary>250721 SQL 1일차</summary>

- **Situation** – 상황

    ***SQL 기초 문법과 기본 SELECT 문 및 GROUP BY, 조건문 등을 중심으로 학습***  

- **Task** – 과제  
아래 SQL 쿼리를 직접 작성하여 동작 방식 이해하기

        1. 2019년 1분기 개봉 영화 중 관객수 10만 이상인 영화의 월별/유형별 관객 소계
        2. 상/하반기 구분 후, 매출 천만 이상 영화의 월별/유형별 관객 소계
        3. 부제가 있는 영화 개수 (':' 포함)
        4. 감독이 2명 이상일 때 쉼표(,) → 슬래시(/)로 바꾸어 출력

- **Action** – 행동  
기초 SQL 명령어와 데이터 형식, DB 개념 복습

        1. SQL 언어 구조 이해 (DML, DDL, DCL, TCL)
        2. SELECT ~ FROM ~ WHERE 기본 구문 실습
        3. 집계 함수 및 GROUP BY, ORDER BY 실습
        4. WHERE절에서의 다양한 조건문 사용
        5. DISTINCT, COUNT 함수 오류 주의사항 확인

- **Result** – 결과  

        1. SQL은 인덱스가 1부터 시작하며, SELECT 쿼리의 순서 및 문법 구조를 익힘
        2. 스키마(schema)와 데이터베이스(database)의 차이(MySQL에서는 유사)
        3. 데이터 웨어하우스, 데이터 마트, 레이크의 개념 정리
        4. 정형/반정형/비정형 데이터 유형 이해
        5. GROUP BY로 집계 시, SELECT 절에 포함된 컬럼 규칙 이해

*(참고 파일: `완_01_sql연습.sql`)*
</details>


<details>
   <summary>250722 SQL 2일차</summary>

- **Situation** – 상황

    ***테이블 간 관계를 탐색하기 위한 다양한 JOIN과 서브쿼리 학습***  

- **Task** – 과제  
다양한 JOIN과 서브쿼리 실습 문제 해결

        1. NEW YORK 근무 사원의 이름과 급여 조회
        2. emp와 dept를 조인해 사원명, 부서명 조회
        3. SMITH와 동일한 부서 사원 조회 (SMITH 제외)
        4. 사원-매니저 INNER JOIN / 매니저가 NULL인 경우 포함한 LEFT JOIN
        5. 40번 부서도 결과에 포함되는 OUTER JOIN 작성
        6. 급여 등급(salgrade) 조인을 통한 등급 확인

- **Action** – 행동  
JOIN 및 서브쿼리 활용 실습

        1. EQUI JOIN, NON-EQUI JOIN, OUTER JOIN, SELF JOIN 구조 익힘
        2. FROM 절에 서브쿼리(파생 테이블), SELECT 절 스칼라 서브쿼리 실습
        3. WHERE 절의 서브쿼리에 ANY, ALL, SOME 연산자 적용 방법 확인
        4. 다중 조인 시 테이블 별칭(alias) 및 ON 조건 활용법 숙지
        5. SQL의 동작순서: FROM -> WHERE -> (GROUP BY -> HAVING) -> SELECT -> ORDER BY -> LIMIT

- **Result** – 결과  

        1. INNER JOIN은 공통 컬럼이 양쪽 테이블에 존재할 때만 결과 출력
        2. OUTER JOIN은 NULL도 포함되므로 데이터 유실 방지 가능
        3. SELF JOIN은 한 테이블 내부 관계 탐색에 매우 효과적
        4. 서브쿼리는 복잡한 조건 분리 시 가독성과 성능 개선에 유리
        5. 서브쿼리 위치에 따라 사용 가능한 연산자가 다름을 이해

*(참고 파일: `완_02_JOIN.sql`, `완_03_subquery.sql`)*
</details>


<details>
   <summary>250723 SQL 3일차</summary>

- **Situation** – 상황

    ***DML(INSERT/UPDATE/DELETE), 제약조건(INTEGRITY), 인덱스(INDEX) 등 실무 활용 중심 학습***  

- **Task** – 과제  
실제 데이터 삽입/수정/삭제 및 성능 튜닝 실습

        1. emp01 테이블 생성 및 다양한 INSERT 방식 실습
        2. UPDATE/DELETE와 TRANSACTION(트랜잭션) 처리 연습
        3. PK, FK, UNIQUE, CHECK 등 제약조건 추가 및 삭제 실습
        4. ON DELETE / ON UPDATE 옵션의 동작 방식 확인
        5. INDEX 생성/삭제 및 성능 비교

- **Action** – 행동  
테이블 생성부터 인덱스까지 전체 흐름 실습

        1. INSERT 구문: 전체 칼럼 vs 특정 칼럼 입력 실습
        2. UPDATE 구문: 조건절 포함, 연산 포함, JOIN 기반 수정
        3. DELETE vs TRUNCATE 비교 실습
        4. 트랜잭션(SAVEPOINT, ROLLBACK, COMMIT) 흐름 테스트
        5. PRIMARY KEY와 FOREIGN KEY 설정 및 조회
        6. CREATE INDEX / DROP INDEX 명령어 실습

- **Result** – 결과  

        1. DML 명령어는 COMMIT을 기준으로 반영/취소 가능
        2. 제약조건을 통해 데이터 무결성 확보 (예: NULL 제한, 참조 무결성)
        3. ON DELETE CASCADE는 부모 삭제 시 자식 데이터 자동 삭제됨
        4. 인덱스는 검색 속도를 높이지만 INSERT/UPDATE 성능에는 영향을 줄 수 있음
        5. 클러스터형 인덱스는 실제 데이터 정렬까지 변경함, 보조 인덱스는 별도 구조로 관리됨

*(참고 파일: `완_04_DML-.sql`, `완_05_INTEGRITY-.sql`, `완_06_index-.sql`)*
</details>

