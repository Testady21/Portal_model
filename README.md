# UPPAAL Scholarship Application Portal Model
This project models and verifies a Scholarship Application Portal using the UPPAAL model checker. The system simulates a real-world portal where students can log in, submit scholarship applications, view academic transcripts, and access their personal information. The model ensures correct interactions between students, the scholarship approval committee, the academic server, and the database cloud, focusing on safety and liveness properties.

# Features
Student Portal: Simulates user login, application submission (merit or merit-cum-need), transcript viewing, and personal information access, enforcing one application per session.

Server: Authenticates student credentials, routes requests, and manages application processing.

Database Cloud: Stores and retrieves academic and personal data, ensuring conflict-free access.

Approval Committee: Evaluates scholarship applications based on CGPA, approving or denying requests.

# Model Structure
Four UPPAAL templates: Student_Portal, Server, Approval_Committee, and Database_cloud.

Safety and liveness properties verified using temporal logic queries (e.g., deadlock freedom, mutual exclusion, state reachability).

Assumptions include a fixed number of students, perfect database integrity, and mutually exclusive application types per session.

# Requirements
UPPAAL model checker (latest version)
