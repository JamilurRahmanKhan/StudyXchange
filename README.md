# StudyXchange — Student Career & Academic Collaboration Platform
A **role-based Laravel web platform** that helps students navigate their academic + career journey through **Admissions**, **Community Q&A**, **Research collaboration**, **Resource groups**, **Jobs**, and **Skill assessments** — with separate dashboards for **Students**, **University admins**, **Company admins**, and a **Super admin**.

> Built as a Software Engineering course project (solo).

---

## Highlights
- **Multi-role system** (Student / University / Company / Super Admin) with role-guarded routes and dashboards  
- End-to-end modules: **Admissions**, **Q&A**, **Research Projects + Tasks + Meetings**, **Resource Spaces**, **Jobs**, **Quizzes + Descriptive Assessments**, **Career Recommendations**
- Modern Laravel stack: **Laravel 11**, **Breeze auth**, **Vite**, **TailwindCSS**
- Built-in chat capability via **Chatify** (`munafio/chatify`)

---

## Roles & Dashboards
| Role | Description | Dashboard Route |
|---|---|---|
| Normal User (Student) | Access all student modules | `/` |
| University User | Manage universities, circulars, courses, assessments | `/university-user/dashboard` |
| Company User | Post jobs & manage applicants | `/company-user/dashboard` |
| Super Admin | Platform-level admin dashboard | `/super-admin/dashboard` |

**Role values (stored in `users.role`)**
- `1` = Super Admin  
- `2` = University User  
- `3` = Normal User  
- `4` = Company User  

---

## Core Modules

### Admissions
- Browse university admission circulars
- View circular details
- **Compare universities**
- Submit admission applications
- Search/filter admissions

### Ask Question (Community Q&A)
- Post/edit/delete questions
- View details + search
- Filter feeds (e.g., newest/trending-style filters)
- Vote on questions (upvote/downvote)
- Comments + spam report flow

### Research Collaboration
- Create research projects and view project detail
- Join/request collaboration and respond to invites
- **Task management** inside projects (create/update/detail)
- **Meeting workflow** (create meeting, respond, finalize, delete)

### Resource Spaces
- Create public/private topic groups
- Join requests for private spaces + approval workflow
- Post content + edit/delete
- Post voting (upvote/downvote)
- Comments on posts
- Engagement dashboard view per space
- Blog-style posts for spaces

### Jobs
- Browse job circulars
- Search + view job detail
- Apply to jobs
- View company profile pages
- Company admin: create/manage job circulars + view applicants

### Skill Assessment
- Quiz-based assessments
- Descriptive assessments
- Submission + results views

### Career Recommendations
- Recommendations page for students (based on profile/preferences)

### Chat
- Integrated chat package: **Chatify** (`munafio/chatify`) for in-app messaging.

---

## Tech Stack
- **Backend:** Laravel 11 (PHP 8.2+)
- **Frontend:** Blade + TailwindCSS + Vite
- **Auth:** Laravel Breeze (session-based)
- **Chat:** Chatify
- **DB:** MySQL

---

## Quickstart (Local Setup)

### Requirements
- PHP **8.2+**
- Composer
- Node.js **18+**
- MySQL

### 1) Install dependencies
```bash
composer install
npm install
