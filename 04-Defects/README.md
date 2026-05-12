# Defects (Bugs Found)

## BUG_POS_004: Login Accepts Any Credentials

| Field | Details |
|-------|---------|
| **Title** | System allows login with any credentials |
| **Severity** | Medium |
| **Status** | Open |
| **Found In** | Login page |

### Steps to Reproduce
1. Type any random username (e.g., "abc")
2. Type any random password (e.g., "123")
3. Select any role
4. Click "Sign In"

### What Should Happen
System checks username and password, rejects wrong ones

### What Actually Happens
User logs in successfully no matter what they type

### Why This Matters
In a real restaurant, anyone could access the system and place fake orders

### Note
This is accepted as a "demo mode" limitation for now, but must be fixed when backend is built
