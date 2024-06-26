# 리눅스 명령어 참고서: top, ps, jobs, kill

리눅스 명령어 `top`, `ps`, `jobs`, `kill`에 대해 조사함.
![git](file:///Users/yunji/Desktop/YKrMxZePPjblD9e7LnR473n3NJXreNAY9o1mTC6oG2hoOuE2ZOH1rd8u0PYtEroty63ZLGkDZ_aEKOuoTBNRbE_daW-kwdAbgHiMD5fLlXGPzjUTHb5Lnmlp0F4Qr4b29PZcpZ396IAzZdZ3rNIUfw.svg)
## 목차
- [top](#top)
- [ps](#ps)
- [jobs](#jobs)
- [kill](#kill)

## top
`top` 명령어는 실행 중인 시스템의 동적 실시간 뷰를 제공함. 
시스템 요약 정보와 현재 리눅스 커널이 관리하는 프로세스 또는 스레드 목록을 표시함.

### 사용법
```sh
top
```
### 주요기능
- CPU, 메모리, 스왑 사용량을 포함한 시스템 요약을 표시함.
- 실시간으로 프로세스 목록을 PID, 사용자, 우선순위 등과 함께 보여줌.

## ps 
`ps` 명령어는 현재 실행 중인 프로세스의 스냅샷을 보고하는 데 사용됨. 시스템에서 실행 중인 프로세스와 관련된 정보를 제공함.

### 사용법
```sh
ps [옵션]
```

### 일반적인 옵션
- `ps -e`: 모든 프로세스를 표시함.
- `ps -f`: 전체 형식으로 출력함.
- `ps -u [사용자]`: 특정 사용자의 프로세스를 표시함.

## jobs
`jobs` 명령어는 현재 터미널 세션에서 시작된 작업의 상태를 표시함.

### 사용법
```sh
jobs [옵션]
```

### 주요기능
- 작업의 상태(실행 중, 중지됨 등)를 목록으로 보여줌.
- `fg`, `bg`, `kill` 명령어와 함께 사용할 작업 ID를 표시함.

## kill
kill 명령어는 프로세스에 신호를 보내는 명령어로, 주로 프로세스를 종료하는 데 사용됨.

### 사용법
```sh
kill [옵션] <pid>
kill -l [신호]

#사용예시
kill 1234
kill -9 1234
```

### 일반적인 신호
- `kill -9 <pid>`: 프로세스를 강제 종료합니다.
- `kill -15 <pid>`: 프로세스를 정상적으로 종료합니다.













