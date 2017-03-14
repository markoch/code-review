# Code Review

## Phase 1: The Light Pass

### General
- Code formatter has been used
- Line indentation char and line breaks
- Only required files are changed
- Disagreement between code and specification
- Comments in source code are included
- Documentation of the implementation is created or updated
- Does not contain any unimplemented areas like //TODO or //FIXME
- Optimistic or undefensive programming

### Unclear Or Messy
- Verify correct and meaningful naming
- Magic numbers and values
- Variables used for more than one purpose
- Minimized variable, method and class scopes
- Method signature
- Packing too much into one line
- Complex IF conditions, IF instead of Switch
- Cyclomatic complexity

### Error Handling
- Avoid empty catch blogs
- Error handler over-catches exceptions and aborts current flow or application
- Error handler is not implemented e.g. contains TODO, FIXME

### Java
- Review class imports
- Wrong use of == and equals()
- Wrong use of collection data types, like List instead of Set
- Object contract errors (e.g. equals and hashCode)
- Exposure of immutable data types

### Git Commit Message
- Describes what and why it has changed
- Verify correct format

## Phase 2: The Contextual Pass
### Code Structure
- Understandability of written changes
- No logical errors
- Max usage of static compiler checking
- Does not violate architecture guidelines, design principles or implementation patterns
- Are there any alternative implementations that increase simplicity, readability or maintainability
- Check edge cases in functions
- Any better approach to use a framework, library or class exists?
- Look for omissions: Shouldn't this component also do X?
- Enough log statements to find bugs quickly

### External Systems
- Reduce amount of calls / Optimize calls to external systems

### Tests
- Unit-tests and End 2 End Tests are added and test all functionality
- Test coverage of changed lines and critical path

### Code-Review Commenting
- Adding comments: Be polite and constructive
- Add positive comments for good code e.g. unusually elegant solution, creative solution, great design

### Finalizing
- Sign of the pull request

## References
[Code Review](https://github.com/thoughtbot/guides/tree/master/code-review)

[Code Briefing: What does it mean when code is “easy to reason about”?](https://medium.freecodecamp.com/code-briefing-what-does-it-mean-when-code-is-easy-to-reason-about-64453e71b751#.f0136qxo3)

[Do Not Allow Bad Smells In Your Code](https://codetrips.com/2015/01/25/do-not-allow-bad-smells-in-your-code/)

[Writing Great Git Commit Messages; A Revision](https://medium.com/@f8/writing-great-git-commit-messages-a-revision-b86311c610e#.b114xxhjv)

[Giving better code reviews](https://medium.com/@mrjoelkemp/giving-better-code-reviews-16109e0fdd36)

[Coding like Shakespeare: practical function naming conventions](https://rainsoft.io/coding-like-shakespeare-practical-function-naming-conventions/)

[Simple Testing Can Prevent Most Critical Failures: An Analysis of Production Failures in Distributed Data-Intensive Systems](https://www.usenix.org/system/files/conference/osdi14/osdi14-paper-yuan.pdf)

[Software Architecture and Design](https://msdn.microsoft.com/en-us/library/ee658093.aspx)

[YouTube: Core Design Principles for Software Developers](https://www.youtube.com/watch?v=llGgO74uXMI)

[Information about properly formatted commit messages](https://github.com/torvalds/subsurface-for-dirk/commit/b6590150d68df528efd40c889ba6eea476b39873)
