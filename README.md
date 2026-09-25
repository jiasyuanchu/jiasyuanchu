# Hi, I'm Chia-Hsuan Chu

> A backend-leaning full-stack engineer who turns messy real-world workflows into reliable systems, most recently AI tools for manufacturing and a ticketing platform for city operations.

## Recent Work

**Ticketing & sign-off platform for city operations** (Go, PostgreSQL, AWS S3)
- Built the ticketing backend end to end: drafts, photo attachments via presigned S3 URLs, threaded comments with server-side @mention resolution, and electronic sign-off with an audit history
- Designed permission levels and template backfills; signer eligibility is checked under a membership row lock to close race conditions
- Structured error codes, request-context logging and Swagger docs for every ticket endpoint

**AI platform for engineering drawings** (Django, React/TypeScript, Electron, Python)
- Local-first AI desktop assistant: 2D / multi-page PDF and STEP 3D drawing comparison, title-block recognition, and RAG search over engineering files
- Konva-based annotation editor: marquee multi-select, group drag, and auto-detection that syncs with existing annotations
- Customer-specific inspection-sheet and quotation Excel generators, plus bidirectional metric/imperial conversion
- Fixed OOM on large multi-page PDFs by streaming pages in the image-processing service, and cleared event-loop blocking and PIL memory leaks in the Python sidecar

**Earlier**
- Real-time communication SaaS with Go/Gin, handling high-concurrency messaging with PostgreSQL, Redis and AWS SQS/Kafka
- Distributed file processing with AWS S3 and image proxy services
- AI chatbot management APIs with Redis caching

## Technical Stack

- **Backend:** Go (Gin), Python (Django, FastAPI), Node.js (Express)
- **Frontend & Desktop:** React, TypeScript, Zustand, React Query, Konva, Electron
- **AI & Vision:** Claude Agent SDK, Gemini, RAG, sqlite-vec, OpenCV, YOLO
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
