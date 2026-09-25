# Hi, I'm Chia-Hsuan Chu

> A backend-leaning full-stack engineer who turns messy real-world workflows into reliable systems, most recently AI tools for manufacturing and a ticketing platform for city operations.

## Recent Work

### Ticketing & sign-off platform for city operations
*Go, PostgreSQL, AWS S3, Swagger*

- Built the ticket module end to end: schema, repository, handlers, draft save / submit / discard, status transition rules, assignment, and a per-change activity log
- List API with filters and tab counts; detail, photo and activity endpoints
- Concurrency-safe editing with row locks and optimistic concurrency; signer eligibility checked under a membership lock to close race conditions
- Photo attachments via presigned S3 URLs, with ownership checks, size caps and `If-Match` reads so size and bytes come from the same object version
- Comments with server-side @mention resolution, including Unicode-aware name matching
- Electronic sign-off with verification codes and sign-off history
- Permission levels with explicit `MANAGE_REQUIRED` errors, template backfill migrations, and super-admin role assignment
- Async streaming job for downloading whole folders as zip
- UUIDv7 primary keys, structured error codes, request-context logging and full Swagger coverage

### AI platform for engineering drawings (web)
*Django, React/TypeScript, Konva, React Query, YOLO, Gemini*

- Balloon inspection sheets end to end: backend API with deduplication, a dedicated editor tab, syncing balloons from drawing annotations, reordering and bulk delete
- Reworked the inspection editor UX: marquee multi-select, group drag, batch delete, and auto-detection that reuses existing annotations instead of re-running YOLO
- Customer-specific inspection report (FAI / CPK) and quotation Excel generators for seven manufacturers, including embedded drawings, conditional formatting and tolerance calculations
- Detection pipeline: LLM fallback when YOLO finds nothing in a selected area, dedup of LLM results, and a migration to Gemini 3.5 Flash
- LLM chat agent tools for importing inspection results, managing balloons, and querying price records, with a confirmation flow for AI-parsed prices
- Drawing protection: screenshot blackout on focus loss, watermarked thumbnails and downloads, and group-based download permissions
- Multi-page PDF upload with splitting and SSE-driven drawing-number conflict detection
- Bidirectional metric / imperial conversion across backend and frontend
- Image-processing service: streamed PDF pages to fix OOM on large files, and adaptive dilation so thin lines survive thumbnailing

### Local-first AI desktop assistant for manufacturers
*Electron, React/TypeScript, Python (FastAPI) sidecar, Claude Agent SDK, cadquery*

- Drawing comparison agent: 2D and multi-page PDF diff, plus STEP 3D model diff with staged progress for large parts (~140s)
- Custom title-block builder: upload a title-block image, have an LLM parse its structure, then refine it in a multi-step wizard (grid adjustment, cell merging, inline editing)
- Inspection editor with balloon multi-select, marquee selection, drag-to-reorder and cancellable detection
- Hardened the sidecar: moved blocking work off the event loop, closed PIL and PDF handle leaks, and fixed IDOR on export endpoints
- Per-company LLM usage warnings with an acknowledgement flow

### Earlier
- Real-time communication SaaS with Go/Gin, handling high-concurrency messaging with PostgreSQL, Redis and AWS SQS/Kafka
- Distributed file processing with AWS S3 and image proxy services
- AI chatbot management APIs with Redis caching

## Technical Stack

- **Backend:** Go (Gin), Python (Django, FastAPI), Node.js (Express)
- **Frontend & Desktop:** React, TypeScript, Zustand, React Query, Konva, Electron, SSE
- **AI & Vision:** Claude Agent SDK, Gemini, RAG, sqlite-vec, OpenCV, YOLO, cadquery (STEP 3D)
- **Data:** PostgreSQL, MySQL, MongoDB, Redis
- **Infrastructure:** AWS (S3, SQS), Docker, Kubernetes, Kafka, Google Cloud
- **Practices:** RESTful API design, unit & integration testing, CI/CD, code review

## Certifications
- AWS Certified AI Practitioner (2024-2027)
- AWS Certified AI Practitioner Early Adopter (2024)
- Akamai Web Performance and Offload Certification (2024)

## Languages
- Mandarin Chinese (Native)
- English (Proficient)
- German (Basic)

## Connect With Me
- Email: jiasyuanchu@gmail.com

> "The purpose of writing code is to develop software, and software brings value to society."
