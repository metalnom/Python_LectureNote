---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.jpg')
marp: true
---

![bg left:60% 60%](https://www.python.org/static/community_logos/python-logo-inkscape.svg)

# **Lec_01**
### Beginning

---
## Instructor
**Jung Changdo**
* Amateur Pythonist


### References
- "데이터분석을 위한 파이썬 철저입문", 위키북스, 2019
- <데이터 사이언스 스쿨 온라인220>, 패스트캠퍼스
- <올인원 패키지: 파이썬 웹 개발>, 패스트캠퍼스

---
# Programming ?

- 컴퓨터에게 일을 시키기 위한 작업
- 게임, 웹, 앱, 자동화...


# Python ?

- 배우기 쉽다
- 무료다
- 라이브러리가 많다

---
# Set Up
- Anaconda
    - Python + 기본 라이브러리 + 많이 쓰는 라이브러리
    - 이것저것 한꺼번에 설치해주는 무료 배포판
    - https://www.anaconda.com/products/individual
    - Windows, Python 3.7, 64-Bit Graphical Installer 다운로드
    - 설치 중 'Destinaion Folder'는 'C:\Anaconda3'으로 변경
    - 'Advanced Options'에서 'Register...'를 체크

---
# Start
- Jupyter Notebook
    - 코드 작성, 실행, 문서 작성 가능
    - [Anaconda3 (64-bit)]-Anaconda Prompt 실행
    - 작업폴더 생성 후 Jupyter Notebook 실행
     ```bash
    C:\Users\[계정명]> md PythonStudy
    C:\Users\[계정명]> cd PythonStudy
    C:\Users\[계정명]\PythonStudy> Jupyter notebook
    ```

---
# Jupyter Notebook
- mode
    - 명령모드(esc) : 셀 수정할 때 사용
    - 편집모드(enter) : 셀 안의 내용을 수정할 때 사용
- 단축키
    - 셀 실행 : shift + enter
    - 셀 삭제 : (명령모드) x
    - 되돌리기 : (명령모드) z
    - 셀 생성 : (명령모드) a(위로), b(아래로)

---
# Jupyter Notebook
- Magic Command
    - 셀 내부에서 동작하는 특수명령어
    - % : 한줄의 magic command 실행
    - 자주 쓰는 magic command
        - pwd : 현재 디렉토리 경로
        - ls : 현재 디렉토리 내 파일 리스트 출력
        - whos : 현재 선언된 변수 출력
        - reset : 현재 선언된 변수 모두 삭제

---
# print()
- 기본적인 출력 함수
``` python
print('Hello World')
```
- Separator 옵션
```python
print('A', 'B', 'C', sep=' ')
print('A', 'B', 'C', sep='-')
print('A', 'B', 'C', sep='\n')
print('A', 'B', 'C', sep='\t')
```
---
# print()
- End 옵션
``` python
print('Line1')
print('Line2')
print('Line3')

print('Line1', end=' ')
print('Line2', end=' ')
print('Line3')

print('Line1', end='\t')
print('Line2', end='\t')
print('Line3')
```

---
# print()
- format
``` python
print('%s is %s' % ('Python', 'Easy'))
print('{} is {}'.format('Python', 'Easy'))
print('{0} is {1}'.format('My Name', 'Changdo'))
print('{1} is {0}'.format('My Name', 'Changdo'))
print('{var1} is not {var2}'.format(var2='Difficult', var1='Python'))

print('Num1 = %5d, Num2 = %4.2f' % (9876, 1234.5678))
print("Num1 = {0:5d}, Num2 = {1:4.2f}".format(9876, 1234.5678))
print("Num1 = {a:10d}, Num2 = {b:10.3f}".format(a=9876, b=1234.5678))
```

---
# Comments
- 주석
    - 실행하고 싶지 않은 코드 앞에 #를 입력
    - 코드에 대한 설명을 넣고 싶을 때 주로 활용
    - 단축키 : ctrl + /
``` python
#print('Hello World')
print('Goodbye')
print('See you next time.')
# 오늘 수업은 여기까지 입니다.
# 다음 수업에서는 "변수, if문" 등에 대해 공부하고,
# 간단한 메뉴판 프로그램을 만들어보겠습니다.