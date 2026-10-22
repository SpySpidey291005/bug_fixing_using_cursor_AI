# bug_fixing_using_cursor_AI

# Student Utilities – Python Unit Testing

## Overview

This project contains Python utility functions for calculating average marks, checking whether a student has passed, and determining grades based on average marks. It also includes unit tests using Python's built-in `unittest` module to verify the functionality of these functions.

## Files

* `student_utils.py` – Contains the utility functions.
* `test_student_utils.py` – Contains unit tests for the utility functions.

## Functions

### 1. `calculate_average(marks)`

Calculates the average of a list of marks by adding all marks and dividing the total by the number of marks.

**Example:**

```python
calculate_average([80, 90, 100])
```

**Output:**

```text
90.0
```

### 2. `is_passing(mark)`

Checks whether a student's mark meets the passing requirement.

* Passing mark: `40`
* Returns `True` if the mark is greater than or equal to `40`.
* Returns `False` if the mark is below `40`.

### 3. `get_grade(average)`

Returns a grade based on the student's average marks.

| Average Marks | Grade       |
| ------------- | ----------- |
| 90 and above  | Distinction |
| 60–89.99      | First       |
| 45–59.99      | Second      |
| Below 45      | Fail        |

## Unit Testing

The project uses Python's built-in `unittest` module to test the utility functions.

The tests cover:

* Average calculation for three marks.
* Average calculation for a single mark.
* Passing marks above the passing threshold.
* Marks exactly equal to the passing threshold.
* Marks below the passing threshold.
* Distinction grade.
* First grade.
* Second grade.
* Fail grade.

## How to Run

### 1. Run the utility file

```bash
python student_utils.py
```

### 2. Run the unit tests

```bash
python test_student_utils.py
```

## Expected Test Result

The test suite runs **9 tests** and reports `OK` when all tests pass successfully.
