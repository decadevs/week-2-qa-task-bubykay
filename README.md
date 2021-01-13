WEEK TWO TASK

## **1. What is test coverage and why is it very important in testing?**

What is the difference between the testing technique anCoverage is a metric in software testing for how far/thorough software testing is. Below are coverage types;

   ### 1. **Function coverage**

Functional coverage is the extent to which some functionality has been exercised by tests, and is expressed as a percentage of the type(s) of element being covered. For example, using traceability between tests and functional requirements, the percentage of these requirements which are addressed by testing can be calculated, potentially identifying coverage gaps.

### **Statement Coverage**

This indicates the fraction of code statements of been tested at least once.

   ###  **Branch coverage**

In an if … statement, branch coverage indicates how thorough both if conditions have been tested likewise if the condition is false i.e. have both the true and false path been tested, how thorough have then been tested?

### **Why coverage is important in testing**

1. It can assure the quality of the test
2. It can help identify what portions of the code were actually touched for the release or fix
3. It can help to determine the paths in your application that were not tested
4. Prevent defect leakage
5. Time, scope and cost can be kept under control
6. Defect prevention at an early stage of the project lifecycle
7. It can determine all the decision points and paths used in the application, which allows you to increase test coverage
8. Gaps in requirements, test cases and defects at the unit level and code level can be found in an easy way

## 2. What is the difference between the testing technique and types of testing?

Software testing is the activity to check whether the actual results match the expected results and to ensure that the software is defect free while Software Testing Techniques help you design better test cases

### 3. Discuss each type of testing and discuss the sub-testing types associated with each type of testing.

1. Create a folder in google drive with name Testing Types Task

  1. Inside the folder, create more folders with name of the type of bug that can be found on the site
  2. Go to link AcademyBugs.com
  3. Click find bugs.
  4. On the site, there are only 25 bugs. You will perform exploratory testing where you will test every functionality on the site and find all defects (features that do not work as expected).
  5. For each bug you find take a screen shot of the bug report and save it under the related folder.
  6. When done, take a screen shot of bug number found and save to folder.
  7. Submit the google drive link, do not restrict user, set link to everyone with link.
  8. This will teach you how to classify bugs under testing types and the kind of defects to look out for in an application.

