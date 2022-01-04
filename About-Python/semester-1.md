from turtle import RawPen


num1 = 10
num2 = 20

print (num1, num2)
print('num1 =', num1, 'num2 =', num2)
print('num1=', num1,' , ' 'num2=', num2, sep='')
print('num1=%d, num2=%d' % (num1,num2))

# 2. 입력과 형 변환

num3 = int(input('num3=>'))
num4 = eval(input('num4=>'))

print('num3 + num4 =', num3+num4)

# 3. 연산자와 자료형

a = 100, 200, 300, 400
print(a)
print(a[3])


print(type(123)) # int
print(type('hello')) # str
print(type(12.2)) # float
print(type([1,2,3,4])) # List (배열) => 변경 가능
print(type((1,2,3,4))) # Tuple => 변경 불가능
print(type({10,20,30})) # Set
print(type({'a':10, 'b':20, 'c':30})) # Map (dict)
print(type(10>50)) # boolean 

# 4. if

_uname = 'hong'
_passwd = '1234'

uname = input('# 아이디를 입력하세요: ')
passwd = input('# 비밀번호를 입력하세요: ')

if((uname == _uname) and (passwd == _passwd)) :
    print('>> 로그인 성공!!')
else :
    print('>> 로그인 실패!!')
    
# 5. for 

for i in range(3):
    print('Hello World')
    
for i in range(1,4,1):
    print(i, ': Hello World')
    
for i in range(0,5,1):
    print(i)

for i in [10,20,30]:
    print(i)
    
for i in range(1,11,1):
    print(i, end=' ')
    
    
    
    
    
    
    
    
    
    
    
    
    
# 1. 변수 선언과 출력

num1 = 10
num2 = 20

print (num1, num2)
print('num1 =', num1, 'num2 =', num2)
print('num1=', num1,' , ' 'num2=', num2, sep='')
print('num1=%d, num2=%d' % (num1,num2))

# %d: 10진수(정수형)

# %f: 실수형

# %e: 지수형

# %o: 8진수

# %x: 16진수

# %u: 부호없는 10진수

# %g: 실수형 자동출력

# %p: 포인터의 주소

# %c: 하나의 문자로 출력

# %s: 문자열


# camel case & snake case

# 변수명은 문자와 숫자를 섞을 수 있지만 , 숫자가 앞에 오면 안 됩니다.

# 변수명에는 공백 사용 불가능




변수명은 영문 및 숫자만 가능

언더바 사용 가능 (공백이 안되기 때문에)

언더바는 위치에 관계없이 사용할 수 있음

변수명에 예약어를 사용할 수 없음

예약어 : 이미 파이썬 문법에 정의되어 사용되는 단어

변수명으로 예약어를 사용하면 오류 발생함

