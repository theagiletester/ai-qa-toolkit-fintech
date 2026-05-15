## Authentication API Test Scenarios

### Positive Cases
- Valid login request returns JWT token
- Token is returned with correct expiry time

---

### Negative Cases
- Invalid password returns 401
- Missing fields return validation error
- Malformed JSON rejected by API

---

### Security Scenarios
- Token reuse after logout is rejected
- Expired token cannot access protected endpoints
- Tampered JWT signature is rejected

---

### Rate Limiting
- Multiple login attempts trigger rate limit (429)
- Brute force attempt blocked after threshold exceeded

---

### Data Integrity
- Same credentials always generate valid session
- Session invalidation propagates across services
