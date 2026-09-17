# Git Practice

## An article I found interesting

[Things You Should Never Do, Part I](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/) by Joel Spolsky, published in April 2000.

## Why I find it interesting

Spolsky says the worst strategic mistake a software company can make is to rewrite its code from scratch. His example is Netscape, in 1997 Netscape threw away the Navigator 4.0 codebase and started over, and the rewrite took three years, and during those three years Netscape shipped nothing while Internet Explorer took the browser market. Old code looks messy because it has been fixed, where each ugly branch is probably so because of a bug somebody hit in production and patched.

I like the article because it argues against an instinct I have. Reading someone else's code is harder than writing my own code, so a rewrite always feels faster on small projects. Spolsky shows the feeling is wrong in big projects and production code.

## Comment from Veer Pratap Singh

The point about old code containing hard-earned bug fixes stood out to me. A strange condition might look unnecessary until removing it brings back a problem that only happens for a few users. Before replacing that code, I would look through its commit history and add tests for the behavior it needs to preserve. This also connects to Fowler's technical debt article: improving a system does not have to mean starting over. Small refactors let a team keep shipping while checking that each change still works. I would not take this as a rule that every rewrite is wrong, but I would want a specific reason why gradual improvements cannot solve the problem first.
