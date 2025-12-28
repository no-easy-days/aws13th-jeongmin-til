# [2025-12-28]

##  ☀️ 오늘의 목표 (Scrum)

### python 예습하기

## 📝 배운 내용 (Today I Learned)

### 변수와 자료형 (int, float, str, bool, list, dict, tuple, set)

```
## 기본 자료형

# int : 정수
x = 10

# float : 실수
x = 3.14

# str : 문자열
x = "STRING"

# bool : True / False
x = True
y = False

## 컬렉션 자료형

# list : 수정이 가능한 순차 리스트
x = [1,2,3]

# tuple : 수정이 불가능한 순차 리스트
x = [1,2,3]

# set : 순서와 중복이 없는 구조
x = {1,2,3}

# dict : key - value 구조
x = {"name" : "jeongmin", "age" : 26}
```

### 조건문과 반복문(If, for, while)

```
## if : 조건문 
if x > 0:
    print("양수")
else x == 0:
    print("0")
eles:
    print("음수")

## for : 반복문
for i in range(3):
    print(i,end=" ")

>> 0 1 2

## while : 반복문 2
count = 0
while count < 3:
    print(count,end=" ")
    count += 1

>> 0 1 2
#
```
### 함수 정의와 호출
```
## 함수 : 중복코드를 제거하고 가독성 향상을 목적으로 사용 (정의 후 재사용)

def add(a,b):
    return a + b

## 함수 호출

x = add(3, 5)
print(x)

```
  

### 기본 입출력 (input, print)

```
## 입력 : input
name = input("name : ")

## 출력 : print
print("안녕하세요 제 이름은 ", name, "입니다")
or
print(f"안녕하세요, {name}입니다")
```

### 클래스에 대하여
- 클래스란 객체를 만들기 위한 설계도
-  객체 : 실제로 만들어진 것
-  클래스 : 그 객체를 만들기위한 틀
-  예) 클래스 : 자동차, 객체 : 아반떼, 소나타
- 사용 이유 : 관련된 데이터와 기능을 하나로 묶기 위함, 코드를 재사용하기 위함, 구조화 및 유지보수를 위함

```
## 클래스 정의
class Car:
    def __init__(self, brand, model, year):
        self.brand = brand
        self.model = model
        self.year = year
        self.speed = 0   # 초기 속도

    def accelerate(self, amount):
        self.speed += amount
        print(f"{self.model} 속도 증가: {self.speed}km/h")

    def brake(self, amount):
        self.speed = max(0, self.speed - amount)
        print(f"{self.model} 감속: {self.speed}km/h")

    def info(self):
        print(f"{self.year}년식 {self.brand} {self.model} / 현재 속도: {self.speed}km/h")

## 객체 생성
 car1 = car("현대","아반떼",2023)
 car2 = car("현대","소나타",2022)

## 매서드 사용
 car1.info()
 car1.accelerate(30)
 car1.brake(15)
```
