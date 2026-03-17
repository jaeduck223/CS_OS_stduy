📌 Source Code → Machine Code 변환 과정 (핵심 정리)
1. 프로그래밍 언어의 계층

컴퓨터 언어는 인간과 하드웨어 사이 거리에 따라 두 가지로 나뉜다.

High-level Language

예: C, C++, Java, Python

인간이 이해하기 쉬운 문법

CPU는 직접 이해할 수 없음

Low-level Language

하드웨어가 직접 이해하는 언어

CPU와 가장 가까운 계층

2. 저급 언어의 종류
Machine Code

CPU가 직접 실행하는 이진수 명령어

예: 10101010

실무에서는 16진수 표현 사용

Assembly Language

기계어를 사람이 읽기 쉽게 표현

기계어와 1:1 대응

3. 소스코드 실행 방식
Compile 방식

소스코드를 한 번에 번역하여 실행파일 생성

Source Code → Compiler → Object Code → 실행

특징

실행 속도 빠름

빌드 시 오류 검출

대표 언어

C

C++

Go

Rust

Interpret 방식

소스코드를 한 줄씩 읽으며 실행

Source Code → Interpreter → 실행

특징

개발 속도 빠름

실행 중 오류 발견

대표 언어

Python

JavaScript

Ruby

4. 컴파일 과정 (C/C++ 기준)

실제로는 다음 단계를 거친다.

Source Code
   ↓
Preprocessing
   ↓
Compilation
   ↓
Assembling
   ↓
Linking
   ↓
Executable Program
5. CPU 아키텍처 영향

같은 코드라도 CPU에 따라 결과가 달라진다.

예

x86

ARM

각 CPU는 Instruction Set Architecture (ISA) 가 다르기 때문이다.

6. Bytecode (중간 코드)

일부 언어는 중간 코드를 사용한다.

예

Language	Runtime
Java	JVM
Python	Python VM

장점

플랫폼 독립성

높은 이식성

⚙️ 전체 실행 흐름
High-level Code
        ↓
Compiler / Interpreter
        ↓
Low-level Code
        ↓
CPU Execution
        ↓
Hardware Action

✔ 핵심 개념

고급언어 → 변환 → 저급언어 → CPU 실행
