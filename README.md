## Company Search App
A full-stack web application that allows users to search for companies by country and name. This project consists of a React frontend integrated with Tradeshift UI components and a robust Node.js/TypeScript backend built using Object-Oriented Programming (OOP) principles and design patterns.
------------------------------
## 🚀 Features## Part 1: Company Search Page

* Mandatory Search Filters: Dropdown selector for countries and a text input for company names.
* Loading State: Simulated 1-second network delay featuring a Tradeshift UI Spinner component.
* Header Integration: Custom app header displaying the app-icon.svg.

## Part 2: Company Details Modal

* Interactive Results: Clicking any company from the search list opens a modal view.
* Detailed View: Displays comprehensive company data extracted from the search payload.

## Part 3: Node.js & TypeScript Backend

* Production-Ready API: Replaces initial JSON file mocking with a live local server.
* Architecture: Formulated using TypeScript and strict Object-Oriented Programming (OOP).
* Design Patterns: Implements clean architectural design patterns for data routing and filtering.

------------------------------
## 🛠️ Tech Stack## Frontend

* Framework: React (TypeScript)
* UI Component Library: Tradeshift UI (Header, Forms, Menu, Modal, Spinner)
* Styling: CSS3 / Tradeshift UI Styles

## Backend

* Runtime Environment: Node.js
* Language: TypeScript
* Design Concepts: Object-Oriented Programming (OOP), Singleton Pattern, Strategy Pattern

------------------------------
## 📁 Project Structure

├── backend/
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

------------------------------
## ⚙️ Installation & Setup## Prerequisites

* Node.js (v16 or higher)
* npm or yarn

## 1. Backend Setup

   1. Navigate to the backend directory:
   
   cd backend
   
   2. Install dependencies:
   
   npm install
   
   3. Start the development server:
   
   npm run dev
   
   The backend server will run on http://localhost:5000. [1, 2] 

## 2. Frontend Setup [3] 

   1. Navigate to the frontend directory:
   
   cd ../frontend
   
   2. Install dependencies:
   
   npm install
   
   3. Start the React development application:
   
   npm start
   
   The application will open automatically in your browser at http://localhost:3000. [4, 5, 6] 

------------------------------
## 📐 Architecture & Design Patterns (Backend)

* Singleton Pattern: Applied to the data repository layer to ensure only one instance of the JSON data controller reads from disk, optimizing memory usage.
* Strategy Pattern: Used for implementing decoupled search and filter algorithms. This allows the system to easily swap or scale up filtering mechanics (e.g., matching by country vs. matching by name text tokens) without modifying core controller logic.
* Strict Type Safety: Fully typed interfaces define the exact contracts between the data layers, network requests, and API responses.

------------------------------
To help refine this document further, tell me if you need mock JSON structures added to the documentation, a list of exact API endpoints, or explicit Tradeshift UI CDN links included in the setup steps.

[1] [https://github.com](https://github.com/KelvinPhu/Project-FullStack-Employee-System-CRUD)
[2] [https://github.com](https://github.com/vipullsingh/product-listing-react)
[3] [https://github.com](https://github.com/KelvinPhu/Project-FullStack-Employee-System-CRUD)
[4] [https://github.com](https://github.com/KelvinPhu/Project-FullStack-Employee-System-CRUD)
[5] [https://github.com](https://github.com/MeerUzairWasHere/open-source-portfolio)
[6] [https://gist.github.com](https://gist.github.com/Saik0s/9af22ebcf92f67aa0ac31a396e8c2288)
