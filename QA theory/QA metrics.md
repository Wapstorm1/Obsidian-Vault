**1. Requirements Coverage**

Measures how many requirements have at least one test case linked to them.

  

Formula:

\text{Requirements Coverage} = \frac{\text{Requirements Covered by ≥1 TC}}{\text{Total Requirements}} \times 100\%

Purpose: Ensures all requirements are being tested.

Note: Does not measure test depth or quality.

---

**2. Test Execution Coverage**

Shows the percentage of planned test cases that were actually executed.

  

Formula:

\text{Test Execution Coverage} = \frac{\text{Executed TCs}}{\text{Planned TCs}} \times 100\%

Purpose: Tracks testing progress.

---

**3. Pass Rate / Fail Rate / Blocked**

- **Pass Rate**:
    
    \frac{\text{Passed TCs}}{\text{Executed TCs}} \times 100\%
    
- **Fail Rate**:
    
    \frac{\text{Failed TCs}}{\text{Executed TCs}} \times 100\%
    
- **Blocked**:
    
    \frac{\text{Blocked TCs}}{\text{Planned TCs}} \times 100\%
    
    Purpose: Monitors quality and issues during execution.
    

---

**4. Defect Density**

Measures how many defects are found per requirement.

  

Formula:

\text{Defect Density} = \frac{\text{Total Defects Found}}{\text{Number of Requirements}}

Purpose: Identifies how defect-prone the requirements are.

Unit: _Defects per Requirement_.

---

**5. Defect Removal Efficiency (DRE)**

Shows how effectively defects are removed before UAT (User Acceptance Testing).

  

Formula:

\text{DRE} = \frac{\text{Defects Found Pre-UAT}}{\text{Defects Found Pre-UAT + Defects Found in UAT}} \times 100\%

Purpose: Indicates testing effectiveness before release.

---

**6. UAT Leakage**

Percentage of defects that escaped into UAT.

  

Formula:

\text{UAT Leakage} = \frac{\text{Defects Found in UAT}}{\text{Total Defects (Pre-UAT + UAT)}} \times 100\%

Purpose: Shows missed defects during internal testing.

![[QA_Metrics_CheatSheet.pdf]]