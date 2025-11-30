# Cybersecurity Threat Detection Expert System (Prolog)

#Project Overview
This project is an **AI-based expert system** built using **Prolog**, designed to detect common cybersecurity threats by analyzing system symptoms and behaviours.  
It uses a **knowledge-base + rule-based inference engine**, similar to how traditional AI expert systems work.

The system can detect:
- DDoS Attack  
- Brute Force Attack  
- Malware Infection  
- Ransomware Behaviour  
- Port Scanning  
- SQL Injection Attempt  

It also generates a **Risk Score (0–100)** based on symptom weights.


# Features

#Rule-Based Attack Detection  
Uses Prolog rules to match conditions like:
- High CPU usage  
- High network traffic  
- Suspicious ports  
- Failed login attempts  
- SQL error logs  
- Unknown processes  

# Knowledge Base  
Contains facts & rules that help the inference engine reason like an AI system.

# Risk Score Calculator  
Provides threat severity using weighted scoring.

# Recommendations  
Provides security suggestions after detecting the threat.

#System Architecture
1. **Input Symptoms**  
   User provides observed behaviours of the system.

2. **Knowledge Base**  
   Prolog facts and rules represent cyber attack signatures.

3. **Inference Engine**  
   Prolog matches rules to predict the attack.

4. **Risk Score Generator**  
   Calculates total risk weight.

5. **Output Module**  
   Displays:
   - Detected attack  
   - Risk score  
   - Recommended actions  

# How to Run
1. Install **SWI-Prolog**  
   https://www.swi-prolog.org/

2. Save the Prolog file as:  
   `cyber_threat_detector.pl`

3. Run in terminal:
   ```prolog
   swipl cyber_threat_detector.pl
   ```

4. Set symptoms manually:
   ```prolog
   assert(high_cpu).
   assert(repeated_failed_logins).
   ```

5. Run the detection:
   ```prolog
   detect_attack.
   ```

#Sample Output
```
Detected Attack: brute_force
Risk Score: 40
Recommendation:
- Change all passwords immediately
- Enable account lockout policy
- Enable 2FA
```


# Technologies Used
- **Prolog (SWI-Prolog)**
- Rule-based AI
- Expert system reasoning
- Knowledge representation

# Author
This project was developed as part of a **CSA / Artificial Intelligence** course to demonstrate rule-based reasoning using Prolog.

