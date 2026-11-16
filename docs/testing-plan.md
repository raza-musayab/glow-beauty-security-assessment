Testing Plan – Glow Beauty Salon

Web Application Security Assessment

1. Introduction

This testing plan defines the procedures for checking the functionality, security, and performance of the web application used as the practice target for the Glow Beauty Salon security assessment.

Testing will be performed in an authorized PortSwigger Web Security Academy laboratory.

The beauty salon scenarios are used to represent realistic business requirements.

2. Testing Objectives

The objectives are:

- Check application functionality.
- Identify input validation problems.
- Examine authentication and authorization.
- Review session management.
- Identify potential web application vulnerabilities.
- Check application responses to invalid inputs.
- Observe application performance during normal use.
- Document test results and recommendations.

3. Testing Environment

Item| Details
Client| Glow Beauty Salon
Practice Platform| PortSwigger Web Security Academy
Browser| Google Chrome or Firefox
Security Tool| Burp Suite Community Edition
Documentation| GitHub
Test Data| Fictional salon information
Selected Lab| To be recorded after selection

4. Functional Testing

Functional testing checks whether the application behaves as expected.

Test ID| Test Case| Expected Result
FT01| Open the application| Application loads successfully
FT02| Navigate application pages| Pages display correctly
FT03| Enter valid information| Information is accepted where supported
FT04| Submit empty required fields| Clear validation message appears
FT05| Enter invalid email in a relevant form| Invalid email is rejected

5. Security Testing

Security testing checks whether the application has potential security weaknesses.

Test ID| Security Test| Expected Result
ST01| Authentication assessment| Login security is evaluated
ST02| Authorization assessment| Unauthorized access is prevented
ST03| SQL Injection assessment| Unsafe database input is handled securely
ST04| XSS assessment| Untrusted input is handled safely
ST05| Session management assessment| Sessions are handled securely
ST06| Input validation assessment| Invalid input is handled correctly

All security tests will be conducted only in the authorized practice laboratory and within its permitted boundaries.

6. Performance Testing

Performance testing observes how the application behaves during normal usage.

Test ID| Performance Check| Expected Result
PT01| Open application homepage| Page loads successfully
PT02| Navigate different pages| Pages respond normally
PT03| Submit normal requests| No unexpected application errors
PT04| Observe response times| Response times are recorded

No load testing or denial-of-service testing will be performed.

7. Main Path Testing

Scenario: Customer Appointment Booking

This is an illustrative business workflow for the salon.

Steps:

1. Customer opens the salon application.
2. Customer views available beauty services.
3. Customer selects Facial Treatment.
4. Customer enters fictional customer information.
5. Customer selects an appointment date.
6. Customer submits the booking information.

Expected Result:

The application should accept valid information and display an appropriate booking confirmation, if the selected application supports this functionality.

8. Failure Path Testing

Scenario: Invalid Customer Information

Steps:

1. Customer opens a relevant registration or booking form, if available.
2. Customer enters an invalid email address.
3. Customer leaves a required field empty.
4. Customer submits the form.

Expected Result:

- Application should reject invalid information.
- A clear validation message should appear.
- The application should not crash.
- Incorrect information should not be accepted as valid.

9. Test Result Recording

Every test will be documented using the following format:

Test ID| Actual Result| Status
FT01| Pending execution| Not tested
FT04| Pending execution| Not tested
ST01| Pending execution| Not tested
PT01| Pending execution| Not tested

Results will be updated after actual testing.

10. Test Evidence

The following evidence will be collected:

- Screenshots of the practice laboratory.
- Relevant application pages.
- Test input and application responses.
- Security testing observations.
- Performance observations.
- Test results.

Sensitive information such as passwords and session tokens will not be published.

11. Pass and Fail Criteria

Pass:

- Application behaves according to expected results.
- Invalid information is handled appropriately.
- Unauthorized access is prevented.
- No unexpected application crash occurs.

Fail:

- Application accepts invalid information.
- Unauthorized access is possible.
- Unexpected errors or crashes occur.
- A security weakness is verified.

A failed security test does not automatically mean a confirmed vulnerability; findings must be verified and documented.

12. Conclusion

This testing plan establishes a structured approach for evaluating the web application associated with the Glow Beauty Salon security assessment.

It covers functional testing, security testing, performance checks, the main business workflow, and failure scenarios.

The results will support the next project task: mapping the application and its attack surface.
