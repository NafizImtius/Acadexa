Acadexa

Intelligent Thesis Management and Global PhD Research Companion System
A full-stack web platform that digitizes the university thesis lifecycle (supervisor discovery, thesis registration, synopsis approval, progress tracking, viva preparation) and helps students prepare for global PhD applications.

Live demo: https://acadexa-frontend.onrender.com

Built for CSE471: System Analysis and Design, BRAC University, Spring 2026 (Group 02, team of four).

The problem

Thesis management at many universities runs on email threads and disconnected spreadsheets. That causes slow synopsis approvals, no visibility into progress, and uneven supervisor workloads. Students who want to study abroad also get little structured help connecting their thesis to global research opportunities. Acadexa puts the whole workflow, and the move toward PhD applications, in one place.

Features

Students

Find supervisors with filters (availability, level, type), and read or leave anonymous reviews
Search external PhD professors by name, country or research area, bookmark them, and track applications
Submit a thesis idea, then a full synopsis once the idea is approved
Log monthly progress updates with a live progress bar and supervisor comments
Deadline tracker with a pressure score, task list and Google Calendar meeting scheduling
Viva preparation: flashcards and AI-generated questions
Global research alignment score and an AI-powered PhD readiness and gap analysis
Searchable thesis archive of past defended theses

Supervisors: approve, reject or request revisions on submissions; review student progress; publish theses to the archive.
Admins: dashboard with thesis, progress and deadline-pressure analytics; faculty workload view; final approval of thesis registrations.

Tech stack
Layer	Technology
Frontend	React, Tailwind CSS
Backend	Node.js, Express.js (REST API)
Database	MongoDB
Integrations	Google Calendar API, Cloudinary (thesis PDFs), AI model APIs
Tools	Git and GitHub, Postman (API testing), Figma (UI design), Lighthouse
Deployment	Render


Known limitations
Demo authentication. Login uses name and student ID only, with no passwords or tokens. A production version would need JWT-based authentication and encrypted credentials.
Accessibility score is 66. Lighthouse flags missing button and form labels, low colour contrast and a missing main landmark. These are planned fixes.
If the demo is on a free hosting tier, the first load can take a moment while the server wakes up.

Run locally
bash
git clone https://github.com/NafizImtius/Acadexa.git
cd Acadexa

# Backend
cd backend
npm install
npm start

# Frontend (in a new terminal)
cd frontend
npm install
npm start

Create backend/.env 
