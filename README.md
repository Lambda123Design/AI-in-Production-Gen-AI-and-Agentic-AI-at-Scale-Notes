# AI-in-Production-Gen-AI-and-Agentic-AI-at-Scale---Notes
This Repository contains my Udemy course notes of "AI in Production: Gen AI and Agentic AI at Scale" by Ed Donner

**Table of Contents:**

**I) Week 1**

**A) Day 1 - Instant AI Deployment: Your First Production App on Vercel in Minutes**

**B) Day 1 - From Zero to Live: Deploying Your First AI-Powered SaaS on Vercel**

**C) Day 1 - From AI Concepts to Cloud Deployment: Navigating the DevOps Landscape**

**D) Day 1 - Course Overview: Building Production AI Systems Across 4 Weeks**

**E) Day 1 - Deploy Your First Live AI App with OpenAI and Vercel Integration**

**F) Day 1 - Managing API Costs and Environment Setup for Production AI Systems**

**G) Day 1 - Course Expectations and Community Support for Production AI**



# **A) Day 1 - Instant AI Deployment: Your First Production App on Vercel in Minutes**

This is a big moment. This is the start of the juiciest course I've ever made. Welcome to the beginning of generative AI and Agentic AI in production, week one, day one. The next four weeks are about taking AI and putting it into production, making it production grade.

But wait, before we get started, I must stop you right there. It is super important in these kinds of courses to begin with objectives, introduction, curriculum, and logistics to set you up for success. But no, people have taken my courses before. Know that that is not my style. It's not my jam. We will not start with objectives or introduction or curriculum or logistics. We will start with instant gratification by getting straight into it. Let's go ahead.

Before we do any talking, let's deploy something to production right now. And so let's get to it. Instant gratification. We're going to begin in a web page, in a GitHub web page at this site: github.com. I'm going to put this link wherever I possibly can so you find it easy to find. It should be in the Udemy resources. If you can't find it, then you might have to type it in, but it will be there somewhere. Look for it: Editor Donna Production. That's the repo in GitHub. Go into the folder called "week one" and then look at the file called "day one instant gratification."

Let me tell you two things right away. First, what you see when you do this might look different from what I've got in the videos, and that's because I constantly update this as people encounter any snafus doing this. I will keep it up to date and with the latest information. So what you see might be richer than what I show in the video. It will only be improved, so don't worry if it looks a bit different. Also, as we go through these instructions, when you do it, if you have a slightly different experience on a different website, then don't worry about it. It's possible that in different regions, some of these websites look a bit different. It's also possible that they've changed over time. See if it fits. Easy to figure out what you're supposed to do. Just read the cues from the screen, follow along, and if not, message me in Udemy and we'll figure it out together.

All right, with that in mind, let's get to instant gratification. We are going to make a production deployment in a matter of minutes. Step one is to sign up for something called Vercel. You may be wondering what Vercel is. You'll see it in just a second. Follow this link here to Vercel. Vercel allows you to build and deploy on the cloud. It's an incredibly easy-to-use cloud infrastructure service that lets you build and scale AI apps and deploy them really, really quickly.

The first thing we're going to do is click "Sign Up." It says, "Your first deploy is just a sign up away." I'm going to set it to personal projects. I give myself a name, say continue, and then you get an authentication screen where you can choose to authenticate using Google, GitHub, GitLab, or Bitbucket. Pick your poison, go through, sign up for an account, and then follow the rest of the instructions that are on the GitHub page. You should now have your own Vercel account.

Next step is to install the IDE that we will use, which is Cursor. For those who were on my Agentic course, you're already familiar with this. For others, here are the instructions to install Cursor. If you'd rather use a different IDE, that's totally fine; any IDE will do. If you use something like VSCode, Cursor is itself a fork of VSCode, as is Windsurf, so it will be very familiar. Visit Cursor and press the download button. For Mac, download for Mac OS; for Windows, download for Windows. Follow the installation wizard, selecting defaults. Once installed, open up Cursor in a terminal and create a new project by clicking "New," and we will create one called "Instant."

When you open up Cursor, it might look like this, or you might have to go to File → New Window. Press the "Open Project" button. In the dialog, create your project somewhere—it's normal to have a folder called "projects" within your home directory. Create a new folder and call it "instant." Open it, and now you have a new fresh project ready for work. Close the chat screen in Cursor; we're focusing on the Instant Project and following the instructions in GitHub.

Step three is to create a FastAPI application. FastAPI is a Python server that acts as an app server. It can respond to different web requests by running Python code. In this case, it's a simple server responding to the slash route, returning the text "live from production." Copy the code from GitHub, create a new file called instant.py in Cursor, paste the code, and save the file. Remember, saving is crucial; it's not like a Google doc.

