# Risk Analysis and Test Coverage

## Risk Analysis in Software Testing
Risk analysis is an essential to properly approach software testing.  It allows is to identify and give priority to areas of high risk or exposure.

In other words, properly identifying risks by likelihood and potential effect allows you to focus your resources on testing what's important. Thus, formulating an effective test plan.

Keep in mind risks beyond user interaction; things like new hardware, technology, and automation tools.

Many risks are unavoidable, which makes it necessary to have a plan to hadle and mitigate them.  Naturally, this plan should include a risk assessment database, in which risks are porperly classified and prioritized.

The risk identification process should include: business risk, testing risk, developing and integration risk, etc.

In assessing each risk, highlight the effect, the cause, and the likelihood.  The combination of which, will help you refine your test plan and prioritize your resources.

---

## Test Coverage
> Test coverage is a tool for finding untested parts of a codebase [with the intent of improving the test suite].

There are many angles to test sufficiency, which might be the right but inprecise gauge.  High coverage of high quality tests may get you there.

Test coverage is commonly stated as a percentage.  But do not rely too much on a high number, because the tests might focus on routine areas but not cover important aspects.  In other words, it is possible to reach high coverage numbers with low quality testing.

Conversely, low coverage numbers point to insufficient testing.

*Thus, high coverage is not necessarily good, but low coverage is bad*

> If a part of your test suite is weak in a way that coverage con detect, it's likely also weak in a way it can't

A coverage tool can tell you about existing code, but can't tell you about code that ought to exist; omissions.  That's where high quality testing shines.

Related but separate, a lot of tests might not be a good thing, because there might be duplication or lack of simplicity.

*Warning*
> a thoroughly tested program will take roughly twice as long to produce as one that's not tested at all

*** More info: read How to miuse coverage below ***

> coverage tools are only helpful if they’re used to enhance thought, not replace it.

---

## Random Module Python
The Randome moodule gives us access to functions for many operations, the most important of which is random number generation.

- randint(l, h) -random integer N, l <= N <= h
- random -random floating point number in range [0.0, 1.0)
- choice(seq) -returns a random choice form a non-empty sequence (e.g. array)
- shuffle(seq) -shuffles the seq in place
- randrange(start,stop,step) -returns a randomly selected element from the range

---

### Resources

- [How to use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
- [Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)
- [How to misuse coverage](http://www.exampler.com/testing-com/writings/coverage.pdf)

---

[Back to table of contents](../README.md)