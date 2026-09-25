# Wiki Club SATI Board Elections

Election website for Wiki Club SATI (South Asia Technical Initiative).

## Overview

This project provides a web-based platform for conducting Wiki Club SATI board elections.

The website supports:

- Candidate nominations
- Candidate selection for the voting phase
- Online voting
- Write-in candidate suggestions
- Phase-based election control
- Election results and nomination review for administrators

## Election Flow

1. **Nomination**: Members submit their details and nominate themselves for one or more positions. Nominations are stored in Google Sheets.
2. **Voting**: Final candidates are added to the Candidates sheet after reviewing nominations. Members can vote through the website and suggest additional deserving candidates.
3. **Closed**: The election no longer accepts nominations or votes.

## Board Positions

- Event Coordinator
- Technology Coordinator
- Management Coordinator
- Graphics & Branding
- Social Media
- Finance
- Content Writing

## Technology

- HTML
- CSS
- JavaScript
- Google Apps Script
- Google Sheets
- Vercel
- GitHub

## Data Flow

```text
Election Website
       |
       v
Google Apps Script
       |
       v
Google Sheets
   ├── Config
   ├── Nominations
   ├── Candidates
   └── Votes
```

## Google Sheets Structure

### Config

Controls the current election phase.

Available phases:

```text
nominate
vote
closed
```

### Nominations

Stores submitted nomination forms.

### Candidates

Stores candidates approved for the voting phase.

```text
Position | CandidateName
```

### Votes

Stores submitted ballots and write-in suggestions.

## Deployment

The frontend is deployed using Vercel.

The backend is powered by a Google Apps Script web app connected to the election Google Sheet.

## Important

Do not commit:

- Admin passwords
- Private credentials
- API keys
- Election response data
- Private Google Sheet data

## Project

**Wiki Club SATI**  
South Asia Technical Initiative
Wiki Club SATI Board Election Website