Next, create a requirements.txt file with the listed contents: FastAPI and uvicorn. This file lists Python package dependencies. Save it. Then, create a file called vercel.json where we define the Vercel project configuration. Paste in the contents and save it. The JSON has sections on builds and routes, indicating that any incoming requests will be handled by instant.py.

Step six: install Node. If you don’t have it installed, download it from the official Node website, stick with defaults unless you know otherwise, and install it. Open a terminal in Cursor (Ctrl + backtick on Windows or Command + backtick on Mac) and check Node installation using node --version and npm --version.

Next, install Vercel using npm. While it's installing, don't worry too much about warnings—they happen all the time. Then run vercel login to log in with the method you used to sign up. Finally, the moment of truth: run vercel . while in the project folder. Follow the prompts: select scope, create a new project (name it "instant" or anything you like), confirm the code directory, and skip additional settings. Vercel creates necessary files and deploys the project.

Once deployed, you'll see information about your deployment including a URL. Click the URL (Command + click on Mac, Control + click on Windows) to open it in a browser. You should see "live from production," confirming that you have deployed to production online. You could be forgiven for thinking this isn't yet an AI app per se; it’s just the first step. This is the foundation for deploying your first production AI app. We'll build on this in the next video.

**B) Day 1 - From Zero to Live: Deploying Your First AI-Powered SaaS on Vercel**

Now, I appreciate that some of you have seen Vercel before and deployed your own projects and are probably thinking, “Ah, this is small potatoes.” Maybe it is, maybe not yet mind-blowing. But hopefully, for those new to it, you were pleased to see that it’s really not that hard.

If we go back to Cursor, in addition to the link to production, there was another link called "Inspect." I want to take you through that command. Click the link, and it shows us the screen in Vercel where we can look at our deployment, seeing a little preview right there. One thing you might have noticed is that when you went to this web page, you actually had to be signed in to Vercel to access it. You could argue that it’s not really live on the internet if you need to be signed into Vercel, but we can change that. If you expand the deployment configuration section, you’ll see deployment protection is turned on. Clicking that takes us to the settings page, where Vercel authentication ensures visitors need to be logged in and a member of our team. Unfortunately, only we could see this right now, but luckily, we can turn it off, press save, and it confirms the change. Now, for example, copy this URL to a new incognito window in Chrome, and you'll see "live from production" being served to anyone on the internet. There we are—live on the internet in minutes. Never fear, we’ll be coming back to add a healthy dose of artificial intelligence soon.

This is what I have in store for you. We are going to do some hardcore learning. This is probably the most intensive course I’ve ever made. It’s all in four weeks, but I have packed it full. We’ll work on some of the juiciest projects I’ve ever built—very commercial, very hands-on, really interesting, and quite challenging. At the same time, I hope to make it fun. That’s my vibe: making sure it’s entertaining as well as educational. Hopefully, you’ll enjoy building things that are scalable, resilient, and secure.

Let me tell you about the objectives, who the course is for, and how you’ll know you’ve been successful at the end. There are really two main audiences for this course. First, entrepreneurs. If you want to take a SaaS app and deploy it online on the internet—with authentication, SSL, subscriptions, and a secure, scalable setup—then this course is for you. The first week is the most intense because we’ll do all of that and then build on it. Second, if you want enterprise-level knowledge on AI deployed in the cloud for scale and resiliency—working with major cloud providers like AWS, GCP, and Azure, and gaining relevant expertise to apply for roles that require this—then this course is also for you.

That said, there’s a continuum of people between these two extremes. Maybe you want to be an entrepreneur but currently work at a company. Maybe you’re in a medium-sized company and want to deploy for future growth. Maybe you want to beef up your resume to apply for more roles. If you’re anywhere on that spectrum, this course is designed for you.

So, what will you get out of it at the end? What are the success factors? There are three main outcomes. First, for the entrepreneur, you should be able to deploy, monetize, and make money from your own AI application. Of course, you’ll need product-market fit—I can’t promise people will pay for it—but the technology side will be solved. Second, you’ll be able to implement production-grade AI at major companies, gaining transferable skills that you can apply in different situations. I focus on transferable skills and common platforms and frameworks so you’ll have that capability. Third, you’ll be able to apply for roles that require this skill set. I’ve reviewed many job descriptions and, as a hiring manager myself, know what’s needed. Other courses cover a lot, but one piece often missing is AI productionization—and that’s exactly what you’ll gain from this course.

