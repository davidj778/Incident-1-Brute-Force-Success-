[Main Page](https://github.com/davidj778/davidj778)

# Incident 1 - Brute Force Success (Windows) - Working Incidents and Incident Response


Handle the incidents generated within Azure Sentinel, following the NIST 800-61 Incident Management Lifecycle protocol.
<p align="center">
<img src="https://i.imgur.com/5oSkomd.png" alt=""/>
</p>


<h2>Step 1: Preparation</h2>
We integrated all logs into the Log Analytics Workspace and Sentinel, along with setting up alert rules.

<h2>Step 2: Detection & Analysis</h2>

1. Set Severity, Status, Owner

![1](https://imgur.com/w3fZ1Eb.jpg)

2. View Full Details (New Experience)

![1](https://imgur.com/5k8MxTi.jpg)

3. Observe the Activity Log (for history of incident)

![1](https://imgur.com/oMjddi1.jpg)

4. Observe Entities and Incident Timelines (are they doing anything else?)

![1](https://imgur.com/jNpjcq9.jpg)

5. "Investigate" the incident and continue trying to determine the scope

![1](https://imgur.com/iTPZJEz.jpg)
![1](https://imgur.com/ATqIK3K.jpg)
![1](https://imgur.com/S3ORbbM.jpg)

6. Inspect the entities and see if there are any related events

![1](https://imgur.com/fqmo2BZ.jpg)

7. Determine legitimacy of the incident (True Positive, False Positive, etc.)

![1](https://imgur.com/2IDDJH8.jpg)
![1](https://imgur.com/mTvSWJC.jpg)

8. If True Positive, continue, if False positive, close it out


<h2>Step 3: Containment, Eradication, and Recovery</h2>

- Use the simple Incident Response PlayBook

  - CUSTOM: Brute Force SUCCESS - Windows and Linux

**Incident Description**

- This incident involves observation of potential brute force attempts against a Windows VM.

**Initial Response Actions**

- Verify the authenticity of the alert or report.

- Immediately isolate the machine and change the password of the affected user

- Identify the origin of the attacks and determine if they are attacking or involved with anything else 

- Determine how and when the attack occurred

  - Are the NSGs not being locked down? If so, check other NSGs

- Assess the potential impact of the incident.

  - What type of account was it? Permissions?

**Containment and Recovery**

- Lock down the NSG assigned to that VM/Subnet, either entirely, or to allow only necessary traffic

![1](https://imgur.com/RiAv1X5.jpg)
![1](https://imgur.com/qwJ3Si6.jpg)
![1](https://imgur.com/RiAv1X5.jpg)

- Reset the affected user's password
- Enable MFA



<h2>Step 4: Document Findings/Info and Close out the Incident in Sentinel</h2>

![1](https://imgur.com/D8S95Xu.jpg)
