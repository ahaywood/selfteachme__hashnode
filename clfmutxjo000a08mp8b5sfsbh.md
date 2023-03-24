---
title: "Planning for Success: My Approach to Designing Applications"
seoDescription: "Learn how a UI flow diagram and Figma can help with designing applications, as demonstrated in the creation of the "Made with Xata" project."
datePublished: Fri Mar 24 2023 18:07:01 GMT+0000 (Coordinated Universal Time)
cuid: clfmutxjo000a08mp8b5sfsbh
slug: planning-for-success-my-approach-to-designing-applications
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679680609446/35bb9267-8b66-4489-afdb-431d1e5c4ca7.png
tags: ui, product-design, figma, ui-ux-designer

---

Last week, I started designing an application called **Made with Xata** where users will be able to share projects that they…well…made with [Xata](https://xata.io).

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679680655298/8f8d15c0-f52b-421b-b92f-953dbe7d6284.png align="center")

It’s funny, how you can start with a “simple” idea, like a gallery, and it quickly inflates into a much large project:

* We’re showcasing projects, how do those projects get added?
    
* Once the projects are added, someone will need to approve those projects before they go live on the site. That means we’ll need an admin screen and users.
    
* Now, we’re talking about authentication, which means a user will also need to be able to do all the standard stuff: forgot password, reset password, logout. Not to mention, managing their account. Or, approving a user’s account, granting them access.
    
* Are we showing profile pictures (avatars) for each user? We need to store those images somewhere.
    
* What if an entry changes? Or, there’s a typo that needs to be corrected? We need a way to manage the information.
    

Suddenly, we have a lot of features that we need to take into consideration. 😅

### UI Flow Diagram

Anytime I start building an application and thinking through all the various states, one of the tools that I’ll reach for is a UI Flow diagram. Web applications are different than marketing sites. — Granted the lines are blurring, but generally a web application has multiple states within each page, dependent on a user’s interaction. Therefore, a UI Flow diagram displays more information than the traditional site map.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679680713868/d5a32653-fd1e-4db5-b9c6-6b7f06942ff4.png align="center")

This helps illustrate how all the data that flows through the application.

* Where are users entering the application?
    
* What decisions are being made?
    
* What the jobs that a user is trying to accomplish?
    
* How is the user moving through the application? How many clicks does it take to accomplish their goal?
    
* What happens when the user follows the happy path? What are the edge cases?
    
* Where can guests go? Where can logged-in users go?
    

### Stubbing out a New Project within Figma

Once the UI Flow Diagram is in a good place, I started designing screens within Figma. If it were a larger application, I would have started with low fidelity wireframes instead. But, this is a smaller project and an area where I could save a little bit of time.

One of the hardest parts in design is getting started. This project was a little easier because it matches Xata’s existing branding and there were existing design patterns that I could reference. I went through their entire site, looking at typography, iconography, and various treatments, taking screenshots as I went.

I’ve always been able to overcome a blank canvas, by dumping all my reference images and branding elements on the screen. Then, it feels like I’m trying to solve a puzzle instead of building something from scratch.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679680986481/692d990a-8f25-4294-9878-ee8b0f89ca6e.png align="center")

Sometimes, it’s about building momentum, going through the motions, and starting with something easy. This can be as simple as setting up the page structure within Figma.

I organize every project the same way. This level of consistency makes it easy to come back to projects and easily find what I’m looking for.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679681022674/11c8cdab-b4df-45f4-ba50-7f04493d11b0.png align="center")

Another tip? Don’t always start with the “thing” that makes the most sense. Logically, I should start at the top and work my way down the page. Or, start with the hero or the featured section, building supporting elements around it. But, those can also be the hardest sections to put together, especially when you’re still trying to build a library of styles and components.

A lot of times, I’ll start with the footer, because it’s one of the easiest elements to design. I know I need the copyright information, links to the legal pages, and social media icons.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679681089136/d83a1c52-8a13-4f52-b7df-36084991d1ab.png align="center")

*Disclaimer: I didn't design this footer* ☝️

I’ve come to realize that a big difference between juniors and seniors is that seniors have developed a process that they know works for them. I’m a designer, but I don’t *feel* creative every single day. I’m not sitting around waiting for inspiration to strike. But, I have routines and processes in place that help me produce results regardless of what mood I’m in.

So, if you’re interested in following along, I’m designing and building as much of this project in public. I’m [live streaming three days at week on Twitch](https://twitch.tv/selfteachme), blogging here on Hashnode, and [dropping videos on YouTube](https://youtube.com/c/selfteachme). I’ve also put a project page together in [Notion to track progress](https://www.notion.so/Project-Page-Made-with-Xata-e1c3579bb49e4713bdd7a77b2e6f415a). All code is [open source and on GitHub](https://github.com/ahaywood/made-with-xata).