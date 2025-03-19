# ActionTest

# MACMORNING - BE

## IngQ Project

#### 파이썬 가상 환경 구축
##### 사전 준비
1. Python 3.11.0 버전 다운로드
    - https://www.python.org/downloads/release/python-3110/

2. uv 프로젝트 관리 툴 다운로드
    - 설치 방법 2가지(pip install VS 전역 설치)
        1. ~~`pip install uv` Python 프로젝트 내에서만 사용~~
        
        2. MacOS(전역 설치)

            brew install uv
        
        3. Window(전역 설치)

            powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"


    - __2번 또는 3번 전역 설치 진행__

        - uv 설치 후 실행 안 될 경우 환경 변수 확인

</br>

##### 가상환경 구축 및 프로젝트 실행
1. git clone을 통해 해당 repository 내용 로컬로 복사

    ```
    git clone https://github.com/JNU-econovation/MacMorning-BE.git macmorning_be
    ```

2. 해당 디렉터리로 이동

    ```
    cd macmorning_be
    ```

3. 의존성 설치 및 가상 환경 구성

    ```
    uv sync
    ```

4. 프로젝트 실행

    ```
    uv run main.py
    ```


</br></br></br>

#### 추후 계획


#### 기타 번외
---
> uv 사용법
    
     https://sigridjin.medium.com/%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EA%B0%9C%EB%B0%9C%EC%9E%90%EB%9D%BC%EB%A9%B4-uv-%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%A9%EC%8B%9C%EB%8B%A4-546d523f7178

---
> 새로운 의존성 추가하고 싶은 경우(예시)

    uv add fastapi
    uv add uvicorn --extra standard


    uv run dev
    uv applicati
---