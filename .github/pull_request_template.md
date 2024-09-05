## Requester Checklist

### Implementation

- [ ] Have you tested your implementation locally?
- [ ] If applicable, has an appropriate changelog entry been added? Do not include if you are fixing/changing something that is only in the current release.
- [ ] There are no warnings that have been suppressed unnecessarily
- [ ] Have automated tests been added, or have related ones been updated to cover the change?
- [ ] Have all OneBlink dependency updates been completed (eg apps / apps-react / types etc).
- [ ] Have you ensured this change does not add unwanted dependencies?
- [ ] If this PR contains a refactor, have relevant Jira testing tasks added?
- [ ] Changes that will knowingly make the feature/bug incomplete have been commented with TODO and a description of what needs to be done to finish the feature/bug
- [ ] Any changes made to public APIs have been reflected in the documentation
- [ ] Have you isolated business logic where possible to allow for unit testing?

### Logging and Debugging

- [ ] Are the error messages, if any, informative?
- [ ] Are there enough log events and are they written in a way that allows for easy debugging?
- [ ] "Debugging" code removed
- [ ] Front-end: No erroneous `Console.WriteLines`

### Readability

- [ ] All class, variable, property and method modifiers are provided with the smallest scope possible
- [ ] New files, variables and functions are descriptive/comprehensible and named consistently.
- [ ] There is no dead code (unreachable code)
- [ ] There is no usage of [magic numbers](<https://en.wikipedia.org/wiki/Magic_number_(programming)>)
- [ ] There is no commented out code.
- [ ] In hard-to-understand areas, comments exist and describe rationale or reasons for decisions in code

### Security

- [ ] All personal data inputs are checked (for the correct type, length/size, format, and range).
- [ ] No sensitive information is logged or visible in a stacktrace
- [ ] Are authorization and authentication handled correctly?
- [ ] Is (user) input validated, sanitized, and escaped to prevent security attacks such as cross-site scripting or SQL injection?
- [ ] Is data retrieved from external APIs or libraries checked for security issues?
- [ ] Do API endpoints return appropriate status codes

## Reviewer Guide

- It is important that you understand the purpose of the PR.
- You are encouraged to engage with the requestor if you do not understand any of the proposed code changes/additions/deletions.
- Do you, the reviewer, understand what the code does? Do you think a specific expert, like a security expert or a usability expert, should look over the code before it can be accepted?
- Is a framework, API, library, or service used that should not be used? Are there alternatives you could recommend?
- Are there existing hooks/components/functions in the same code base that could be utilised?
- When reviewing tests, attempt to identify missing edge cases that may be relevant to the proposed implementation
- Ensure you check for:
  - Security
  - Scalability
  - Performance
  - Maintainability
