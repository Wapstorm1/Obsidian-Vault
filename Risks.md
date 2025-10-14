# **What “risk” means**

  

Potential failure with business impact. Evaluate by **Probability × Impact**. You don’t guess randomly; you derive from requirements, dependencies, and history.

  

# **Where risks come from (5 buckets)**

1. **Product/UX**: wrong behavior, confusing flows, missing feedback.
    
2. **Security/Abuse**: enumeration, brute force, token misuse, data leakage.
    
3. **Timing/State**: expiry, lockout, concurrency, “last write wins”, race conditions.
    
4. **Dependencies**: email/SMS providers, clocks, caches, databases, 3rd parties.
    
5. **Process/Observability**: logging gaps, missing metrics, rollback paths, feature flags.
    

  

# **Deriving risks (repeatable)**

- Take each rule. Ask: **What if it’s late? wrong? missing? bypassed?**
    
- Take each dependency. Ask: **What if it’s slow? down? inconsistent?**
    
- Take each boundary. Ask: **What if it’s exactly at/just past the limit? repeated fast? concurrent?**
    
- Take each user path. Ask: **What if user switches device/timezone/network mid-flow?**