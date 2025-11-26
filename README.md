# Triggers-packages-work
Question 1 and question 2 
---
## 👨‍💻 Team Members
- **Baziga Nkuranga caleb : 28845**  
- **Arizewe jeniffer id**  
- **Uwabera**  
- **Gasana**  
- **Sabin Izere patience ID: 27816**  
- **Muneza PRINCE ISHIMWE id: 27816**

---
🔐 Login Security Monitoring System

A lightweight database-level security mechanism designed to detect suspicious login activity and automatically generate alerts when users exceed safe login attempt limits.

🚀 What This System Does

Tracks all login attempts (successful + failed) through a login_audit table.

Automatically detects repeated failed logins using a database trigger.

Generates security alerts when a user fails more than two times in the same session/day.

(Optional) Sends email notifications to the security team for fast response.

🎯 Why It Matters

Prevents brute-force and credential-guessing attacks.

Provides clear auditing for all login activity.

Automates early warning signals without needing external tools.

Strengthens overall system security with minimal overhead.

🧩 How It Works

App inserts each login attempt into login_audit.

Trigger checks the user’s failed attempts for the day.

If failed attempts > 2 → system inserts a record into security_alerts.

(Optional) A procedure sends out an alert email.

✔ Expected Behavior

1–2 failed attempts: only logged.

3+ failed attempts: security alert triggered and recorded.
