---
published: false
---

## The Dangers of Unnecessary Abstraction

### Sometimes you just need to kill your abstractions

I had an interesting experience this week...

I was working on a small library that I started a week or two ago. I haven't made too much progress, really only just created the foundation for what I want this library to become.

Every night I've tried working on the project this week, I've gone to be fairly dissapointed with the progress I had made. I kept undoing things I had done the night before and then having to go back and redo my unit tests to accomodate my changes, which can really kill a test driven workflow.

Later in the week I remembered something I've heard several times from other developers:

> Don't let perfection become the enemy of progress

I realized that I was probably overcomplicating things, so I decided to revisit my objects and only keep what I needed to have working code. 

It was then that I realized I was creating abstractions that I didn't need, but that I was anticipating I would need. I remembered I shouldn't be creating abstractions for their own sake, but to enable my code when I needed them.

What happened next was rather surprising (to me), and validated my suspicions. I went back and deleted all my interfaces and abstract classes (pushing abstract properties and methods to the child class), ran my tests, and they all pass. The abstractions were doing absolutely nothing to help my tests work.

So, the lesson I learned this week was:
### If your tests pass without any of your abstractions, chances are you don't need them.