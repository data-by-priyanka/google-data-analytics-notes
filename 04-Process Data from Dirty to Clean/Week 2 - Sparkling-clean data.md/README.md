# Dirty Data vs Clean Data

**Dirty data** is incomplete, incorrect, inconsistent, duplicated, or irrelevant data.

**Clean data** is accurate, complete, consistent, and aligned with the business objective.

Good analysis depends on clean data.

---

## Related Roles

**Data Engineers**
- Build and maintain data infrastructure
- Transform raw data into usable formats
- Manage databases and processing systems

**Data Warehousing Specialists**
- Design storage systems
- Ensure data availability and backup
- Maintain data security

---

## Null Values

A **null** indicates that a value does not exist in a dataset.

Null values must be handled carefully during analysis.

---

# Types of Dirty Data

### Duplicate Data
Same record appears multiple times.

Causes:
- Manual entry
- Batch imports
- Migration errors

Impact:
- Inflated counts
- Misleading metrics

---

### Outdated Data
Old information that should be updated.

Impact:
- Incorrect insights
- Poor decision-making

---

### Incomplete Data
Missing important fields.

Impact:
- Inaccurate analysis
- Reduced productivity

---

### Incorrect Data
Data that exists but contains errors.

Causes:
- Human error
- Fake or test entries

Impact:
- Faulty conclusions
- Financial loss

---

### Inconsistent Data
Different formats used for the same information.

Example:
- "USA" vs "United States"

Impact:
- Classification errors
- Confusion in segmentation

---

# Data Validation

**Data validation** checks accuracy before importing or using data.

Tools include:
- Field length restrictions
- Format checks
- Drop-down lists
- Controlled input types

A **field** is a single data value in a row or column.

---

# Data Merging

**Data merging** combines multiple datasets into one.

Challenges:
- Misaligned formats
- Inconsistent naming
- Duplicate entries
- Different cleaning standards

---

## Questions Before Merging

- Do I have all required data?
- Are datasets cleaned consistently?
- Are formats compatible?
- Will merging create redundancy?

---

# Common Data Cleaning Pitfalls

- Ignoring spelling errors
- Failing to document corrections
- Overlooking misfielded values
- Missing null values
- Cleaning only part of the dataset
- Losing focus on business objectives
- Fixing symptoms instead of root causes
- Not backing up data
- Underestimating time needed for cleaning

Always back up data before cleaning.

---

# Spreadsheet Tools for Data Cleaning

## Conditional Formatting
Highlights cells that meet specific conditions.

## Remove Duplicates
Automatically deletes duplicate rows.

## Text Functions

- `COUNTIF(range, "value")`
- `LEN(range)`
- `LEFT(range, n)`
- `RIGHT(range, n)`
- `MID(range, start, length)`
- `CONCATENATE(item1, item2)`
- `TRIM(range)`

These help detect errors, inconsistencies, and formatting issues.

---

## Additional Cleaning Techniques

- Sorting
- Filtering
- Pivot tables
- VLOOKUP
- Plotting data to identify outliers

Visualization helps detect anomalies quickly.

---

# Data Mapping

**Data mapping** matches fields between different data sources.

It ensures compatibility when transferring or merging data.

---

## Data Mapping Steps

1. Identify data to move.
2. Map fields between systems.
3. Transform data into consistent format.
4. Transfer data.
5. Test and validate transferred data.
6. Begin analysis once confirmed clean.

---

## Schema

A **schema** describes how data is organized in a database.

It defines:
- Tables
- Fields
- Relationships

Understanding schema improves mapping accuracy.

---

# Key Takeaway

Data cleaning is not optional.

Clean data:
- Improves integrity
- Reduces bias
- Prevents costly mistakes
- Strengthens stakeholder trust

Without clean data, even advanced analysis becomes unreliable.
