# Software Testing of Hotel Management System (Java + JUnit 5)

This project presents a comprehensive unit testing analysis of a Java-based Hotel Management System. The work focuses on designing, implementing, and evaluating test cases to ensure the correctness and reliability of the system.

The project was developed as part of a Software Testing course.

## Overview

The tested system is a console-based Hotel Management System that handles:

* Room booking and cancellation
* Food ordering
* Billing and checkout
* Room availability tracking

The system uses object-oriented design and file handling (serialization) to manage hotel data.

## Testing Scope

Due to system design constraints, only components independent of user input and file I/O were selected for unit testing.

The following components were tested:

* Input validation (name, phone, gender)
* Room classes (Single and Double room)
* Billing logic
* Utility methods (room indexing, availability counting)
* Exception handling
* Runnable thread behavior

## Testing Methodology

The testing strategy includes:

* Positive and negative test cases
* Boundary Value Analysis
* Edge case testing
* State verification
* Integration-level assertions

Special handling was used for testing components dependent on user input.

## Tools and Technologies

* Java
* JUnit 5 (JUnit Jupiter)
* Eclipse IDE

## Test Implementation

* Total test cases: **119**
* Test files:

  * ValidatorTest.java
  * RoomTest.java
  * BillTest.java
  * HotelUtilityTest.java

All tests were executed using JUnit in Eclipse.

## Results

* Total Tests Run: 119
* Errors: 0
* Failures: 0

All test cases passed successfully, confirming the correctness of the tested components.

## Key Highlights

* Strong validation testing using regular expressions
* Complete boundary testing for room indexing logic
* Accurate billing verification across all room types
* Use of Java Reflection to test Scanner-dependent classes
* Reliable handling of edge cases (empty inputs, null states)

## Limitations

* Methods dependent on user input (Scanner) were not unit tested
* File handling (serialization) was not included in unit testing
* Some UI-based outputs were not validated

## Conclusion

The project demonstrates a structured and systematic approach to software testing. The results confirm that the system’s core logic is reliable and behaves correctly under various conditions.

It also highlights the importance of separating business logic from input handling to improve testability in software systems.
