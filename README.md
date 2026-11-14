# ASTRAVITAL — Astronaut Health Intelligence (Hackathon Demo)

A responsive, browser-based prototype with a demo login, mission dashboard, simulated health check-in, rule-based alerts, browser notifications, and an AI-style health copilot.

## Run locally
1. Extract this folder.
2. Open it in VS Code.
3. Open `index.html` with the VS Code Live Server extension, or double-click `index.html`.
4. Demo login:
   - Email: `commander@astravital.demo`
   - Password: `Orbit2026!`

No build tools or package installation are required.

## Publish a public demo
You can deploy this static prototype using Netlify:
1. Create/sign in to a Netlify account.
2. Choose **Add new site → Deploy manually**.
3. Drag the extracted project folder (the folder containing `index.html`) into the deploy area.
4. Netlify will provide a public URL. Test the login and dashboard on that URL.

A public static deployment does not turn the demo login into secure production authentication. The demo credentials are visible in the client-side JavaScript and must never be used for real accounts or sensitive health information.

## Demo functionality
- Login screen and session-only demo sign-in.
- Dashboard with simulated vital signs and illustrative trend chart.
- Daily check-in form updates the dashboard.
- Rule-based alert generation and alert review.
- Browser notification permission request; notifications appear only while the page is open and permission is granted.
- AI Health Copilot uses local demonstration rules to explain current demo readings and suggest general next steps.

## Important limitations
This is not a medical device, diagnostic tool, validated AI model, or emergency alert system. All readings and thresholds are simulated/illustrative. It does not connect to sensors, persist records to a secure server, send email/SMS/push alerts to a closed browser, or provide real AI inference. It must not be used for real astronaut care.

## What is needed for a real multi-user live system
- Backend API and database with encryption, access controls, audit logs and retention policies.
- Secure authentication (e.g. Supabase Auth/Firebase Auth) with server-side authorization.
- Validated sensor/device integrations and per-astronaut clinical baselines.
- Server-side alert processing plus push/email/SMS provider integration.
- A properly hosted AI service with privacy safeguards, clinician-approved content, evaluation and clear human oversight.
- Clinical, cybersecurity, aerospace and operational validation before any real-world use.
