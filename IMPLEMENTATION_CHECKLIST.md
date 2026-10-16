# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] All images accepted (JPG/PNG) up to 5 MB each
- [ ] Theme length validated
- [ ] Upload returns a job_id
- [ ] Video file < 20 MB
- [ ] Narration matches theme (manual review)
- [ ] Processing time ≤ 2 min for 5 images on a consumer GPU
- [ ] GET /jobs/{id} returns status (queued, processing, done, failed)
- [ ] When done, response includes signed URL for MP4
- [ ] Responsive layout
- [ ] Progress updates every 5 s
- [ ] Video plays in‑browser
- [ ] Initialize repo, Dockerfile, CI pipeline
- [ ] Implement /jobs endpoint and Redis queue
- [ ] Create Postgres schema
- [ ] Integrate diffusers Stable Diffusion for frame interpolation
- [ ] Store image embeddings in pgvector
- [ ] Add unit tests
- [ ] Wire LangChain LLM prompt templates
- [ ] Integrate Coqui TTS
- [ ] Combine audio with FFmpeg
- [ ] Build React upload UI
- [ ] Add polling for status
- [ ] Implement video preview
- [ ] Write integration tests, load test with 5 concurrent jobs
- [ ] Configure OpenTelemetry
- [ ] Deploy Docker Compose locally & document
- [ ] Unit tests for API input validation
- [ ] Mock worker to test queue handling
- [ ] Integration test that runs full pipeline on a sample 3‑image set
- [ ] Load test with 5 parallel jobs using Locust
- [ ] Security test: ensure only owner can download video (signed URL)
- [ ] Docker Compose for local dev (api, worker, redis, postgres)
- [ ] GitHub Actions CI builds multi‑arch image and pushes to Docker Hub
- [ ] Optional Helm chart for k8s (cloud‑agnostic)
- [ ] Expose via Nginx reverse proxy with TLS (self‑signed for demo)

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
