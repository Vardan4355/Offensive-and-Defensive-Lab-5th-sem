# Experiment 9: Hydra Password Guessing

## Aim

To perform a controlled password-guessing demonstration using Hydra in an authorized lab environment and to document the observed results through screenshots.

## Scope and Safety

This experiment was carried out only in a lab setup with consent and proper authorization. Hydra is a powerful password-cracking tool and must be used only against systems that the tester owns or has explicit permission to test.

## Requirements

- Kali Linux / Linux-based penetration testing system
- Hydra installed
- A target host or service in a lab environment
- Wordlist or username/password list
- A terminal for command execution

## Procedure

### Step 1: Launch Hydra against the target service

The first screenshot shows Hydra being executed from the terminal with the target service configured. The command is used to test authentication attempts against the lab target in a controlled environment.

![Hydra command launched in the terminal](https://github.com/4316sushil39/Offensive-and-defensive-security-COM-502-/raw/main/Exp-9/Screenshot%202026-11-13%20151222.png)

### Step 2: Attempt password guessing

The second screenshot shows the authentication attempts being processed by Hydra. It records the tool trying multiple credentials against the target service, which is the core step in password guessing.

![Hydra attempting login combinations against the target](https://github.com/4316sushil39/Offensive-and-defensive-security-COM-502-/raw/main/Exp-9/Screenshot%202026-11-13%20151312.png)

### Step 3: Confirm the successful login result

The third screenshot captures the successful result returned by Hydra. This confirms that a valid credential pair was found during the authorized lab exercise.

![Hydra result showing the recovered valid credentials](https://github.com/4316sushil39/Offensive-and-defensive-security-COM-502-/raw/main/Exp-9/Screenshot%202026-11-13%20152144.png)

## Result

The lab demonstrated the use of Hydra to test a target service using a list of possible credentials. The screenshots show the execution flow from the command launch to the successful login attempt.

## Conclusion

This experiment helped understand the workflow and impact of password guessing tools like Hydra. It also highlighted the importance of strong authentication, password policies, and layered security controls.
