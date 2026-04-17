# CodeArena — Hackathon Frontend

A complete LeetCode/HackerRank-style coding platform frontend. All UI is built and functional. Your job is to wire up the backend.

## Project Structure

```
coding-platform/
├── index.html          Landing page
├── problems.html       Problem list with filters
├── problem.html        Problem detail + code editor
├── submissions.html    Submission history
├── leaderboard.html    Global rankings
├── contests.html       Contest list
├── dashboard.html      User dashboard + heatmap
├── profile.html        User profile page
├── login.html          Login form
├── signup.html         Signup form
├── css/styles.css      All styles
├── js/script.js        All frontend logic + API stubs
└── data/problems.json  Dummy problem data
```

## Backend APIs to Implement

All TODO comments are in `js/script.js`. Key endpoints:

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/login | Authenticate user |
| POST | /api/auth/signup | Register user |
| GET | /api/problems | List problems (with filters) |
| GET | /api/problems/:id | Get single problem |
| POST | /api/run-code | Execute code against test cases |
| POST | /api/submit-code | Submit solution |
| GET | /api/submissions | Get submission history |
| GET | /api/leaderboard | Get rankings |
| GET | /api/contests | Get all contests |
| POST | /api/contests/:id/register | Register for contest |
| GET | /api/user/stats | Get user statistics |
| POST | /api/ai/hint | Get AI hint for problem |

## Running Locally

Just open `index.html` in a browser — no build step needed.

For the problems page to load JSON data, serve via a local HTTP server:
```bash
npx serve .
# or
python -m http.server 8080
```
