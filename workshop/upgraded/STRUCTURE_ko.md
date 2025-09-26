# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시(`legacy`) 폴더의 모든 파일과 디렉터리를 복사하여 생성된 디렉터리입니다. 이 폴더는 Python 2.5 기반의 레거시 코드를 최신 Python 버전으로 업그레이드하는 작업 공간으로 사용됩니다.

## 주요 파일 및 폴더

- `MANIFEST.in`: 패키징 시 포함할 파일 목록
- `README.rst`: 프로젝트 설명서
- `distribute-0.6.10.tar.gz`: 배포 관련 압축 파일
- `distribute_setup.py`: Python 패키지 배포 스크립트
- `setup.py`: 프로젝트 설치 및 배포 스크립트
- `docs/`: 프로젝트 문서 디렉터리
    - `Makefile`: 문서 빌드용 Makefile
    - `source/`: Sphinx 기반 문서 소스 및 설정
    - `build/`: 빌드된 문서 결과물
- `guachi/`: 주요 Python 모듈 디렉터리
    - `__init__.py`: 패키지 초기화 파일
    - `config.py`: 설정 관련 코드
    - `database.py`: 데이터베이스 관련 코드
    - `tests/`: 테스트 코드 디렉터리
        - `test_configmapper.py`, `test_configurations.py`, `test_database.py`, `test_integration.py`: 각종 테스트 스크립트
- `guachi.egg-info/`: 패키지 메타데이터 디렉터리
    - `dependency_links.txt`, `PKG-INFO`, `SOURCES.txt`, `top_level.txt`: 패키지 정보 파일

## 활용 목적

- 레거시 코드를 최신 Python 환경에 맞게 수정 및 테스트
- 문서, 테스트, 배포 스크립트 등 전체 프로젝트 구조를 유지하며 업그레이드 진행
- 각 파일 및 폴더는 원본 레거시 프로젝트와 동일하게 복사되어 있으므로, 변경 전/후 비교 및 기능 검증이 용이함

---
이 폴더의 모든 파일은 레거시 프로젝트의 구조와 동일하게 복사되어 있습니다. 업그레이드 작업은 이 폴더에서 진행하세요.