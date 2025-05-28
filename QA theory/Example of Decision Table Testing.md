**Example of Decision Table Testing**

**Scenario: Testing a discount application system**

**Business Rules**:

1. If the customer is a **member** and purchases **≥ 100 units**, they get a **20% discount**.
2. If the customer is a **member** and purchases **< 100 units**, they get a **10% discount**.
3. If the customer is **not a member**, they get **no discount**, regardless of purchase quantity.

**Steps**:

1. **Identify Conditions**:
• Is the customer a member? (Yes/No)
• Quantity purchased (≥ 100 / < 100).

2. **Determine Actions**:
• Apply a 20% discount.
• Apply a 10% discount.
• No discount.

3. **Construct the Decision Table**:
 ![[Pasted image 20250107163227.png]]
4. **Define Test Cases**:

• Test Case 1: Member with ≥ 100 units → 20% discount.
• Test Case 2: Member with < 100 units → 10% discount.
• Test Case 3: Non-member with ≥ 100 units → No discount.
• Test Case 4: Non-member with < 100 units → No discount.