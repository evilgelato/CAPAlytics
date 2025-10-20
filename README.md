# CAPAlytics
GitHub repo blueprint for CAPAlytics

CAPAlytics/
├─ backend/
│  ├─ app/
│  │  ├─ core/               # settings, security, logging
│  │  ├─ db/                 # models, migrations, session
│  │  ├─ schemas/            # Pydantic models
│  │  ├─ services/           # business logic (ingest, nlp, reports)
│  │  ├─ api/                # routers (v1)
│  │  ├─ utils/              # helpers (csv/xlsx, pdf, s3, email)
│  │  ├─ main.py             # FastAPI factory
│  │  └─ __init__.py
│  ├─ alembic/               # DB migrations
│  ├─ alembic.ini
│  ├─ pyproject.toml         # (or requirements.txt + setup.cfg)
│  └─ Dockerfile
├─ frontend/
│  └─ streamlit/             # MVP UI (can later replace with React)
│     ├─ app.py
│     └─ components/
├─ data_samples/
│  ├─ capax_example.xlsx
│  ├─ capa_sample.csv
│  └─ mapping_keywords.yaml  # root cause keywords → category
├─ docs/
│  ├─ api.md                 # OpenAPI + examples
│  ├─ schema.md              # ERD + tables
│  ├─ security.md            # auth, roles, data handling
│  └─ roadmap.md
├─ infra/
│  ├─ docker-compose.yml
│  ├─ nginx.conf
│  └─ deploy_example.tf      # (optional) Terraform starter
├─ tests/
│  ├─ unit/
│  └─ api/
├─ .env.example
├─ .gitignore
└─ README.md