![image](https://user-images.githubusercontent.com/96330958/147997583-b79deb7f-2af6-4f0e-942f-f517620f6aa3.png)

ㄴ 오버라이딩

더하기 빼기 같은 연산자에서도 오바라이딩이 가능함 

변수의 이름만 보고도 의미를 파악할 수 있어야 함

변수의 의미가 파악되더라도 너무 길어지면 안 됨 ...




## ch3.

input() 함수
- 키보드로 입력받도록 도와주는 함수

input() 함수는 입력받은 값을 모두 문자열로 취급함
- 즉 num1, num2에 입력된 100, 200은 숫자가 아닌 문자열임 !!

```py
>>> result = num1 + num2
100200
```

정수로 변환하는 int() 함수
- input() 로 입력받은 값을 정수로 변환 !!

CLI 의 반대 > GUI ..

GUI 는 원래 어려움 / 잘하기가 쉽지 않음

운영체제의 영향을 상당히 많이 받음




## 터틀 예제 !!!

```py
import turtle as t

t.shape('arrow')
t.title('Hello Turtle')

t.forward(200)


# 프로그램이 계속 실행되어 있도록 함. 이벤트 대기 상태
scr = t.Screen()
scr.mainloop()
```

거북이 회전시키기

turtle.forward(200)

turtle.left(90) 등등 ,,




## 연산자

산술 연산자의 우선순위 !!

- 더하기와 곱하기가 동시에 나오는 경우 : 곱하기 먼저 수행

그 외 연산자

//, %, ** 

각각 나누기(몫), 나머지 값, 제곱 연산자이다 !!

## 대입 연산자

### 여러 개의 대입 연산자

콤마로 분리해서 왼쪽에 변수가 2개 이상 나올 수도 있음 

그런 경우에는 오른쪽도 반드시 콤마로 분리된 2개의 숫자, 수식, 문자열 등이 와야 함

3개 이상도 한꺼번에 나올 수 있지만 '=' 을 기준으로 왼쪽과 오른쪽의 개수가 같아야 함 ..

## 복합 연산자의 역할

변수에 값을 변경한 후에 다시 자신에게 대입함

이때 num1 = num1 + 200 은 num1 += 200 과 같은 의미 

## 비교 연산자

어떤 것이 큰지 작은지 같은지를 비교하는 연산자

비교 연산자를 단독으로 사용하는 경우는 거의 없음
- 조건문이나 반복문과 함께 사용함

True False => Boolean ! 

비교 연산자의 활용

- 변수에 들어 있는 값을 주로 사용함

## 논리 연산자

비교 연산자가 여러 번 필요할 때 사용함

`AND OR NOT`

연산자의 우선순위

![image](https://user-images.githubusercontent.com/96330958/148000266-fbce4619-271d-412e-94e6-07286f559c82.png)

## ch4.

### 데이터형과 문자열

데이터형

- 변수나 상수의 종류를 의미함
- 변수의 종류 다양함

4가지 기본 데이터형

var1 = 100
var2 = 3.14
var3 = "파이썬"
var4 = True

정수형 변수 : int
실수형 변수 : float
문자열형 변수 : str
불형 변수 : bool

type() 함수

- 변수의 종류 확인하기

정수형 
정수와 정수의 연산은 정수
정수와 실수의 연산은 실수
정수와 정수여도 나누기를 하면 실수가 나옴

# 문자열의 형태

- 큰따옴표 또는 작은따옴표로 묶어서 표현
- 문자열은 0개의 글자부터 여러 개의 글자까지 모두 문자열로 취급함

>>> var1 = ""
>>> var2 = ''

여러 줄의 문자열을 표현하기

- 큰따옴표나 작은따옴표를 3개 연속 사용해서 묶어줌

문자열 연결

- 더하기 연산자 사용

문자열끼리만 가능 !!

문자열에 숫자를 곱하는 것은 가능 => 오버라이딩

len()
- 문자열의 길이를 파악할 때 사용함

>>> var1 = "난생처음! Python"
>>> len(var1)
12

한글, 기호, 영문, 공백, 숫자까지 모두 글자로 취급함

upper(), lower()

모두 대문자, 소문자로 바꾸는 함수

isupper(), islower()

문자열이 모두 대문자냐 소문자냐 물어보는 ..

count()

문자열에서 어떤 글자가 몇 번 등장하는지 확인함

find()

문자열에서 특정 단어가 몇 번째 위치에 있는지 출력함 !

## ch5.

### 조건문

순차 구조 (기본 제어구조)

- 순차적으로 코드가 실행됨
- 가장 단순한 구조이기도 하지만, 실제로 많이 사용되는 구조이기도 함

선택 구조 (logic)

- 두 가지의 경우 중에서 어느 하나를 선택한 방향으로 코드가 실행됨
- 길에서 갈림길을 만나면 어느 한쪽으로만 가야 하는 것과 같음

반복 구조


if문
- if 조건식 :ㅣ에서 조건식이 참이라면 실행할 문장이 실행됨. 거짓이라면 그냥 프로그램 종료

num = 200
if num > 100 :
    print('어쩌구')

들여쓰기가 매우매우 중요함 ,,, Tab 키를 이용하자 

if ~ else문

- 거짓일 때 실행해야 할 문장이 따로 있을 때 사용함
- 조건식이 참이라면 문장 1을 실행하고, 그렇지 않으면 문장 2를 실행

중첩 if문

- 조건을 검사하는 과정이 2번 이상인 경우
- if문 안에 또 다른 if문이 있는 형태
- 서울에 사는 학생 중에서 25살 이상인 학생이 몇 명인지를 구하는 경우 

![image](https://user-images.githubusercontent.com/96330958/148002512-20b0c43c-b6d0-4df1-b99a-b582e8f61e30.png)

elif문

랜덤한 값 추출하기

## ch6.

### 반복문

for문의 형식

- for 변수 in range(시작값, 끝값+1, 증가값):

for i in range 를 기억해라 !

중첩 for문

- for문 안에 또 for문을 사용할 수도 있음 .. 권장 X 

while문 

- 조건식이 참인 경우에 반복함

while 문

- 강제로 증가시키는 행을 추가해야 함 => 안 하면 무한 반복 ,,

무한 반복하는 간단한 while문

![image](https://user-images.githubusercontent.com/96330958/148003961-518e4b40-1b7a-4ce4-8dae-355ca9782bb7.png)

반복문을 탈출하는 break문

- 반복문 안에서 break문을 만나면 무조건 반복문을 빠져나옴..

처음으로 돌아가는 continue문

- break문은 반복문을 빠져나가지만, 이와 달리 continue문은 남은 부분을 모두 건너뛰고, 반복문의 처음으로 돌아감 .. 권장 X




내일은 Lab 실습 .. 거북이는 제외 ..

실습 파일 압축해서 제출하면 됨 ..
