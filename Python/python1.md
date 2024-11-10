Python 설치 방법 (MacBook)

1. Homebrew 설치
Homebrew는 macOS에서 패키지 설치를 쉽게 도와주는 툴입니다.

터미널을 열고 아래 명령어로 Homebrew를 설치합니다:

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    

3. Python 설치

Homebrew를 설치한 후, 아래 명령어로 Python을 설치합니다:

brew install python

설치가 완료되면, Python 버전을 확인합니다:

python3 --version

3. Python 실행

Python이 제대로 설치되었는지 확인하기 위해 Python 인터프리터를 실행합니다:

python3

Python 셸이 열리면, 간단히 print 문을 입력해 봅니다:

print("Hello, Python!")

셸에서 빠져나오려면 exit()를 입력하거나 Ctrl + D를 누릅니다.

Python 기본 문법

1. 기본 입출력

# 출력
print("Hello, World!")

# 입력
name = input("Enter your name: ")
print(f"Hello, {name}!")

2. 리스트 (List)
리스트는 Python에서 가장 많이 사용되는 자료구조 중 하나로, 여러 개의 값을 저장할 수 있습니다.
python

# 리스트 생성
fruits = ["apple", "banana", "cherry"]

# 요소 접근
print(fruits[0])  # apple

# 리스트에 요소 추가
fruits.append("orange")
print(fruits)  # ['apple', 'banana', 'cherry', 'orange']

# 리스트 컴프리헨션
squared_numbers = [x**2 for x in range(5)]
print(squared_numbers)  # [0, 1, 4, 9, 16]

3. 딕셔너리 (Dictionary)

딕셔너리는 키와 값으로 이루어진 데이터 구조입니다.
python

# 딕셔너리 생성
person = {"name": "Alice", "age": 25}

# 값 접근
print(person["name"])  # Alice

# 값 수정
person["age"] = 26

# 딕셔너리 컴프리헨션
squared_values = {x: x**2 for x in range(5)}
print(squared_values)  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}

4. 리스트 컴프리헨션 예제
리스트 컴프리헨션은 리스트를 간단하게 생성하는 문법입니다.

# 일반적인 리스트 생성
even_numbers = []
for x in range(10):
    if x % 2 == 0:
        even_numbers.append(x)

print(even_numbers)  # [0, 2, 4, 6, 8]

# 리스트 컴프리헨션 사용
even_numbers = [x for x in range(10) if x % 2 == 0]
print(even_numbers)  # [0, 2, 4, 6, 8]

5. 딕셔너리 컴프리헨션 예제
딕셔너리 컴프리헨션을 사용하면 딕셔너리를 간결하게 생성할 수 있습니다.

# 키-값 쌍으로 구성된 딕셔너리 생성
squared_dict = {x: x**2 for x in range(5)}
print(squared_dict)  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}

