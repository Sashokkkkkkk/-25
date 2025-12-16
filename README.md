clientsphere-crm/
├─ .gitignore
├─ .gitlab-ci.yml
├─ README.md
├─ LICENSE
│
├─ docs/
│  ├─ analysis/
│  │  ├─ competitive-analysis.md
│  │  └─ tech-stack-spec.md
│  │
│  ├─ specifications/
│  │  ├─ equipment-spec.md
│  │  ├─ api-spec.yaml
│  │  └─ product-requirements.md
│  │
│  ├─ design/
│  │  ├─ uml/
│  │  │  ├─ use-case-client.drawio
│  │  │  ├─ class-diagram.drawio
│  │  │  └─ export/
│  │  │     ├─ use-case-client.png
│  │  │     └─ class-diagram.png
│  │  └─ prototypes/
│  │
│  ├─ manuals/
│  │  ├─ user-manual.md
│  │  ├─ admin-manual.md
│  │  └─ api-reference/
│  │
│  └─ reports/
│     ├─ internship-final-report.pdf
│     └─ testing-report-16-12.md
│
├─ src/
│  ├─ frontend/
│  │  ├─ public/
│  │  │  └─ index.html
│  │  │
│  │  ├─ src/
│  │  │  ├─ components/
│  │  │  │  ├─ common/
│  │  │  │  ├─ clients/
│  │  │  │  │  ├─ ClientModal/
│  │  │  │  │  │  ├─ ClientModal.jsx
│  │  │  │  │  │  ├─ ClientModal.module.css
│  │  │  │  │  │  └─ index.js
│  │  │  │  │  ├─ ClientList.jsx
│  │  │  │  │  └─ ClientCard.jsx
│  │  │  │  └─ tickets/
│  │  │  │
│  │  │  ├─ hooks/
│  │  │  ├─ services/
│  │  │  │  └─ api.js
│  │  │  ├─ utils/
│  │  │  │  └─ validators.js
│  │  │  ├─ App.jsx
│  │  │  └─ index.js
│  │  │
│  │  ├─ package.json
│  │  └─ .env.development
│  │
│  ├─ backend/
│  │  ├─ src/
│  │  │  ├─ controllers/
│  │  │  │  ├─ clientController.js
│  │  │  │  └─ ticketController.js
│  │  │  │
│  │  │  ├─ routes/
│  │  │  │  ├─ clientRoutes.js
│  │  │  │  └─ ticketRoutes.js
│  │  │  │
│  │  │  ├─ models/
│  │  │  │  ├─ Client.js
│  │  │  │  └─ Ticket.js
│  │  │  │
│  │  │  ├─ middleware/
│  │  │  ├─ utils/
│  │  │  │  └─ reportGenerator/
│  │  │  │     ├─ ReportService.js
│  │  │  │     └─ ReportService-refactored.js
│  │  │  │
│  │  │  └─ app.js
│  │  │
│  │  └─ package.json
│  │
│  └─ shared/
│     └─ schemas/
│        └─ clientSchema.js
│
├─ tests/
│  ├─ frontend/
│  │  ├─ unit/
│  │  │  ├─ components/
│  │  │  │  └─ ClientModal.test.jsx
│  │  │  └─ utils/
│  │  │     └─ validators.test.js
│  │  │
│  │  └─ integration/
│  │     └─ clients-flow.test.js
│  │
│  ├─ backend/
│  │  ├─ unit/
│  │  │  └─ controllers/
│  │  │     └─ clientController.test.js
│  │  │
│  │  └─ integration/
│  │     └─ api/
│  │        └─ clients.test.js
│  │
│  └─ e2e/
│     └─ clients.spec.js
│
├─ postman/
│  ├─ ClientSphere_API.postman_collection.json
│  ├─ environment_test.postman_environment.json
│  └─ newman-run.sh
│
├─ docker/
│  ├─ frontend.Dockerfile
│  ├─ backend.Dockerfile
│  └─ docker-compose.yml
│
├─ scripts/
│  ├─ setup-dev-env.sh
│  ├─ run-tests.sh
│  └─ code-analysis/
│     └─ sonarqube-properties.yml
│
├─ config/
│  ├─ nginx.conf
│  ├─ eslint.config.js
│  └─ jest.config.js
│
├─ logs/
│  └─ README.md
│
└─ .github/
   └─ workflows/
      └─ ci-cd.yml
