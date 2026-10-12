**1. Testing Primary Key**

**Purpose**: Ensure no duplicate or null values are allowed in primary key columns.

**Test Cases**:

1. **Insert Duplicate Values**:
• Try to insert a record with a primary key value that already exists.
• Expected: Database rejects the entry with an error.

2. **Insert Null Value**:
• Attempt to insert a record with a null primary key.
• Expected: Database rejects the entry with an error.

3. **Verify Unique Values**:
• Insert multiple records with unique primary key values.
• Expected: All records are accepted.


**2. Testing Foreign Key**

**Purpose**: Ensure valid relationships between tables and enforce referential integrity.

**Test Cases**:

1. **Insert Record with Invalid Foreign Key**:
• Insert a record where the foreign key value doesn’t exist in the referenced table.
• Expected: Database rejects the entry.

2. **Insert Valid Foreign Key**:
• Insert a record with a foreign key value that exists in the referenced table.
• Expected: Database accepts the entry.

3. **Delete Referenced Record**:
• Try deleting a record in the parent table that is referenced by a child table.
• Expected: Database rejects the deletion (if ON DELETE is not set) or handles it per the defined action (CASCADE or SET NULL).