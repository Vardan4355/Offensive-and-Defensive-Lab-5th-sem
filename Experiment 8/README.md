# Experiment 8: MITRE ATT&CK Mapping

## Aim

To document an authorized security-lab exercise and review the MITRE ATT&CK Enterprise framework as a way to describe observed behavior.

## Requirements and scope

- Kali Linux with Metasploit Framework
- An isolated lab host on a private lab network
- A web browser with access to MITRE ATT&CK and ATT&CK Navigator

The practical activity was limited to an authorized private lab host. Do not test systems without explicit permission. This report summarizes the recorded result and the ATT&CK technique review; it is intended for training and documentation within a controlled lab environment.

## Theory

MITRE ATT&CK is a knowledge base for describing adversary behavior. A tactic represents an objective, while a technique describes a method that may be used to achieve it. The Enterprise matrix organizes techniques by tactic and helps map observed activity to a common taxonomy.

Two technique descriptions were reviewed during this experiment:

- [T1190: Exploit Public-Facing Application](https://attack.mitre.org/techniques/T1190/) is an Initial Access technique describing exploitation of a weakness in an Internet-facing host or system.
- [T1068: Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068/) is a Privilege Escalation technique describing exploitation of a software vulnerability to gain higher privileges on a compromised system.

These descriptions provide context for analysis, but a technique should only be reported as a match when the evidence supports its defining behavior. A private lab address alone does not show that a system was publicly exposed or that the observed activity is an actual exploitation chain.

## Procedure

### Step 1: Record the lab result

Perform the practical exercise only in the authorized, isolated lab and record the observed outcome. The screenshot shows Metasploit reporting a shell with UID 0 on a private lab host.

![Kali Linux lab result showing a root-privileged shell](Screenshot/Step1(1).png)

### Step 2: Review the ATT&CK framework

Open the MITRE ATT&CK website and review the Enterprise matrix as the reference framework for classifying observed behavior.

![MITRE ATT&CK website and Enterprise matrix](Screenshot/Step2(1).png)

### Step 3: Open ATT&CK Navigator

Open ATT&CK Navigator and locate the option to create or open an Enterprise ATT&CK layer.

![ATT&CK Navigator start page](Screenshot/Step3(1).png)

### Step 4: Select a technique in the matrix

View the Enterprise matrix in Navigator and select T1190 for review. A selection identifies a technique to examine; it does not by itself confirm that the lab activity matches it.

![Enterprise ATT&CK matrix in Navigator with T1190 selected](Screenshot/Step4(1).png)

### Step 5: Review T1190

Read the official T1190 description and note its association with Initial Access. Compare its criteria with the lab evidence before classifying the activity.

![MITRE ATT&CK technique page for T1190](Screenshot/Step5(1).png)

### Step 6: Review T1068

Read the official T1068 description and note its association with Privilege Escalation. Treat it as a possible classification only if evidence shows that privileges were elevated from a lower-privileged context.

![MITRE ATT&CK technique page for T1068](Screenshot/Step6(1).png)

## Result

The lab screenshot records a Metasploit session reporting UID 0 on a private host. The Enterprise matrix was reviewed in ATT&CK Navigator, T1190 was selected for review, and the official descriptions of T1190 and T1068 were considered to evaluate whether the observed behavior matched those ATT&CK techniques.

## Conclusion

This experiment documented a practical lab result and reviewed relevant MITRE ATT&CK techniques. ATT&CK Navigator helps organize and communicate a mapping, but conclusions should remain within the authorized scope of the lab and should be based on the actual evidence captured during the activity.
