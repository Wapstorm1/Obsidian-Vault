### **1. Risk-Based Decision — Business / Learner Impact**

**Context**

At Global Payments, I was validating discount logic in a mobile POS system where pricing errors directly affected revenue.

**Decision**

I focused testing on discount application, removal, and recalculation flows instead of broad regression.

**Tradeoff**

I intentionally skipped cosmetic UI issues and low-impact settings screens to fully explore discount edge cases.

**Impact**

I found a critical bug where a discount persisted after removing a product and could be applied repeatedly to different items. This could be abused in production and cause direct financial loss. The release was blocked until fixed.



### **2. Ownership & Influence — Raising the Quality Bar**


**Context**

While testing mobile UI updates at Global Payments, most testing was done on phones and standard tablets.

  

**Decision**

I expanded coverage to foldable devices after noticing layout issues on smaller tablets and realizing foldables expose similar adaptive UI risks.

  

**Tradeoff**

This was not in scope and required extra effort, including borrowing a device and delaying lower-priority checks.

  

**Impact**

I demonstrated broken critical UI elements on foldables, pushed for broader device coverage, and the company added dedicated devices and BrowserStack support. This permanently improved release quality.