That said, the course alone won’t do it. You’ll need to complete the assignments as we go. The best way to learn is by doing. Listening to me isn’t enough; you need to actively engage. When you get stuck, that’s when the real learning happens. You need to complete the projects with me, fix the problems when they arise, make the projects your own, add your own flair, and take on the assignments I give you. That’s the real way to learn. The videos and instructions are just the foundation—the part that matters is what you do.

**C) Day 1 - From AI Concepts to Cloud Deployment: Navigating the DevOps Landscape**

And now let me introduce myself to convince you that I’m actually qualified to talk to you about this. With apologies to those who have heard my intro about three times before, it’s going to be exactly the same and make the same jokes—just put me on two-times speed if you like. For those new to me, I’m Ed Donner. I am the co-founder and CTO of an AI startup called Nebula. Go check us out. Most of my career was at JP Morgan, where I ended up as an MD leading a team of about 300 technologists. I started out in London, which is where I’m from originally, as you can probably tell from my accent. I spent a few great months in Tokyo, and then ended up in NYC, where I live now.

Before Nebula, I founded an AI startup called Untapped, which was acquired a few years ago. There’s a picture from Times Square showing our acquisition announcement—a magical moment for me. If you squint carefully, you can even see a few pixels of me in the image. A bit of a leap of faith, but that is indeed me on the Times Square billboard at that moment. The other reason I show this photo is not just to boast, but also because I actually live about a block from Times Square, behind that guitar you see in the picture. While I’m in London right now, when I’m in New York, you can find me right there looking out at you.

It’s customary with these things to show a personal picture or a hobby. Here’s a picture of me in front of a plane I just flew. You might think I’m skilled at this, but quite the contrary. My skills with LMS are only surpassed by my complete inability to do anything requiring hand-eye coordination. If you ever see me in a cockpit ready to control a plane, you’ll want to look for a parachute quickly. However, if you’re here to take a course on building and deploying LMS, generative AI, and AI in production, then luckily, that is exactly my skill set. Let’s get on with the course.

You might be wondering how this course fits with my other courses. My first course was LLM Engineering, which teaches the foundations of AI engineering—how to select and apply LLMs, how to do things like RAG and fine-tuning, and covers the foundations of generative AI. Shortly after that, I made a companion course that goes deeper into the field of generative AI. These courses are designed as companions: you can take them in either order, one, or both. The AI in Production course sits on top of these two. You don’t need to have taken them, though prior knowledge on RAG and fine-tuning will help you follow along more smoothly. In this course, we won’t be coding things like RAG; instead, we’ll use pre-built components for data ingestion and storage in vector databases, and I’ll guide you through it.

I also have another course called the AI Briefing for Founders and Leaders. This is my only course that isn’t technical—it’s commercial and intended for people who want to understand how to build durable, valuable AI-driven businesses. Some participants in this course may benefit from it, particularly if they’re looking to commercialize LLMs. All my courses are complementary, with minimal overlap, and can be taken in any order. A natural progression might be LLM Engineering for foundations, Generative AI for application, and then AI in Production for deployment.

I aim for my courses to appeal to a wide range of backgrounds. For some, parts may be too fast or complex, in which case take it slow and explore the material yourself. For others, parts may be too simple—deploying to Vercel may be familiar—so you can speed through those sections. I want to set your expectations: this course is highly requested, and many people may have misconceptions about it. When people think of deploying AI software to production, they might expect a course heavily focused on AI concerns. While AI is certainly part of it, 70–80% of this course is actually about platform engineering—DevOps, configuring cloud providers, and production deployment. Whether the Python code is a simple "hello from production" or calling an LLM, the bulk of your work now is infrastructure, not AI per se.

Throughout this course, we will maintain an AI lens. We will work with vector databases and APIs like Bedrock and SageMaker, but much of the work is traditional cloud platform engineering. We’ll cover observability, deploying MCP servers, and other relevant practices, but platform engineering is the majority of what you’ll learn. I have structured this course to follow a T-shaped learning approach: covering breadth across cloud providers, CI/CD, GitHub Actions, and going deep in one area—AWS—since it is the most common in industry. While we’ll touch on Google Cloud and Azure, the focus is AWS to best prepare you for industry standards, and I’ll highlight parallels between providers as we go.

**D) Day 1 - Course Overview: Building Production AI Systems Across 4 Weeks**

**E) Day 1 - Deploy Your First Live AI App with OpenAI and Vercel Integration**

**F) Day 1 - Managing API Costs and Environment Setup for Production AI Systems**

**G) Day 1 - Course Expectations and Community Support for Production AI**




