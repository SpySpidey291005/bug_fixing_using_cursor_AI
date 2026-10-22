# Code Audit Checklist – Student Utilities

## 1. Project Information

| Item                 | Details                 |
| -------------------- | ----------------------- |
| Project Name         | Student Utilities       |
| Programming Language | Python                  |
| Testing Framework    | `unittest`              |
| Source File          | `student_utils.py`      |
| Test File            | `test_student_utils.py` |

## 2. Code Audit Checklist

| S. No. | Audit Item          | Verification Criteria                                            | Status     |
| -----: | ------------------- | ---------------------------------------------------------------- | ---------- |
|      1 | Average Calculation | Calculates the average of the provided marks correctly.          | ✅ Passed   |
|      2 | Single-Mark Average | Correctly calculates the average when only one mark is provided. | ✅ Passed   |
|      3 | Passing Threshold   | Defines `PASS_MARK = 40`.                                        | ✅ Verified |
|      4 | Above Passing Mark  | Returns `True` for marks above 40.                               | ✅ Passed   |
|      5 | Exact Passing Mark  | Returns `True` for marks equal to 40.                            | ✅ Passed   |
|      6 | Below Passing Mark  | Returns `False` for marks below 40.                              | ✅ Passed   |
|      7 | Distinction Grade   | Returns `Distinction` for averages of 90 or above.               | ✅ Passed   |
|      8 | First Grade         | Returns `First` for averages from 60 to below 90.                | ✅ Passed   |
|      9 | Second Grade        | Returns `Second` for averages from 45 to below 60.               | ✅ Passed   |
|     10 | Fail Grade          | Returns `Fail` for averages below 45.                            | ✅ Passed   |
|     11 | Unit Test Execution | Executes the test suite using `unittest`.                        | ✅ Passed   |
|     12 | Test Results        | All 9 tests pass successfully.                                   | ✅ Passed   |

## 3. Test Case Checklist

| S. No. | Test Case                | Input           | Expected Output | Status   |
| -----: | ------------------------ | --------------- | --------------- | -------- |
|      1 | Average of three marks   | `[80, 90, 100]` | `90.0`          | ✅ Passed |
|      2 | Average of a single mark | `[40]`          | `40.0`          | ✅ Passed |
|      3 | Above passing mark       | `41`            | `True`          | ✅ Passed |
|      4 | Exact passing mark       | `40`            | `True`          | ✅ Passed |
|      5 | Below passing mark       | `39`            | `False`         | ✅ Passed |
|      6 | Distinction grade        | `95`            | `Distinction`   | ✅ Passed |
|      7 | First grade              | `60`            | `First`         | ✅ Passed |
|      8 | Second grade             | `45`            | `Second`        | ✅ Passed |
|      9 | Fail grade               | `30`            | `Fail`          | ✅ Passed |

## 4. Test Execution Checklist

| Item         | Details                        | Status      |
| ------------ | ------------------------------ | ----------- |
| Test Command | `python test_student_utils.py` | ✅ Executed  |
| Total Tests  | 9                              | ✅ Completed |
| Failures     | 0                              | ✅ None      |
| Errors       | 0                              | ✅ None      |
| Final Result | `OK`                           | ✅ Passed    |

## 5. Final Audit Summary

| Audit Parameter      | Result                        |
| -------------------- | ----------------------------- |
| Average Calculation  | Passed for tested cases       |
| Passing Validation   | Passed for tested cases       |
| Grade Classification | Passed for tested cases       |
| Unit Testing         | All 9 tests passed            |
| Overall Audit Status | ✅ **PASSED FOR TESTED CASES** |
