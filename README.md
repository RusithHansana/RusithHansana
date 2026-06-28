# Rusith Hansana

Software Engineer building scalable web, AI-powered, and interactive systems.

Focused on clean architecture, performance, and product-driven engineering.

---

## Selected Projects

### NomadAgent — AI-Powered Travel Research Agent

Cross-platform mobile application that turns natural-language trip descriptions into verified, day-by-day itineraries — researching destinations in real time and streaming progress live to the user.

Built with Flutter and a Python FastAPI backend, powered by a LangGraph agent pipeline with Google Gemini AI and Tavily web search.

Key highlights:

- Multi-step agentic pipeline (planner → researcher → extractor → compiler) orchestrated by LangGraph with full state management
- Real-time SSE streaming with bounded event history and monotonic cursor deltas for memory-safe progress updates
- Intelligent web research using Tavily with hybrid relevance scoring (confidence + destination keyword matching)
- Parallel LLM extraction via `asyncio.gather`, cutting structured venue data extraction time by ~60%
- Tiered venue verification with type-specific weight tables and cross-task deduplication
- Interactive map view with accurate coordinates, PDF export, and share sheet integration

Tech:
Flutter 3.11 · Dart · Riverpod · GoRouter · Python 3.10 · FastAPI · LangGraph · Google Gemini API · Tavily · Pydantic v2 · SSE-Starlette

Architecture focus:
Linear LangGraph state graph with bounded event buffer streaming. Clean separation of agent nodes (planner, researcher, extractor, compiler) with feature-based Flutter module structure and Riverpod state management.

[View Repo](https://github.com/RusithHansana/nomad-agent)

### BizAgent — AI-Powered Receptionist for Service Businesses

Cross-platform mobile application that provides a 24/7 AI-powered receptionist for service-based businesses, handling FAQs, lead qualification, and automated appointments.

Built with React Native and Expo, utilizing Google Gemini AI and Google Sheets for a zero-cost CRM.

Key highlights:

- AI-driven conversational booking using Gemini 2.5 Flash with structured prompt design
- Lead qualification and FAQ handling with prompt injection protection
- Zero-cost CRM integration via Google Sheets API (no database required)
- Serverless Node.js backend on Vercel with sliding-window rate limiting
- Offline resilience with local storage caching for failed synchronizations
- Modern, accessible UI using React Native Paper (Material 3)

Tech:
React Native 0.81 · Expo SDK 54 · TypeScript · Google Gemini API · Node.js · Express · Google Sheets API · Vercel

Architecture focus:
Clean separation of mobile client and serverless API layers. Implementation of service-based architecture for API communication and Context-based reactive state management.

[View Repo](https://github.com/RusithHansana/biz-agent-react-native)

---

## Technical Stack

Frontend  
React · Next.js · Flutter · TypeScript

Backend  
Node.js · Express · FastAPI · Firebase

AI & ML  
Google Gemini API · LangChain · MediaPipe

Data  
MongoDB · PostgreSQL · Firestore · Hive

Infrastructure  
Docker · GitHub Actions · CI/CD

---

## Engineering Principles

- Keep architecture predictable  
- Prefer clarity over abstraction  
- Optimize only after measurement  
- Design APIs before UI  

---

## Current Focus

- Learning Rust
- Advanced system design  
- AI integration in production workflows  
- Distributed backend architecture  
- Performance optimization  
---

## Contact

[LinkedIn](https://www.linkedin.com/in/rusith-hansana/)</br>
[Portfolio](http://www.rusithhansana.me/)</br>
[Email](rusithhansana.dev@gmail.com)
