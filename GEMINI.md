# Valstorm Python SDK - AI Context

## Project Overview
This directory contains the Python SDK for the Valstorm API. It provides typed Python classes and models for interacting with all endpoints exposed by the Valstorm backend.

## Tech Stack
- **Language:** Python 3.11+
- **Code Generation:** OpenAPI Generator (`openapi-generator-cli`)
- **HTTP/Networking:** Standard generated REST clients (urllib3)
- **Validation:** Pydantic models

## Core Architecture
- The SDK is primarily **auto-generated** from the backend OpenAPI schema.
- Models are located in `valstorm_api/models/`.
- API endpoints are grouped into classes in `valstorm_api/api/`.

## Development Guidelines
- **DO NOT** manually edit the generated files inside `valstorm_api/` unless explicitly instructed to or if you are applying a temporary patch.
- Instead of manual edits, modify the backend FastAPI routes/models to update the OpenAPI spec, and then re-run the generation script.
- Look for `git_push.sh` or `.openapi-generator-ignore` to understand generation rules.