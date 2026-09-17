# Git Practice

## An article I found interesting

**[Things You Should Never Do, Part I](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/)** by Joel Spolsky

### Why I find it interesting

This article argues that the single worst strategic mistake a software company can make is deciding to rewrite its code from scratch. Spolsky uses Netscape's decision to throw away the Navigator 4.0 codebase and rebuild it as his main example, and he makes the case that old code is not "worse" just because it is messy. Every ugly branch and odd special case in a mature codebase is usually a bug fix that somebody learned the hard way. When you rewrite, you throw all of that knowledge away and then spend years rediscovering it.

What I like about the piece is that it pushes back on an instinct almost every developer has. Reading someone else's code is harder than writing your own, so a rewrite always *feels* like the faster path. The article makes a strong argument that this feeling is misleading, and that careful incremental refactoring almost always beats a clean-slate rebuild. It is more than twenty years old, but the lesson comes up constantly, whether the "rewrite" is a new framework, a new language, or a migration to microservices.
