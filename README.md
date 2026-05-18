Company Search AppA full-stack web application that allows users to search for companies by country and name. This project consists of a React frontend integrated with Tradeshift UI components and a robust Node.js/TypeScript backend built using Object-Oriented Programming (OOP) principles and design patterns.🚀 FeaturesPart 1: Company Search PageMandatory Search Filters: Dropdown selector for countries and a text input for company names.Loading State: Simulated 1-second network delay featuring a Tradeshift UI Spinner component.Header Integration: Custom app header displaying the app-icon.svg.Part 2: Company Details ModalInteractive Results: Clicking any company from the search list opens a modal view.Detailed View: Displays comprehensive company data extracted from the search payload.Part 3: Node.js & TypeScript BackendProduction-Ready API: Replaces initial JSON file mocking with a live local server.Architecture: Formulated using TypeScript and strict Object-Oriented Programming (OOP).Design Patterns: Implements clean architectural design patterns for data routing and filtering.🛠️ Tech StackFrontendFramework: React (TypeScript)UI Component Library: Tradeshift UI (Header, Forms, Menu, Modal, Spinner)Styling: CSS3 / Tradeshift UI StylesBackendRuntime Environment: Node.jsLanguage: TypeScriptDesign Concepts: Object-Oriented Programming (OOP), Singleton Pattern, Strategy Pattern📁 Project Structuretext├── backend/
│   ├── src/
│   │   ├── controllers/     # Request handlers
│   │   ├── models/          # Data models and interfaces
│   │   ├── repositories/    # Data access layer (Singleton Pattern)
│   │   ├── services/        # Business logic & filtering (Strategy Pattern)
│   │   └── server.ts        # Express server entry point
│   ├── data/                # Source JSON files (countries.json, searchResults.json)
│   ├── tsconfig.json
│   └── package.json
│
├── frontend/
│   ├── public/              # Static assets (app-icon.svg)
│   ├── src/
│   │   ├── components/      # SearchForm, CompanyList, CompanyModal
│   │   ├── App.tsx          # Application entry point & layout
│   │   └── index.tsx
│   └── package.json
└── README.md

Use code with caution.⚙️ Installation & SetupPrerequisitesNode.js (v16 or higher)npm or yarn1. Backend SetupNavigate to the backend directory:bashcd backend
Use code with caution.Install dependencies:bashnpm install
Use code with caution.Start the development server:bashnpm run dev
Use code with caution.The backend server will run on http://localhost:5000.2. Frontend SetupNavigate to the frontend directory:bashcd ../frontend
Use code with caution.Install dependencies:bashnpm install
Use code with caution.Start the React development application:bashnpm start
Use code with caution.The application will open automatically in your browser at http://localhost:3000.📐 Architecture & Design Patterns (Backend)Singleton Pattern: Applied to the data repository layer to ensure only one instance of the JSON data controller reads from disk, optimizing memory usage.Strategy Pattern: Used for implementing decoupled search and filter algorithms. This allows the system to easily swap or scale up filtering mechanics (e.g., matching by country vs. matching by name text tokens) without modifying core controller logic.Strict Type Safety: Fully typed interfaces define the exact contracts between the data layers, network requests, and API responses.
