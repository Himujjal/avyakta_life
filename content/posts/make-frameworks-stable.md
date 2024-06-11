+++
title = 'Make Frameworks Stable'
description = "Why don't devs make software that last long?"
date = 2024-03-29T01:15:38+05:30
draft = false
+++

# Software that lasts for years

`C`. Let's start with `C`, the grandpa of all languages. 3 years ago I got myself writing [tree-sitter-svelte](https://github.com/Himujjal/tree-sitter-svelte) && [Ekon](https://github.com/ekon-org/ekon). The projects aren't all original and written from scratch.
I had not done C programming since my `C` classes in University first year (It was 7 years before I started them). `C` is hard. But `C` is constant. It hasn't changed in over 40 years. Maybe one or two changes here and there. But once you learn it well, you
are good to go for the next decade at least. That tells something about `C`. It has its problems, but it is probably the greatest+simplest piece of software ever developed by human beings. It lasted for 50 years and will continue to do so for the next 20 years
until languages like `Zig` and `Rust` take its place. `React` and the front-end world learn nothing from here. They just want to make changes for the sake of it.

# React

### First time with React

I learnt it during my internship at a startup named [Plop](https://plopnow.com), where I had to make the dashboard for writers using Ant Design. I didn't know design patterns. I didn't know HOC, but within 2 months, I had made a great piece of software.
Back then, we used Webpack on my old Lenovo machine, used Class components, those long Redux stores etc. It was good. Except Redux, whose initially design was fuck-all. Seriously! looking back now, that was bad. I built an HOC back then with a basic minimal
Svelte Store (❤️) like design. But overall, the devex was only bad due to wonky HMR and no Vite. Class components once you learn them were just fine. The separation of concerns were very clear. I could make an app quite fast once learnt. I was young and quite the enthusiast
as well.

### Second time with React

The second time I had a stint with React was at [Spiralyze](https://spiralyze.com). I recreated the whole front-end including some complex user actions. It was great. I had my custom components made. The app was made. But this time I used functional components. I learnt
`useState`, `useRef` and all that shit. I didn't use much of hoooks. Didn't see much point of them. But then again, it was fine. I still made the app quite fast and functional. But once thing I picked up at this period was [Tailwind](https://tailwind.com) and React functional
components. I didn't really like them. I didn't see much point of making functions again and again and adding functions inside functions as event handlers and all. Who the fuck does that! Seriously. `Tailwind` was great. I used `Jotai` and it was great as well.

But it was at that time that I realized that early designs of the software or libraries you write has to be thought from the perspective of:

> Will this library/software design last for 20+ years? Will it be there for my children to see this through?

Software that lasts for long periods is very important.

Writing everything from scratch is not always a good thing to do.

### Third time with React

This time, and the time is now. I joined [Wokay](https://wokay.com). The whole paradigm of React programming I saw here thanks to Tushar was different. It was clean, yet so messy. Something was wrong. There were too many compositions.

# Speed of Rust

Talking about Rust has its fair share of problems. Rust moves fast. Unlike `C/C++` Rust adds almost a new change in its library. And at this pace, its going to be time till learning Rust will be unlearnable. You learn
Rust today, you will not identify newer Rust code maybe 5-10 years from now. Modern C++ vibes. Nonetheless, Rust is a great programming language.
