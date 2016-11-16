# Code Review
Checklist for doing a code review

# Phase 1: The light pass
## General
- Adding comments: Be polite and constructive
- Correct use of code formatter
- Line indentation char ar line breaks
- Only required files are changed
- Verify comments in source
- Check static dode analysis results
- Disagrement between code and specification
- Max usage of static compiler checking
- Optimistic and undefensive programming

## Unclear or messy
- Verify correct and meaningful naming
- Magic numbers and values
- Variables used for more than one purpose
- Design principles: DRY, SOLID, GRASP, YAGNI
- Variable, method and class scope
- Method signture
- Packing too much into one line
- Long Method
- Cyclomatic complexity

## Java
- Review class imports
- Missuse of == and equals()
- Misuse of Arrays, List or Set
- Object contract errors (equals and hashCode)
- Exposure of immutable data types

## Gerrit commit message
- All details are included
- Describe what and why it has changed

# Phase 2: The contextual pass
## Code structure
- Understanability of written
- Logical errors
- Wrong usage of implementation patterns
- Alternative implementations that increase simplicity, readability or maintinability
- Check edge cases in functions
- Better approach to use a framework, library or class
- Look for ommissions: Shouldn't this component also do X?

## External systems
- Reduce amount of calls / Optimize calls to external systems

## Tests
- Existing tests still pass
- Test coverage of changed lines and critical path
- Enhancements to newly added tests

## Code-Review Commenting
- Add comments for good code: Unusally ellegant solution, creative solution, great design,...

## Finalizing
- Sign of the pull request

# References
[Code Review](https://github.com/thoughtbot/guides/tree/master/code-review)

[Code Briefing: What does it mean when code is “easy to reason about”?](https://medium.freecodecamp.com/code-briefing-what-does-it-mean-when-code-is-easy-to-reason-about-64453e71b751#.f0136qxo3)

[Do Not Allow Bad Smells In Your Code](https://codetrips.com/2015/01/25/do-not-allow-bad-smells-in-your-code/)

[Writing Great Git Commit Messages; A Revision](https://medium.com/@f8/writing-great-git-commit-messages-a-revision-b86311c610e#.b114xxhjv)

[Giving better code reviews](https://medium.com/@mrjoelkemp/giving-better-code-reviews-16109e0fdd36)

[Coding like Shakespeare: practical function naming conventions](https://rainsoft.io/coding-like-shakespeare-practical-function-naming-conventions/)
