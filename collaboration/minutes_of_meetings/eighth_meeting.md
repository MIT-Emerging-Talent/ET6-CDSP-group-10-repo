# MINUTES OF GROUP MEETING

**Date:** 13th July 2025

**Time:** 5:00 PM – 6:45 PM GMT

**Venue:** Google Meet

**Recorder:** Yool Malaak

---

## Attendance

The following members were present:

Yool Malaak

Ghyath Ibrahim

Nimatallahi Masuud

Tamir El-Waleed

Lukmon Alao

---

## 1.0 OPENING

1.1 Ghyath called the meeting to order and welcomed all present at 5:05 PM

1.2 Yool recorded all the members present.

---

## 2.0 AGENDA

- **2.1** Team prepares to begin the analysis

- **2.2** Data Cleaning and Currency Handling

- **2.3** Missing Values and Data Encoding Strategy

- **2.4** Generator Type Consolidation

- **2.5** Project Research and Publication

---

## 3.0 MEETING DISCUSSIONS

### 3.1 Data Cleaning and Analysis Preparation

- Plan to open a new Jupyter Notebook for analysis after completing data
  cleaning.

- Ghyath to transfer code to personal laptop and verify implementation.

- Pull request created for documentation; Ghyath requested code review.

- Synthetic dataset generated via ChatGPT and pushed to repository.

- Team to ensure that local VS Code environments are synchronized with the
  repository.

- Yool assigned to convert various currencies in the dataset to USD.

### 3.2 Data Cleaning and Currency Handling

- Discussed challenges with currency conversion across countries.

- Ghyath to develop code that auto-assigns currency based on country field.

- Some data entries are encoded in Latin; team to handle encoding during
  loading.

- Decision to convert the `cost` column from float to integer for
  standardization.

- Yool suggested tracking restaurant data for Nigeria and aligning data
  formatting with other regions.

### 3.3 Missing Values and Data Encoding Strategy

- Ghyath proposed automatic handling for missing values in generator-related
  columns.

- Noted that Python accepts mode filling only for categorical (non-numeric)
  fields.

- Advised against filling all missing values — instead, handle based on
  context.

- Team to analyze missing values in columns like generator runtime and diesel
  usage.

- Recognized that projects using grid electricity may naturally lack generator
  data.

### 3.4 Generator Type Consolidation

- Discussed differences in cost and performance between PMS, petrol, and
  diesel generators.

- Strategy agreed: Consolidate all types under a single label — “generator” —
  for this study.

- Decision to replace specific petrol generator entries with the general
  “generator” label.

### 3.5 Project Research and Publication

- Team intends to prepare the project for academic or professional
  publication.

- Will develop analysis questions such as:

- "Which countries rely most on generators?"

- “Cost comparisons by generator type and country”

---

## 4.0 SHARING OF ROLES

### 4.1 Various tasks to ensure efficient progress and timely delivery

---

## 5.0 CLOSING

5.1 With no further issues to discuss, Tamir moved to close the meeting. The
motion was accepted, and the meeting was officially closed at **6:05 PM**
