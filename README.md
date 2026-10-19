# greet-ci

인사말 프로그램 및 GitHub Actions CI 워크플로우 실습 저장소입니다.

## 요구사항

- Python >= 3.11
- uv

## 실행 방법

```bash
uv run --locked python greet.py Hee
uv run --locked python greet.py
```

## 테스트 및 코드 품질 검사

```bash
uv run --locked pytest -q greet.py
uv run --locked black --check greet.py
uv run --locked flake8 greet.py
uv run --locked mypy greet.py
```

## 패키지 빌드

```bash
uv build
```
