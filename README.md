# What do?

Principles for working in a group in a iterative manner.

### How to start?

* Start with user story mapping -> stories (everyone)
* Then continue with feature/example mapping -> concrete examples for stories (smaller group)
* And then you can write specifications -> gherkin (PM + dev + QA)
* Finally dive into executable specification -> cucumber (dev + QA)

### Principle questions after every iteration

* What did we do well?
* What have we learned?
* What can we do better?
* What puzzles us?

### The flow

Maximum amount for following cycle should be few hours!

```
Story --> Build --> Release --> Feedback --> Change --> Story --> ...
```

### Pairing / Mobbing

[Read this: "Mob Programming Guidebook"](http://www.mobprogrammingguidebook.com/images/mobprogrammingguidebook.pdf)

* Every piece of code needs be reviewed by someone else, so you’ll need to context switch to do review. You don’t need this when pairing / mobbing because it’s already reviewed.
* Knowledge about the change/new thing is not shared or is shared very superficially (just going through the code won’t give deep insight on the change).
* Knowledge from others is not shared to you, e.g. “we can’t change this because…” or “did you know that this is easier to implement this way”.
* Worst case scenario you become the only person knowing about something - this is also a business risk!
* Thinking that you are more productive when you can advance multiple things at once by splitting the work between different people is just an illusion.
* You can get stuck and don’t even notice. You fall into a rabbit hole and 5 hours later wake up to the realization that you didn’t achieve anything. This happens less often in a group.

**If you have trouble concentrating or start getting bored while pairing/mobbing:**

* Have a break! No one can stay focused forever.
* Pairing/mobbing is difficult, it’s also a skill which your team can learn. It takes time for everyone to adjust. Learn what different methods people prefer when pairing/mobbing.
* Switch driver! It’s boring to watch the other person type for 2 hours. Try ping-pong: Change driver every 15 minutes.
* Don’t try to do it 100% of time. It’s exhausting. But don’t also fall into the trap of thinking that you’ll get things done faster by sitting alone.
* Think where your team should apply this, it does not work when doing research.

**Also a few things about PRs and having to do reviews (aka Why I Hate Pull Requests):**

* PRs almost always arrive too late, too big. By the time the PR is made, it’s already based on subjective choices that could have been fixed by early comments instead. This easily ends up in a lot of rework and frustration.
* Reviewing PRs is really hard, especially when they arrive late. If it’s too big it’s really hard to focus on all the things that matter: design issues, making it more understandable for everyone, are we doing the right thing here, etc. If the PRs arrive too early, you miss the bigger picture unless the reviewer really knows the intent. If you decide “nah, it’s good enough”, you’re doing a bad review.
* When people submit PRs, they mentally consider the job “done”. You’re almost certainly going to hurt someone’s feelings if you do a thorough review and if there’s a lot of comments. Having to do rework on something already “done” is straining for both the author and the reviewer. This almost never happens when sitting together, and almost always happens when working separately.
* If you get negative / constructive criticism, next time you are going to postpone your PR even later, polishing the thing unnecessarily, because you want to do the job well to avoid the psychological pain. This doesn’t make the situation better, only worse.

### Customer

 In most companies, management is actually to blame for deliberately isolating engineers from discovering the customer's needs.

 Real customer needs happens over the lifetime of a project, and those discovered needs will necessarily change the quoted scope of work, this means that an MBA practice driven organization is going to shy away from a shifting scope project that discovers real customer needs. Instead they focus the engineering team on getting something Done™ by date certain. Where Done™ is a product no customer wants because discovery of real needs has been squelched. In addition the product is likely riddled with chaos because the team has been repeatedly focused on creating new features instead of characterizing their own work and removing the chaos. The only good thing about Done™ projects is they usually come with a release party that has pizza and cake - even better they come with at least tepid career advancement because the team did deliver by the agreed upon date - I mean, what was delivered didn't get adopted, but that won't matter until someone notices the lack of customer adoption, usually the CFO applying the 4X Rule, and cuts the group's budget.

> "Ford was able to significantly improve their quality by tasking managers with simply asking workers "how can this be done better?", listening to what they had to say and then supporting new, practical improvements to the manufacturing process. The prior approach was for the manager to think up improvements in abstraction - usually their boss's ideas - and push those ideas onto the workers. Today, this top down anti-pattern is repeated in management of software teams."

**Anti-patterns:**

* Developers that notice something is amiss with product/market fit are gently steered back to their keyboard to implement more features, with a promise that their concerns will be handled by the Idea Silo
* Development managers that try and understand the Big Picture of product/market fit, packaging, and pricing are patted on the head and sent back to focus the development team on implementing the scoped features that no customer wants
* Developers that wander into the field and notice that customers are really struggling to use the product are carefully steered back to the Idea Silo's agenda

[Source: "developers can't fix bad management"](https://iism.org/article/developers-can-t-fix-bad-management-57)
