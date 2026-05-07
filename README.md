# 🗂️ MRF Digitalization System

A full-stack web application built during my internship at **HS Technologies (Phils.), Inc.** that replaces paper-based Material Request Forms with a streamlined digital workflow — real-time data, role-based access, and a complete request lifecycle from submission to issuance.

[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white)](https://cloudinary.com)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)

> ⚠️ This is a private internal system. The repository is for portfolio reference — production credentials and sensitive data are not included.

---

## Overview

Before this system, material requests at HS Technologies were handled entirely on paper — prone to delays, lost forms, and no visibility into request status. This project digitizes the entire MRF lifecycle:

```
Employee submits request → Manager reviews → Approved / Denied
       ↓                                            ↓
  Pending Queue                          Approved → Issued to employee
                                         Denied  → Returned for revision → Resubmitted
```

---

## Features

### Request Management
- **Submit MRF** — employees fill out a structured form with item details, quantity, purpose, and supporting media
- **Approval workflow** — managers can approve or deny requests with remarks
- **Denial & revision flow** — denied requests are returned to the requester for revision and resubmission
- **Issuance tracking** — approved requests are marked as issued once materials are released

### Real-time Data
- All request state is synced live via **Firestore** — no page refresh needed to see status updates
- **Notification bell** — users receive in-app notifications for approvals, denials, and issuance events

### Media Uploads
- Conformers can attach supporting documents and images via **Cloudinary**
- Uploaded media is stored and linked directly to each MRF record

### Authentication & Roles
- **Firebase Auth** — secure login for all users
- Role-based access: employees see their own requests, managers see the full queue

### PDF Generation
- Issued MRFs can be exported as formatted PDF documents for physical record-keeping

### Reusable Component Architecture
- Built with modular, reusable React components following clean code standards
- Maintained with branch-based Git workflows in collaboration with a backend developer

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18 · TypeScript · JSX |
| Styling | Tailwind CSS |
| Database | Firebase Firestore |
| Auth | Firebase Authentication |
| Media Storage | Cloudinary |
| Build Tool | Vite |
| Version Control | Git · GitHub (branch-based workflow) |

---

## My Role

This project was assigned to me as a **QA Intern / Frontend Developer** at HS Technologies. I was solely responsible for the entire frontend — architecture, component design, and the full request lifecycle UI — while collaborating with a backend developer on API contracts and data structure.

Key contributions:
- Designed and built the complete MRF submission, approval, denial, and revision workflow
- Integrated Firebase Auth for role-based access control
- Set up Cloudinary media upload pipeline with real-time Firestore sync
- Implemented in-app notification system for request status events
- Built PDF generation for approved MRF records
- Maintained codebase using Git branch-based workflows with pull request reviews

---

## Screenshots

> Screenshots coming soon.

---

## What I Learned

- Structuring a real-world multi-role workflow in React with Firestore as the state backbone
- Managing complex UI state across approval/denial/revision cycles
- Collaborating on a production codebase with a backend developer using Git branching
- Integrating third-party services (Cloudinary, Firebase) in a professional environment

---

> Built by [Carl Christian Jarque](https://carl-jarque-portfolio.netlify.app) · [LinkedIn](https://linkedin.com/in/carl-jarque-6b65b63bb) · Internship @ HS Technologies (Phils.), Inc.
