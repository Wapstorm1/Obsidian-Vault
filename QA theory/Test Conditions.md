A **test condition** is a specific situation, input, event, or requirement that must be tested to validate system behavior. It answers the question: **“What should be tested?”**


1. **Test Conditions**
    
    – User can convert currency only between their own accounts
    
    – Conversion uses real-time exchange rates
    
    – Conversion is blocked if balance is insufficient
    
    – Fee is applied to each conversion
    
    – Converted amount must be accurately reflected in both source and destination accounts
    
2. **Exploratory Ideas**
    
    – Convert currency when exchange rate changes during the session
    
    – Try conversion during system maintenance hours
    
    – Attempt conversion with maximum decimal precision
    
    – Attempt to convert entire balance minus fee (edge case rounding)
    
    – Attempt conversion with unstable internet







Verify that [requirement/feature/aspect], when [input or situation], [expected outcome].



# **Minimal method (use every time)**

  

**Step 1 — Normalize the requirement (verb + object + invariant).**

Example: “OTP expires after 10 minutes; only the latest code is valid.”

  

**Step 2 — Derive P/N/B with a formula.**

- Positive = valid input + valid state → success outcome.
    
- Negative = invalid input or forbidden state → rejection outcome.
    
- Boundary = at the edge of the invariant → pass just before / fail at or after.
    

  

**Step 3 — Attach a hard oracle.**

Pick one: **status code**, **message text class** (generic/specific), or **system state** (email sent/not sent; lockout flag).

  

**Step 4 — Enforce one behavior per line.**

No steps, no multi-checks, no dependencies in P/N/B.






# **Pattern bank (steal these)**

  

**Existence check (registered vs unregistered)**

- P: Registered → 200 action done.
    
- N: Malformed → 400; no action.
    
- B: Registered with allowed variants (case/alias) → 200 action.
    

  

**No enumeration**

- P: Unregistered → 200 generic; no side effect.
    
- N: Any message or timing difference → defect.
    
- B: Response timing within tolerance window → indistinguishable.
    

  

**Expiry window**

- P: Submit at T−ε → accept.
    
- N: Submit at T+ε → reject.
    
- B: Submit at **exact T** → reject.
    

  

**Attempt limit / lockout**

- P: Nth wrong consumes limit; N+1 → locked.
    
- N: N−1 wrong → not locked.
    
- B: Lockout duration + ε → unlocked.
    

  

**Resend limit**

- P: K within window → all sent.
    
- N: K+1 within same window → throttled; no send.
    
- B: Next after window rolls → allowed.
    

  

**Single-use**

- P: Use once → success; immediate reuse → reject as used.
    
- N: Reuse later → reject as used.
    
- B: Incomplete token format → invalid.
    

  

**Password policy**

- P: Minimal valid string → accept.
    
- N: Violate one rule → 400; blocked.
    
- B: Exactly at min length with required classes → accept.
    

  

**Session invalidation**

- P: After reset, other session’s next call → 401.
    
- N: Old refresh token after reset → cannot mint.
    
- B: Session created between verify and reset → still invalidated.
    

  

# **Status code cheat (for this feature)**

- 200 for generic success (no enumeration).
    
- 400 for invalid input (bad email format, bad password format).
    
- 401/403 for auth constraints (post-reset token rejection).
    
- 429 for throttle.
    
- 423 or 403 for lockout.
    
    Pick one scheme and be consistent.