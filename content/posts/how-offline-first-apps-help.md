+++
title = 'How Offline First Apps Improve UX'
date = 2024-08-12T14:10:46+05:30
draft = false
+++

In this post, I'll be discussing with a non-tech person how offline-first apps enhance user experience (UX).

## What is Offline First?

Offline first means that any action you take within the app is performed offline first, directly in your browser.
If there's an internet connection—which 96% of the people using our product have—we then apply those actions to our back-end.

So, the user sees the action being taken instantly, while the actual persistence of the action and the state is synced with the back-end and servers later, when possible.

## An Example: Status Change in Wokay Tasks

Let's consider an example where a user changes the status of a task in Wokay.

### What Do Traditional Web Apps Do in This Case?

- They send the event server-side and load a new HTML page based on that. (Hello! Ruby on Rails, Laravel).
- These days, after AJAX became popular, these frameworks have started to adopt AJAX asynchronous practices and update the state of the app.
  - However, they still first send the message to the server,
  - Show a loading indicator,
  - Then update the state.

These traditional methods mean that the user has to wait for the action to complete before they can proceed to the next task. In a fast-paced modern world, this isn't ideal.

### What Do We at Wokay Make the User Do?

- The user changes the status.
- We update the state of the task locally in the browser.
- We instantly show the updated state in the browser.
- We asynchronously send the message to the server.
- When the server returns a success message, all is well. We may show or not show a popup indicating that the task is complete.
- What if it fails?
  - We roll back the action to the previous state.
  - We must show a popup saying that the status update didn’t occur due to "this or that" problem and ask the user to try again.
- The benefits here?
  - For 95% of users, the action will succeed.
  - For the 5% where there is a failure, the action won't occur.
  - We are optimizing for the 95%.

### Conclusion

Traditionally, web apps were defensive:

- The current state of your app was always in sync with the true state in the database.

The problem with this approach is that each interaction trades off speed for accuracy.
Offline-first apps prioritize speed. Nowadays, internet connections are stable for those working in internet-based businesses.

So, we can safely assume that most of our users will be connected online since it's a SaaS product. Thus, the offline-first approach is a good fit for us.

---

Let's vow to never make slow apps again.
