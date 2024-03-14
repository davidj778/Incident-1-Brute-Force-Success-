# Incident 1 - Brute Force Success (Windows) - Working Incidents and Incident Response

Handle the incidents generated within Azure Sentinel, following the NIST 800-61 Incident Management Lifecycle protocol.

<h2>Step 1: Preparation</h2>
We integrated all logs into the Log Analytics Workspace and Sentinel, along with setting up alert rules.

<h2>Step 2: Detection & Analysis</h2>

1. Set Severity, Status, Owner
2. View Full Details (New Experience)
3. Observe the Activity Log (for history of incident)
4. Observe Entities and Incident Timelines (are they doing anything else?)
5. "Investigate" the incident and continue trying to determine the scope
6. Inspect the entities and see if there are any related events
7. Determine legitimacy of the incident (True Positive, False Positive, etc.)
8. If True Positive, continue, if False positive, close it out

<h2>Step 3: Containment, Eradication, and Recovery</h2>

<h2>Step 4: Document Findings/Info and Clouse out the Incident in Sentinel</h2>

## Architecture Before Hardening / Security Controls
![Architecture Diagram](https://imgur.com/ypJkZ7U.jpg)
