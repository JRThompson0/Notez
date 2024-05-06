## Testing With JUnit
___
### What is a unit test?
+ It's just code!
  + The job of this code is to confirm that other code is functional.
  + This was done manually before individuals made testing libraries to accomplish this task more easily
### Why use unit tests?
+ A few reasons:
    + It gives Quick Feedback towards any changes, allowing one to know if they break something.
    + It's a Design Aid that helps one turn a process into a series of testable programs.
    + Documentation to build confidence in the program. 
### Unit Test Setup
+ @BeforeAll,@BeforeEach,@Test,@AfterEach,and @AfterAll to label parts of test and setup methods.
+ Assert and check.
  + First test failure will be the only test failure shown. 
    + AssertAll to group up related tests into assertions
  + Can change test text, place string after assertion
+ @DisplayName("SampleString") to change the display name of tests.
+ @Nested to contain tests within tests.
+ @Disabled to turn off a test.
+ @Tag to group tests that are related to eachother. Can tag multiple test methods in multiple classes.
### Unit Test Principles
+ Single Responsibility
  + Methods that print shouldn't calculate
  + Methods that calculate shouldn't print
  + Small methods are testable methods.
+ Dealing with Dependency:
  + Dependency injection-create a double of the dependency, and have both implement a common interface with all necessary methods

