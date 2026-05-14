# Fintech Authentication System – AI Assisted QA (Structured)

## System Under Test
- Email + password authentication
- Multi-Factor Authentication (SMS / Authenticator app)
- Account lockout after 5 failed attempts
- Session timeout after inactivity
- Trusted device recognition

---

## Prompt Used
Generate comprehensive authentication test cases for a fintech system.

IMPORTANT: Return output strictly grouped under the following sections:
1. MFA Flows
2. Session Management
3. Account Lockout Mechanisms
4. Security & Abuse Scenarios

---

## 1. MFA Flows
- SMS MFA correct code → access granted
- SMS MFA incorrect code → access denied
- Authenticator app valid code → access granted
- Expired MFA code → rejected
- MFA retry limit exceeded → temporary block

---

## 2. Session Management
- Valid session remains active during usage
- Session timeout after inactivity logs user out
- Token expiration invalidates session
- Logout invalidates all active tokens
- Concurrent session handling across devices

---

## 3. Account Lockout Mechanisms
- 5 failed login attempts → account locked
- Locked account prevents all authentication attempts
- Unlock flow validation (email or admin reset)
- Brute force attempt triggers lockout policy

---

## 4. Security & Abuse Scenarios
- Credential stuffing attack detection
- Brute force login attempt prevention
- Token reuse after logout rejected
- Session hijacking attempt blocked
- Suspicious IP login detection (risk scenario)

---

## QA Insight
Authentication systems in fintech require risk-based testing, focusing not only on functional correctness but also on fraud prevention, session integrity, and abuse resistance.
