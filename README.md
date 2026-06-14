# BackEnd

2026 Techeer Summer Boot Camp — 백엔드 레포지토리

## 기술 스택

- **Python** 3.12
- **Django** 6.0

## 시작하기

```bash
python -m venv .venv          # 가상환경 생성
source .venv/bin/activate     # 활성화 (Windows: .venv\Scripts\activate)
pip install -r requirements.txt

python manage.py migrate      # DB 마이그레이션
python manage.py runserver    # 개발 서버 (http://localhost:8000)
python manage.py test         # 테스트
```

## 프로젝트 구조

```
config/        # 프로젝트 설정 (settings, urls, wsgi/asgi)
manage.py      # Django 관리 명령
requirements.txt
```

## CI

`main` 브랜치로의 push / PR 시 `.github/workflows/ci.yml`가 실행됩니다.

- `pip install -r requirements.txt`
- `python manage.py check` — 시스템 점검
- `python manage.py test` — 테스트
