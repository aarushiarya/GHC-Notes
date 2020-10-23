# Find your voice as a code reviewer
Alice Bonhomme-Biais, Software Engineering Coach
ChezAlice Consulting;
Kendra Curtis, Director of Engineering;

### Notes

Code reviews can sometimes be intimidating and stress inducing, however if well done they can really improve team coding, collaboration and create a culture of inclusion. This talk will give you confidence and improve your code reviews. We will focus on how you can find your voice during a review and learn how to contribute to a review regardless of your experience level or the power dynamic.

* Increase code quality and provide consistency to code base
* Code review is the single best thing you can do to improve your code
* Benefits of code review
    * Find a bug early
    * Better quality code
    * learning / knowledge transfer
    * Collective ownership 
    * Find better solution
* Tips
    * let them know if you are the wrong person to review
        * Not familiar with the code
        * Going out for vacation / not available
    * if PR is too long
    * PR do not bundle more than one change
    * PR has good description/ context
    * If any rule breaks, put a comment on PR right away
* Types of code review
    * Features / components
    * Bug fixes
    * Other
        * Scripts / template
        * Fix typo
* Reviewers bring fresh perspective 
    * Edge cases
    * How could I break this code
    * Is there potential for concurrency problems
    * Is there prior knowledge or art that I know about this piece of code
    * Is this code “too complex”? Can I understand code quickly or are there ways it can be simplified
* Feature
    * Discuss and iterate on overall design before discussing details in the code
    * Will come in iterations
    * Do the interactions of various pieces of code make sense
    * Does the change belong in this codebase or in the library
    * Does it integrate well with the rest of the system
* Bugs
    * Smaller and focused
    * Usually on timeline
    * Prior knowledge is imp
    * Try to break the code; insure really fixes the issue; doesn’t introduce another bug
    * Open another issue to track other changes, instead of delaying the bug fix
* Make your comments actionable
    * Explain your reasoning
    * Provide suggestions
    * Any specific questions
    * Specify importance of comment
* Try to establish yourself as go-to person for some part of code
* Use it to learn; ask questions to understand; compliment person who walks you through their code
* Pair with someone who does code review; to learn some tips and tricks
* Healthy communication 
    * How to communicate through code review
    * avoid ownership of code - Avoid term “I, mine”, yours; inside use “we”
    * ask questions, instead of making demands
    * be humble and assume best of author
    * comment can simply be a question to ask clarification
    * positive reinforcement- “thank you” / this is awesome
