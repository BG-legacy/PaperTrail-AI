# 📄 PaperTrail AI

**AI-Powered Document Organizer and Auto-Filer**  
Built with .NET 8 + Blazor + PostgreSQL + OCR

---

## 🔧 Features

- 📂 Drag-and-drop document upload
- 🧠 AI-assisted classification (legal, receipt, warranty, etc.)
- 🔍 Full-text search across uploaded documents
- 🧾 OCR text extraction from PDFs and images
- 🏷️ Smart auto-tagging and renaming
- 🔒 Role-ready backend for future auth

---

## 🏗️ Tech Stack

- **Backend:** ASP.NET Core 8 (Web API)
- **Frontend:** Blazor WebAssembly (C#)
- **OCR:** Tesseract or Azure Computer Vision
- **Database:** PostgreSQL (via Docker)
- **Search:** LINQ-based search (Elasticsearch optional)
- **Deployment:** Docker + GitHub Actions (optional)

---

## 📁 Project Structure

/PaperTrailAI ├── PaperTrailAI.API → ASP.NET Core Web API ├── PaperTrailAI.Blazor → Blazor Frontend (WASM) ├── PaperTrailAI.Application → Use cases, DTOs ├── PaperTrailAI.Domain → Entities, enums ├── PaperTrailAI.Infrastructure → DB + Services ├── docker-compose.yml → PostgreSQL service └── README.md

---

## 🚀 Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download)
- [Docker](https://www.docker.com/)
- [Tesseract OCR](https://tesseract-ocr.github.io/)
- MongoDB Atlas or PostgreSQL installed (recommended via Docker)

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/papertrail-ai.git
cd papertrail-ai
docker-compose up -d
cd src
dotnet run --project PaperTrailAI.API
