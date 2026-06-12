# NyayOS — Legal Infrastructure for Citizen Rights

A case management dashboard for NGOs providing legal aid to citizens in India. Built for paralegal workers to track, manage, and generate legal documents for citizen grievances.

## What It Does

**NGO Workspace** — Paralegal dashboard to manage incoming citizen cases:
- Filter cases by issue type, urgency, and status
- View full case details with a 6-step status tracker
- Auto-generate legal documents (demand notices, complaints, applications)
- Update case status with one click
- Auto-refreshes every 30 seconds

**Citizen Case Lookup** — Self-service portal for citizens to check their own case:
- Enter phone number + access PIN (`NYAY2026`)
- View current case status, next steps, and call transcript

## Issue Types Handled

| Issue | Document Types Generated |
|---|---|
| Unpaid Salary | Salary Demand Notice, Labour Commissioner Complaint |
| FIR Refusal | Complaint to SP/DCP, Magistrate Application (S.156 CrPC) |
| Deposit Withheld | Legal Notice to Landlord, Rent Authority Complaint |
| Pension Delay | Grievance Application, Escalation Letter |

## Tech Stack

- **Frontend:** Vanilla HTML/CSS/JS — single file (`index.html`)
- **Typography:** Playfair Display (serif) + Courier New (monospace)
- **Backend:** Node.js + Express (separate repo / server)
- **API:** REST — `GET /cases`, `GET /cases/:id`, `PATCH /cases/:id/status`

## Running Locally

```bash
# Start the Express server (must be running for the frontend to work)
node server.js

# Open in browser
http://localhost:3000
