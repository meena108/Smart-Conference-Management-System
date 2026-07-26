Smart Conference Management System

I built this system using Node-RED to solve a real problem I saw at technical conferences: managing speaker transitions, media playback, and live agenda updates usually needs several people juggling different tools during a live event. This system brings that into one dashboard.

It was deployed and used across three conferences in 2025, including the i-UG IBM Conference 2025 in Milton Keynes, handling real-time speaker transitions and media triggers during live events.

How it works: the system reads session data from a JSON-based schedule (speaker names, timings, media references) and uses this to drive the live event flow. As each session's scheduled time is reached, the backend triggers the corresponding actions — switching the dashboard display, cueing media playback, and updating the live agenda view — without needing manual switching between separate tools. Session state is tracked internally so the operator can see what's currently live and what's coming up next, and can manually override timing if a session runs long or short.

My role: I focused on the dashboard UI, handled live deployment at the conferences, and led troubleshooting to keep the system running reliably during events.

Acknowledgements: The core logic for this system was built by a colleague at Essist; I worked alongside them on the UI, deployment, and live operation of the system.
