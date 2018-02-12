# Purpose

General place to maintain list of guidelines for unit testing.  I mostly program in C# so it is the flavor of the day.

# Resources that I have used to help my understanding

* Pluralsight courses
    * [Effective C# Unit Testing for Enterprise Applications](https://app.pluralsight.com/library/courses/csharp-unit-testing-enterprise-applications/table-of-contents)
    * [Better .NET Unit Tests with AutoFixture: Get Started](https://app.pluralsight.com/library/courses/autofixture-dotnet-unit-test-get-started/table-of-contents)
    * [Better Unit Test Assertions with Shouldly](https://app.pluralsight.com/library/courses/shouldly-unit-test-assertions/table-of-contents)
    * [Testing .NET Code with xUnit.net 2](https://app.pluralsight.com/library/courses/xunitdotnet2-dotnet-code-testing/table-of-contents)

* Links to stuff
    * [Rusty Divine's checklists - my starting point](https://github.com/osmyn/Practices/blob/master/UnitTestGuidelines.md)
    *

# Current tools used

| Tool | Used For |
|------|----------|
| [xunit](https://github.com/xunit/xunit) | Testing Framework |
| [Shoudly](https://github.com/shouldly/shouldly) | Asserts |
| [AutoFixture](https://github.com/AutoFixture/AutoFixture) | Creating Fixtures
| TBD | Mocking framework

# Unit test code review checklist

TBD:  Change these guidelines into a checklist

* Test names should follow the pattern: 
   * UnitOfWork_Condition_Result
   * [UnitOfWork_StateUnderTest_ExpectedBehavior]
* Test should came common section
    * TBD:  Decide on Arrange, Act, Assert or Given, When, Then
* Fake all dependencies
* Stay within one project layer (i.e API)
* Determine if the test is testing state, value, or interaction
* Avoid more than one Mock
* Only assert against one object
* Favor the public API
    * TBD:  What is the "public" API when the application is doing mainly automated data processing
* Favor builder over setup methods
    * TBD: How does this fit with Fixtures/AutoFixture
* Test Behavior not Methods