[!https://drive.google.com/drive/folders/1y9lZMuiGT\_XMCbMYTAZOQjDN4JC5w6Q6?usp=sharing](https://drive.google.com/drive/folders/1y9lZMuiGT_XMCbMYTAZOQjDN4JC5w6Q6?usp=sharing)

1. What is testing technique, discuss the type of testing techniques and give 2 examples of each

**Types of Testing Techniques**

1. **Error Guessing**

Error guessing is a technique is an experience-based test technique used to anticipate the occurrence of errors, defects, and failures, based on the tester&#39;s knowledge, including:

- How the application has worked in the past
- What kind of errors tend to be made
- Failures that have occurred in other applications

A methodical approach to the error guessing technique is to create a list of possible errors, defects, and failures, and design tests that will expose those failures and the defects that caused them. These error, defect, failure lists can be built based on experience, defect and failure data, or from common knowledge about why software fails.

1. **Boundary Value Analysis**

Boundary value analysis (BVA) is an extension of equivalence partitioning, but can only be used when the partition is ordered, consisting of numeric or sequential data. The minimum and maximum values (or first and last values) of a partition are its boundary values.

**For example** , suppose an input field accepts a single integer value as an input, using a keypad to limit inputs so that non-integer inputs are impossible. The valid range is from 1 to 5, inclusive. So, there are three equivalence partitions: invalid (too low); valid; invalid (too high). For the valid equivalence partition, the boundary values are 1 and 5. For the invalid (too high) partition, the boundary value is 6. For the invalid (too low) partition, there is only one boundary value, 0, because this is a partition with only one member.

In the example above, we identify two boundary values per boundary. The boundary between invalid (too low) and valid gives the test values 0 and 1. The boundary between valid and invalid (too high) gives the test values 5 and 6. Some variations of this technique identify three boundary values per boundary: the values before, at, and just over the boundary. In the previous example, using three-point boundary values, the lower boundary test values are 0, 1, and 2, and the upper boundary test values are 4, 5, and 6

Behavior at the boundaries of equivalence partitions is more likely to be incorrect than behavior within the partitions. It is important to remember that both specified and implemented boundaries may be displaced to positions above or below their intended positions, may be omitted altogether, or may be supplemented with unwanted additional boundaries. Boundary value analysis and testing will reveal almost all such defects by forcing the software to show behaviors from a partition other than the one to which the boundary value should belong.

Boundary value analysis can be applied at all test levels. This technique is generally used to test requirements that call for a range of numbers (including dates and times). Boundary coverage for a partition is measured as the number of boundary values tested, divided by the total number of identified boundary test values, normally expressed as a percentage.

1. **Decision Table Techniques**

Decision tables are a good way to record complex business rules that a system must implement. When creating decision tables, the tester identifies conditions (often inputs) and the resulting actions (often outputs) of the system. These form the rows of the table, usually with the conditions at the top and the actions at the bottom. Each column corresponds to a decision rule that defines a unique combination of conditions which results in the execution of the actions associated with that rule. The values of the conditions and actions are usually shown as Boolean values (true or false) or discrete values (e.g., red, green, blue), but can also be numbers or ranges of numbers. These different types of conditions and actions might be found together in the same table.

The common notation in decision tables is as follows: For conditions:

- Y means the condition is true (may also be shown as T or 1)
- N means the condition is false (may also be shown as F or 0)
- — means the value of the condition doesn&#39;t matter (may also be shown as N/A)

For actions:

- X means the action should occur (may also be shown as Y or T or 1)
- Blank means the action should not occur (may also be shown as – or N or F or 0)

A full decision table has enough columns (test cases) to cover every combination of conditions. By deleting columns that do not affect the outcome, the number of test cases can decrease considerably. For example by removing impossible combinations of conditions. For more information on how to collapse decision tables.

The common minimum coverage standard for decision table testing is to have at least one test case per decision rule in the table. This typically involves covering all combinations of conditions. Coverage is measured as the number of decision rules tested by at least one test case, divided by the total number of decision rules, normally expressed as a percentage.

The strength of decision table testing is that it helps to identify all the important combinations of conditions, some of which might otherwise be overlooked. It also helps in finding any gaps in the requirements. It may be applied to all situations in which the behavior of the software depends on a combination of conditions, at any test level.

1. **State Transition Testing**

Components or systems may respond differently to an event depending on current conditions or previous history (e.g., the events that have occurred since the system was initialized). The previous history can be summarized using the concept of states. A state transition diagram shows the possible software states, as well as how the software enters, exits, and transitions between states. A transition is initiated by an event (e.g., user input of a value into a field). The event results in a transition. The same event can result in two or more different transitions from the same state. The state change may result in the software taking an action (e.g., outputting a calculation or error message).

A state transition table shows all valid transitions and potentially invalid transitions between states, as well as the events, and resulting actions for valid transitions. State transition diagrams normally show only the valid transitions and exclude the invalid transitions.

Tests can be designed to cover a typical sequence of states, to exercise all states, to exercise every transition, to exercise specific sequences of transitions, or to test invalid transitions.

State transition testing is used for menu-based applications and is widely used within the embedded software industry. The technique is also suitable for modeling a business scenario having specific states or for testing screen navigation. The concept of a state is abstract – it may represent a few lines of code or an entire business process.

Coverage is commonly measured as the number of identified states or transitions tested, divided by the total number of identified states or transitions in the test object, normally expressed as a percentage. For more information on coverage criteria for state transition testing.

1. **Equivalent Partitioning**

Equivalence partitioning divides data into partitions (also known as equivalence classes) in such a way that all the members of a given partition are expected to be processed in the same way. There are equivalence partitions for both valid and invalid values.

- Valid values are values that should be accepted by the component or system. An equivalence partition containing valid values is called a &quot;valid equivalence partition.&quot;
- Invalid values are values that should be rejected by the component or system. An equivalence partition containing invalid values is called an &quot;invalid equivalence partition.&quot;
- Partitions can be identified for any data element related to the test object, including inputs, outputs, internal values, time-related values (e.g., before or after an event) and for interface parameters (e.g., integrated components being tested during integration testing).
- Any partition may be divided into sub partitions if required.
- Each value must belong to one and only one equivalence partition.
- When invalid equivalence partitions are used in test cases, they should be tested individually, i.e., not combined with other invalid equivalence partitions, to ensure that failures are not masked. Failures can be masked when several failures occur at the same time but only one is visible, causing the other failures to be undetected.

To achieve 100% coverage with this technique, test cases must cover all identified partitions (including invalid partitions) by using a minimum of one value from each partition. Coverage is measured as the number of equivalence partitions tested by at least one value, divided by the total number of identifiedequivalence partitions, normally expressed as a percentage. Equivalence partitioning is applicable at all test levels.

1. Using the login form specification requirements, identify all testing techniques that can be used to design test case for this login form. Also Implement the identified techniques and document your solution.
  1. Image link - [https://drive.google.com/file/d/1\_3kr18fUMzPnYDybKCabDJ0gZ6SrVInk/view?usp=sharing](https://drive.google.com/file/d/1_3kr18fUMzPnYDybKCabDJ0gZ6SrVInk/view?usp=sharing)
  2. Requirements
    1. Email must be a valid email format
    2. Email characters cannot be less that 15 characters but not greater than 200 characters
    3. Password should contain at least 8 characters and at most 20 characters
    4. Password must contain at least one character, one number and one capital letter
    5. The Login button should be enabled if the user has entered all the valid required fields (email &amp; password)
    6. Only a registered user can login
    7. All invalid inputs should throw the correct error, tester should suggest the type of error, while valid input should show the correct output.

The following are testing techniques that can be used and their implementations

      1. **Error Guessing**
      2. **Boundary Value Analysis**
      3. **Decision Table Technique**

**ERROR GUESSING IMPLEMENTATION**

1. Enter an invalid Email format: login form should throw an error message otherwise, there is a bug
2. Enter email with 9 characters: login form should throw an error message otherwise, there is a bug
3. Enter email with 25 characters: login for should not throw error message otherwise there is a bug
4. Enter email with 222 character: login form should throw an error message otherwise, there is a bug
5. Enter password of 6 character: login form should throw an error message otherwise, there is a bug
6. Enter password of 15 characters: login form should not throw an error message otherwise, there is a bug
7. Enter password of 31 characters: login form should throw an error message otherwise, there is a bug
8. Enter password with 15 character and capital letters only: login form should throw an error message otherwise, there is a bug
9. Enter password with only 15 character and number: login form should throw an error message otherwise, there is a bug
10. Enter character 15 characters with at least one capital letter and number: login form should not throw an error message otherwise, there is a bug
11. Enter only email address: the login button should not be enabled otherwise there is a bug
12. Enter only password: the login button should not be enabled otherwise there is a bug
13. Enter email and password: the login button should be enabled otherwise there is a bug
14. Login with an unregistered email address and password: the form should not login otherwise, there is a bug
15. Login in with a valid registered email address and password: : the form should login otherwise, there is a bug
16.

1. Design a decision table for Upload image Scenario.
  1. Requirements
    1. you can upload only .jpeg format,
    2. file size must be less than 32kb,
    3. Resolution must be only 137\*177

![](RackMultipart20210113-4-va2g8s_html_e3d025d0e2a18ff1.png)

1. Implement a Graph based testing technique for this scenario
  1. An employee who decides to apply for leave, submits application form to HR, HR verifies eligibility, if not eligible application is rejected, if eligible, Manager ensures feasibility, if feasible, application is rejected else if feasible, application is approved

1. Sometimes a tester is not given all the details and has to come up with a solid logic with given requirements.
  1. Implement a Graph based testing techniques for an atm machine that blocks the user from logging in after 3 wrong trials

1. An organization gives you a new mailing application they just designed to identify its strengths and weaknesses with respect to the standard in the market.
  1. what testing technique would you apply and give a detailed description of what you will do when applying this technique.