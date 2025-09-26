# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시 프로젝트(`legacy` 폴더)의 모든 파일과 디렉터리 구조를 그대로 복사하여 최신화 작업을 위한 공간입니다. 각 하위 폴더와 파일은 다음과 같은 역할을 합니다:

- `MANIFEST.in`, `README.rst`, `distribute-0.6.10.tar.gz`, `distribute_setup.py`, `setup.py`: 프로젝트 메타 정보, 설치 스크립트, 배포 관련 파일
- `docs/`: 프로젝트 문서 및 Sphinx 빌드 결과물
  - `Makefile`: 문서 빌드용 Makefile
  - `build/`: Sphinx 빌드 결과물(HTML, doctree 등)
  - `source/`: Sphinx 원본 문서 및 설정 파일
    - `_static/`: 정적 파일(css 등)
- `guachi/`: 주요 Python 모듈 및 테스트 코드
  - `__init__.py`, `config.py`, `database.py`: 핵심 모듈 파일
  - `tests/`: 단위 테스트 코드
- `guachi.egg-info/`: 패키징 정보 및 메타데이터
  - `PKG-INFO`, `SOURCES.txt`, `dependency_links.txt`, `top_level.txt`

이 폴더는 레거시 코드를 최신 Python 환경으로 업그레이드하는 실습 및 테스트를 위한 작업 공간입니다. 각 파일은 원본과 동일하게 복사되었으며, 이후 업그레이드 작업을 진행할 수 있습니다.