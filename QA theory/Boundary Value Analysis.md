Boundary Value Analysis (BVA) is a **black-box testing technique** used to identify errors at the boundaries of input domains rather than within the ranges. This technique is based on the idea that errors are more likely to occur at the edges of an input range, where systems may behave unexpectedly.

**Key Features of Boundary Value Analysis**

1. **Purpose**:
• Test boundary or edge cases, which are more error-prone than values within the range.

2. **Basis**:
• Boundary conditions are tested by selecting test cases at, just below, and just above the boundaries.

3. **Common Use Cases**:
• Numerical inputs.
• Ranges of values (e.g., date, time, or quantity).
• Sequential inputs like IDs or indices.

**How to Perform Boundary Value Analysis?**

1. **Identify Input Ranges**:
• Determine the valid and invalid ranges for input values.

2. **Select Test Cases**:
• For each boundary, select:
• The lower boundary and values just below and above it.
• The upper boundary and values just below and above it.

3. **Execute and Verify**:
• Test the application with the boundary values and validate the output.

Example:

You have password functionality where password should be 8-16 characters. Using BVA we will have 5 TCs: 7, 8, 9 (or any between 8 and 16), 16 and 17. We need to check first negative, first positive, somewhere in the middle, last positive and after that first negative value. 
