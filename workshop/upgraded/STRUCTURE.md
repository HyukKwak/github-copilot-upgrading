# upgraded 폴더 파일 구조 설명

`upgraded` 폴더는 레거시 프로젝트의 모든 파일과 폴더를 복사하여 최신화 작업을 진행하는 공간입니다. 주요 파일 및 폴더 구조는 다음과 같습니다:

- MANIFEST.in: 패키징 시 포함할 파일 목록을 지정하는 설정 파일
- README.rst: 프로젝트 설명서
- distribute-0.6.10.tar.gz: 레거시 Python 패키징 도구 배포 파일
- distribute_setup.py: distribute 패키지 설치 스크립트
- setup.py: 프로젝트 설치 및 배포를 위한 설정 파일
- docs/: 프로젝트 문서 폴더
    - build/: Sphinx로 빌드된 문서 결과물
    - source/: Sphinx 문서 소스 파일 및 설정
- guachi/: 주요 Python 모듈 및 코드
    - __init__.py: guachi 모듈 초기화 파일
    - config.py: 설정 관련 코드
    - database.py: 데이터베이스 관련 코드
    - tests/: 테스트 코드 모음
        - test_configmapper.py: 설정 매핑 테스트
        - test_configurations.py: 설정 테스트
        - test_database.py: 데이터베이스 테스트
        - test_integration.py: 통합 테스트
- guachi.egg-info/: 패키지 메타데이터 정보
    - PKG-INFO, SOURCES.txt, dependency_links.txt, top_level.txt

이 폴더는 레거시 코드를 최신 Python 환경에 맞게 업그레이드하고, 테스트 및 문서화 작업을 진행하는 데 사용됩니다.