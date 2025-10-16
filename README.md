# AI-in-Production-Gen-AI-and-Agentic-AI-at-Scale-Notes
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

**H) Day 2 - Building Full-Stack AI Apps: Frontend-Backend Architecture for LLMs**

**I) Day 2 - Building Full-Stack AI Apps with React, FastAPI, and NextJS**

**J) Day 2 - Building Your First Full-Stack AI SaaS with NextJS and FastAPI**

**K) Day 2 - Building Your First FastAPI Backend for Production LLM Deployment**

**L) Day 2 - Deploying Full-Stack AI Apps with Next.js Frontend and FastAPI Backend**

**M) Day 2 - Adding Real-Time Streaming and Professional UI to Your LLM App**

**N) Day 3 - Adding User Authentication to Your Production AI Application**

**O) Day 3 - Adding User Authentication to Production AI Apps with Clerk**

**P) Day 3 - Adding Subscription Billing to Your Production AI SaaS Application**

**Q) Day 3 - Adding Authentication and Billing to Production AI Applications**



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

# **B) Day 1 - From Zero to Live: Deploying Your First AI-Powered SaaS on Vercel**

Now, I appreciate that some of you have seen Vercel before and deployed your own projects and are probably thinking, “Ah, this is small potatoes.” Maybe it is, maybe not yet mind-blowing. But hopefully, for those new to it, you were pleased to see that it’s really not that hard.

If we go back to Cursor, in addition to the link to production, there was another link called "Inspect." I want to take you through that command. Click the link, and it shows us the screen in Vercel where we can look at our deployment, seeing a little preview right there. One thing you might have noticed is that when you went to this web page, you actually had to be signed in to Vercel to access it. You could argue that it’s not really live on the internet if you need to be signed into Vercel, but we can change that. If you expand the deployment configuration section, you’ll see deployment protection is turned on. Clicking that takes us to the settings page, where Vercel authentication ensures visitors need to be logged in and a member of our team. Unfortunately, only we could see this right now, but luckily, we can turn it off, press save, and it confirms the change. Now, for example, copy this URL to a new incognito window in Chrome, and you'll see "live from production" being served to anyone on the internet. There we are—live on the internet in minutes. Never fear, we’ll be coming back to add a healthy dose of artificial intelligence soon.

This is what I have in store for you. We are going to do some hardcore learning. This is probably the most intensive course I’ve ever made. It’s all in four weeks, but I have packed it full. We’ll work on some of the juiciest projects I’ve ever built—very commercial, very hands-on, really interesting, and quite challenging. At the same time, I hope to make it fun. That’s my vibe: making sure it’s entertaining as well as educational. Hopefully, you’ll enjoy building things that are scalable, resilient, and secure.

Let me tell you about the objectives, who the course is for, and how you’ll know you’ve been successful at the end. There are really two main audiences for this course. First, entrepreneurs. If you want to take a SaaS app and deploy it online on the internet—with authentication, SSL, subscriptions, and a secure, scalable setup—then this course is for you. The first week is the most intense because we’ll do all of that and then build on it. Second, if you want enterprise-level knowledge on AI deployed in the cloud for scale and resiliency—working with major cloud providers like AWS, GCP, and Azure, and gaining relevant expertise to apply for roles that require this—then this course is also for you.

That said, there’s a continuum of people between these two extremes. Maybe you want to be an entrepreneur but currently work at a company. Maybe you’re in a medium-sized company and want to deploy for future growth. Maybe you want to beef up your resume to apply for more roles. If you’re anywhere on that spectrum, this course is designed for you.

So, what will you get out of it at the end? What are the success factors? There are three main outcomes. First, for the entrepreneur, you should be able to deploy, monetize, and make money from your own AI application. Of course, you’ll need product-market fit—I can’t promise people will pay for it—but the technology side will be solved. Second, you’ll be able to implement production-grade AI at major companies, gaining transferable skills that you can apply in different situations. I focus on transferable skills and common platforms and frameworks so you’ll have that capability. Third, you’ll be able to apply for roles that require this skill set. I’ve reviewed many job descriptions and, as a hiring manager myself, know what’s needed. Other courses cover a lot, but one piece often missing is AI productionization—and that’s exactly what you’ll gain from this course.

That said, the course alone won’t do it. You’ll need to complete the assignments as we go. The best way to learn is by doing. Listening to me isn’t enough; you need to actively engage. When you get stuck, that’s when the real learning happens. You need to complete the projects with me, fix the problems when they arise, make the projects your own, add your own flair, and take on the assignments I give you. That’s the real way to learn. The videos and instructions are just the foundation—the part that matters is what you do.

# **C) Day 1 - From AI Concepts to Cloud Deployment: Navigating the DevOps Landscape**

And now let me introduce myself to convince you that I’m actually qualified to talk to you about this. With apologies to those who have heard my intro about three times before, it’s going to be exactly the same and make the same jokes—just put me on two-times speed if you like. For those new to me, I’m Ed Donner. I am the co-founder and CTO of an AI startup called Nebula. Go check us out. Most of my career was at JP Morgan, where I ended up as an MD leading a team of about 300 technologists. I started out in London, which is where I’m from originally, as you can probably tell from my accent. I spent a few great months in Tokyo, and then ended up in NYC, where I live now.

Before Nebula, I founded an AI startup called Untapped, which was acquired a few years ago. There’s a picture from Times Square showing our acquisition announcement—a magical moment for me. If you squint carefully, you can even see a few pixels of me in the image. A bit of a leap of faith, but that is indeed me on the Times Square billboard at that moment. The other reason I show this photo is not just to boast, but also because I actually live about a block from Times Square, behind that guitar you see in the picture. While I’m in London right now, when I’m in New York, you can find me right there looking out at you.

It’s customary with these things to show a personal picture or a hobby. Here’s a picture of me in front of a plane I just flew. You might think I’m skilled at this, but quite the contrary. My skills with LMS are only surpassed by my complete inability to do anything requiring hand-eye coordination. If you ever see me in a cockpit ready to control a plane, you’ll want to look for a parachute quickly. However, if you’re here to take a course on building and deploying LMS, generative AI, and AI in production, then luckily, that is exactly my skill set. Let’s get on with the course.

You might be wondering how this course fits with my other courses. My first course was LLM Engineering, which teaches the foundations of AI engineering—how to select and apply LLMs, how to do things like RAG and fine-tuning, and covers the foundations of generative AI. Shortly after that, I made a companion course that goes deeper into the field of generative AI. These courses are designed as companions: you can take them in either order, one, or both. The AI in Production course sits on top of these two. You don’t need to have taken them, though prior knowledge on RAG and fine-tuning will help you follow along more smoothly. In this course, we won’t be coding things like RAG; instead, we’ll use pre-built components for data ingestion and storage in vector databases, and I’ll guide you through it.

I also have another course called the AI Briefing for Founders and Leaders. This is my only course that isn’t technical—it’s commercial and intended for people who want to understand how to build durable, valuable AI-driven businesses. Some participants in this course may benefit from it, particularly if they’re looking to commercialize LLMs. All my courses are complementary, with minimal overlap, and can be taken in any order. A natural progression might be LLM Engineering for foundations, Generative AI for application, and then AI in Production for deployment.

I aim for my courses to appeal to a wide range of backgrounds. For some, parts may be too fast or complex, in which case take it slow and explore the material yourself. For others, parts may be too simple—deploying to Vercel may be familiar—so you can speed through those sections. I want to set your expectations: this course is highly requested, and many people may have misconceptions about it. When people think of deploying AI software to production, they might expect a course heavily focused on AI concerns. While AI is certainly part of it, 70–80% of this course is actually about platform engineering—DevOps, configuring cloud providers, and production deployment. Whether the Python code is a simple "hello from production" or calling an LLM, the bulk of your work now is infrastructure, not AI per se.

Throughout this course, we will maintain an AI lens. We will work with vector databases and APIs like Bedrock and SageMaker, but much of the work is traditional cloud platform engineering. We’ll cover observability, deploying MCP servers, and other relevant practices, but platform engineering is the majority of what you’ll learn. I have structured this course to follow a T-shaped learning approach: covering breadth across cloud providers, CI/CD, GitHub Actions, and going deep in one area—AWS—since it is the most common in industry. While we’ll touch on Google Cloud and Azure, the focus is AWS to best prepare you for industry standards, and I’ll highlight parallels between providers as we go.

# **D) Day 1 - Course Overview: Building Production AI Systems Across 4 Weeks**

And now I'm excited to unveil our four-week curriculum to become production grade. As usual with my courses, I've organized this into four different modules, one for each week. The first week is focused on building a SaaS project that you deploy onto the internet, including features like authentication and subscription.

In the second week, we’re going to focus on AWS, drilling down on platform engineering for an AI project deployed on AWS. We’ll cover a wide range of AWS concerns, leaving you able to deploy your own projects and at least familiar with the components we don’t touch. This will include infrastructure as code and CI/CD.

The third week will involve a variety of activities related to AI projects. We’ll first take a look at Azure and GCP so that you’ve explored all the major providers. We’ll focus on data engineering by building ingest pipelines, and we’ll examine vector stores and MCP so that you can deploy an agent with MCP servers behind it.

In the fourth week, we turn to Agentic AI. We’ll build and deploy a multi-agent system in production, which will lead to the capstone project and the conclusion of the four weeks. Each of these four modules represents a week of learning together on this journey, with five days in each week representing the different components of the course.

In the first week, which we’re currently in, we’ll build up an app with a front end and back end, implement authentication and subscriptions, and create a healthcare SaaS app. This app will first be deployed to Vercel, and then we’ll perform our first deployment to AWS. In the second week, we’ll discuss AWS architecture, revisit a project from one of my previous courses called The Digital Twin, and create a new version of it. We’ll use Bedrock, add Terraform for infrastructure as code, and GitHub Actions to establish a robust production deployment pipeline.

Week three is a mixed bag of activities. We’ll start a new project, the Cyber Security Analyst, and deploy it on Azure and GCP using MCP servers. We’ll then use AWS SageMaker and build data ingest pipelines using S3, vectors, and MCP servers. The final week, “Gigantic AI in Production,” focuses on multi-agent deployments. We’ll work on the capstone project, including the front end, and integrate observability, monitoring, and security—three crucial aspects of AI and Agentic AI deployments. We’ll also explore Agentic AI platforms, which are extremely relevant and hot in the industry right now.

The capstone project we’ll work on is designed to be a commercial-ready product, with opportunities for you to add your own elements and potentially monetize it. It will be an agentic financial planner SaaS product, allowing users to enter details about accounts, investments, equity portfolios, and retirement accounts. The system will provide advice on rebalancing portfolios and retirement prospects. This fully functioning Agentic app will have different agents working in concert to add value and be useful for the user community, while allowing you to customize and deploy it.

You may be wondering about the different colored tiles in the curriculum overview. The yellow tiles represent DevOps and platform engineering concerns. Blue tiles denote projects, including the healthcare app, Digital Twin Mark II, and the capstone project. The Cyber Security project is small and doesn’t get a blue square, but it’s still counted among the four projects. Purple squares indicate AI-related content. Even though today we haven’t yet focused on AI, the day is young. Remember, only 20% of the course is AI, but there are plenty of purple squares throughout. Even AI components like Bedrock and SageMaker involve significant DevOps work, but the purple tiles confirm the AI focus.

By the end of these four weeks, having completed your projects and assignments, you’ll be well-deserving of the recognition and cup at the end. More importantly, you’ll have acquired the skills to independently deploy commercial LM products, Gemini, and Agentic AI into production. This course has a fairly comprehensive scope, though production deployment is an enormous field, so some areas are beyond our focus. We primarily work on AWS while touching on other providers. Our focus is on transferable, industry-standard skills. For example, for infrastructure as code, we’ll use Terraform rather than Amazon CDK, as it applies across AWS, GCP, and Azure. Similarly, for authentication, we use Clerk, which is provider-agnostic.

We’ll touch on front-end development and Docker containers, but only at a surface level. Entire courses exist on front-end development and Docker, and we won’t go deep here, though self-study guides will be provided. You’ll still have the code available, but for any significant changes, large language models can assist. The goal is to provide you the tools to apply principles learned here to other components, providers, and APIs. After repeating these practices across multiple projects, you’ll develop the ability to research and integrate services independently.

In summary, our goal is to cover a focused subset of production deployment concepts while enabling you to generalize these skills to other contexts. I’ve been talking long enough—now it’s time to do some hands-on work. Let’s go back and add some AI spice to our simple production application.

# **E) Day 1 - Deploy Your First Live AI App with OpenAI and Vercel Integration**

So here I am back on GitHub at github.com, and we’re navigating to week one, specifically week one/day one.part 2.md, which is our Instant Gratification Project Part Two. The first step is to set up an OpenAI API key, as we’ll be making calls to GPT-5. I realize that some of you may already have OpenAI keys, in which case you can skip step one. Others may not have a key or may not want one, since OpenAI requires a $5 upfront payment, which you spend as you go. While the cost is minimal—a fraction of a cent per call—it can still be a consideration for those using multiple APIs. There are free and cheap alternatives that don’t require this upfront payment, and these are carefully noted in the guides folder in the documentation. The guides explain how you can modify the instructions if you choose one of these alternatives.

Assuming you decide to proceed with OpenAI, it’s a good experience to understand how to set up a key and use it, as it’s very common in industry. To get started, visit platforms.openai.com to sign up for an account. If you’re unsure about the difference between ChatGPT the product and using the OpenAI API, this is also covered in the docs. Once signed up, you may need to create an organization, authenticate using Google or other methods, and add your $5 minimum payment. Make sure auto-recharge is turned off to avoid unintended charges. Next, create a new API key by selecting Create secret new secret key, which will usually start with src-proj-. Copy this key to your clipboard and store it safely, ideally in a password manager. If you save it in a text editor, use a plain editor rather than something like Microsoft Word, as word processors may alter characters like dashes.

Once you have your OpenAI key, it’s time to add it to Vercel. The instructions indicate running the command "vercel env add OpenAI_API_key" in Cursor. When prompted, paste in your key, making sure it starts with src-proj- and has no trailing spaces. Next, select which environment the key applies to; for this course, choose all environments by pressing A when prompted or by using space and arrow keys. If a mistake is made, you can always repeat this process. At this point, we’ve successfully set environment variables in Vercel.

The next step is updating our dependencies. In requirements.txt, where we’ve already listed Python libraries like fastapi and uvicorn, we now add "openai" to include the OpenAI Python client library. It’s important to note that this library does not contain any LLM code; it’s an open-source utility provided by OpenAI that constructs HTTP requests and converts responses into Python objects. This wrapper allows us to interact with OpenAI models or even other LLM providers. My guide explains how to use alternative providers while still using this same library.

Now we move on to updating our application code. From GitHub, copy the new code and paste it into instant.py in Cursor, replacing the existing code. This code uses FastAPI and defines a single route that will be called when someone visits it. It creates a new instance of OpenAI using the Python utility, constructs a message prompt: "You're on a website that's just been deployed to production for the first time. Please reply with an enthusiastic announcement to welcome visitors to the site, explaining that it's live on production for the first time." You can customize this message as desired. This message is wrapped in a list of dictionaries with "role": "user" and "content" set to the message.

The response is generated with "client.completions.create" using the lightweight GPT-5 nano model, passing in the messages. The returned content is accessed with "response.choices[0].message.content". Any carriage returns in the response are replaced with an HTML line break tag <br/>. We then construct an HTML string for the webpage with a title and body containing the AI-generated reply. Always save the page before proceeding.

Finally, deploy the project with "vercel deploy". The build process runs, and shortly we’ll have our first AI project live on the internet. Opening the preview shows a generated announcement, like: "Ha. Welcome to our brand new site with a lovely emoji. Now live in production for the very first time, we're thrilled to announce that our production deployment is live! This milestone means real users, real data, and our real working product." GPT-5 has provided an enthusiastic introduction, which may be formal, snarky, or playful depending on your input. Although Vercel calls this a preview, the project is live and accessible online. To safeguard your $5 credit, you can restrict access via Vercel authentication, though with it off, anyone can interact with your generative AI deployment.

# **F) Day 1 - Managing API Costs and Environment Setup for Production AI Systems**

It’s almost a wrap for our first day together on this journey, and I have two more important messages for you. I know you may be a little tired of messages, but these are crucial, so please pay attention. The first message is about API costs, which is extremely important. You are in complete control of your API spending and have full freedom to decide whether to spend nothing or some amount. At the same time, you are responsible for managing these costs. Most of the things we do in this course are free, and I will highlight them as we go. Some activities, particularly those involving AWS, may incur small charges. For example, AWS Lambda offers a generous free tier, so most of what we do there won’t cost anything. Overall, for the entire course, the expenses should remain around $5, maybe up to $10 if you choose to go beyond the basics. The cost could increase if you decide to register your own domains, but this is optional and entirely your choice.

Regarding the $5–$10 range I mentioned, this is not guaranteed, and it’s important to understand that most major cloud providers, such as AWS, GCP, and Azure, do not operate the same way OpenAI does. OpenAI allows a simple pay-as-you-go approach, but enterprise cloud providers require a credit card and accumulate charges without a hard cap. While you can set alerts and quotas, there is no automatic stop, so monitoring your spending is your responsibility. You can always choose not to spend anything, and even when optional costs arise, you can skip them and still gain valuable learning. API costs must always be monitored carefully, and I will show you how to track them and set alerts. Unlike OpenAI, mainstream cloud platforms rarely offer hard caps, so vigilance is essential.

The second message is a lighter, though equally important, one about the challenges of environment setup. In my other courses, the first few days involve installing software, configuring keys, setting up APIs, and similar activities. These setup tasks make up less than 20% of the course time, but they generate about 80% of the questions I receive. Questions about interesting aspects of LLM usage are usually positive and friendly, but environment setup questions often come from frustrated learners. Some students even feel like giving up when things don’t work as expected. I recall one student who was extremely frustrated because his OpenAI API key wouldn’t work. After much discussion, it turned out he had misspelled "OpenAI_API_key" as "open_API_key". This is a common trap, and while it may feel discouraging, these experiences are part of the learning process.

Environment setup can be tricky. Simple typos, overlooked hyphens, or architectural mismatches can cause hours of debugging. For example, I once deployed a binary from my Mac to AWS, and it failed because of system architecture differences. The error message referenced "pedantic", which seemed unrelated and misleading, causing a multi-day troubleshooting process. Everyone will encounter unique issues during setup, and a big part of learning is developing the skill to identify the root cause when error messages are confusing.

This brings me to the course’s terms of service, which I ask you to accept. There are five key commitments. First, embrace roadblocks with enthusiasm and a positive attitude. These challenges are frustrating, but they’re where real learning occurs, even for experienced professionals. Second, when you encounter problems, roll up your sleeves and dig in. Experiment, research, post on forums or Stack Overflow, and investigate the issue thoroughly, because solutions often require deep exploration. Use LLMs like ChatGPT or Claude to assist you by pasting stack traces or error messages, but remember that LLMs have limitations and blind spots. They often provide outdated model names or suggest surface-level fixes rather than addressing the root cause.

For example, during my Mac-to-AWS deployment issue, LLMs initially suggested workarounds for the pedantic error rather than recognizing that the root cause was an architecture mismatch. Only after carefully analyzing the situation did I identify the true problem. LLMs are excellent tools, but context is key. Always provide them with full context and emphasize that the goal is to find the underlying problem, not just patch the immediate error. Developing this habit of analyzing root causes and considering the bigger picture is essential for troubleshooting and problem-solving throughout the course.

# **G) Day 1 - Course Expectations and Community Support for Production AI**

The fourth term asks you to acknowledge that if you post issues on Udemy, I will always try to help. However, my assistance may not be as straightforward as with my other courses because this course involves complex environment setups. In my other courses, when students post problems, they are usually about code that I can reproduce and fix quickly. In this course, many issues relate to your environment, setup, and accounts, which I may not be able to replicate exactly. I can provide hints and guidance, but it may be harder for me to give direct step-by-step instructions. You should still post your questions, and I will do my best to help, but recognize that you may need to persist longer than before. If at any point you feel that a particular setup, such as Azure, is not worth the effort, you can switch to alternatives like GCP. You can always follow along with the videos to absorb the learning even if you hit a roadblock.

I also encourage you to actively engage with the Udemy Q&A. When you solve a problem, post your solution to help others, and look for questions from other students that you might be able to assist with. This is especially valuable in this course because students have different systems and may encounter unique issues. Supporting each other in the community can make a significant difference, and this is more critical here than in any of my previous courses. By helping others, you reinforce your own learning and create a collaborative environment where everyone benefits.

To formalize this, I am piloting a new feature in Udemy that allows more interaction between you and the course. I would like you to review these five terms carefully, and to confirm your agreement, I ask that you say aloud, “I agree.” This is a way of acknowledging your commitment to these terms. Even if you do not literally say it out loud, understanding and accepting the terms is what matters most. Thank you for agreeing to these terms—it is essential for the success of this course.

Finally, I want to remind you that I am available to help and connect with you throughout the course. You can reach me via Udemy Q&A, where I will always respond, though it may be more challenging to provide direct solutions due to the complexity of environment issues. You can also reach me by email or connect with me on LinkedIn. I welcome LinkedIn connections, and if you post your course projects and assignments there, tagging me allows me to provide feedback and amplify your work. Sharing your progress on LinkedIn can showcase your expertise to a wider audience, including potential future clients or employers.

As we wrap up day one, let’s revisit the curriculum. With the first day highlighted as complete, you have successfully deployed your first simple AI app. This marks 5% completion of your journey toward deploying generative and agentic AI into production. Congratulations on reaching this milestone! There is much more ahead, and we begin with day two tomorrow. I am excited to continue this journey with you and can’t wait to see the projects you will build in the coming days.

# **H) Day 2 - Building Full-Stack AI Apps: Frontend-Backend Architecture for LLMs**

Well, if you're still here, that means you haven't been completely put off by day one, which was quite a marathon day. And you're here back for day two of Genii and Agentic AI in production. So what do I have in store for you today? We're going to be talking about the front end and the back end, putting them together to make a full stack application. And I gotta tell you, we are hardly going to scrape the surface of what it takes to write a front end. I imagine some of you are actually front end engineers on this course, looking to get more well-rounded. And for you, the next few slides are going to be kind of easy. For some of you, you might be completely new to front end engineering. I'm just going to cover the basics to give you a framework, to give you the intuition for what it is that goes on when you build the front end side of a web application. I'm going to ask you to review the code, to look at what I'm doing, and get an LLM to explain it if you don't understand it. They're also amazing at generating front end code. Use this to give you the foundation of what's going on when you build a front end and a back end to work together.

Just to start with some definitions: obviously, when we say front end, we're referring to the code that runs in the user's browser—a combination of HTML for the structure of the page, CSS for the appearance of the page, and JavaScript, which is used, for example, for what happens when a button is clicked or for making animations move. It's the interactivity of the page. The back end, on the other hand, is the business logic running on the server. It includes database access, calling LLMs, potentially calling other APIs, storing your secrets, and the like. Your typical web application, of course, has a front end and a back end. The front end makes API calls to the back end by hitting a particular URL, which we call a web endpoint. It hits that URL, which calls the backend code. The backend generates some content and returns it to the front end, typically in the form of a JSON object, and the front end collects that JSON object and uses it to make some changes to the UI.

There is another way the back end is sometimes used, which is that it can be called to create an entire web page, serving up a whole web page to the front end. So the front end might call my home page, and when that URL is called, the server generates the entire home page front end code and passes that back to the browser. So that's a second way that server back end code is used, and we'll be doing both of them in our labs. Now, you may be wondering how Gradio fits into this. If you've taken my other courses, you'll know that I'm a huge fan of Gradio. I use it a lot to build quick UIs that look great, in my opinion. You might be wondering, "Where does the front end/back end of Gradio come in?" Well, here's the answer. Gradio is a back end framework, but confusingly, Gradio is able to generate front end code, and that's kind of kept behind the scenes for us. We write and describe a UI with Python, and Gradio generates the front end for us when it's serving up that user interface. That's why when you're using Gradio, it's a kind of front end/back end in one—because the back end code is able to generate the front end code. We won't be using Gradio in this course because we're doing stuff for reals; we're going to be building real front ends and back ends.

I just want to talk about the progression of different technologies that have happened over time when it comes to front end code. The front end landscape started off some time ago with vanilla HTML web pages, and still some people do this. There's something very satisfying about writing this way. This is where you just have basic HTML code to describe a web page, write your own CSS to do the styling, and have JavaScript. Typically, people use lightweight, low-level libraries like jQuery, which simplify some of the things you have to write in JavaScript. A lot of what you're doing when you write JavaScript at this level is manipulating something called the DOM, which stands for Document Object Model. This is the JavaScript model that represents the web page being rendered in the browser, so that you can do things like navigate around in the code to find a button and then change its color with JavaScript code. That model of what the web page looks like on the browser’s screen is known as the DOM.

Next came the JavaScript front end frameworks—an abstraction layer to make it quicker and more reusable to build sophisticated web pages. There’s a zoo of these frameworks, the most popular by far being React. There's also Vue, Angular, and Svelte, among others. They are all about building UIs from reusable components that you can plug and play together to construct quite sophisticated UIs quickly. Most of the time when you're working with a framework like React, you're building what's known as a single page application (SPA). This refers to the fact that, even though as a user it feels like you're clicking around lots of different web pages, the whole React application—the content and front end code—is loaded up once when you first hit the first URL. From that point onwards, when you're clicking around the application, you're typically making a series of API calls to the server, but it’s all running effectively on the same web page, even though it appears to redraw itself in different ways and feels like you're navigating around.

React and the other frameworks come in two flavors: a JavaScript variant, which is what it began with, and a more modern TypeScript variant, which is React using TypeScript, a strongly typed version of JavaScript. If you're not sure what that means, ask ChatGPT—it will explain it brilliantly. The final step in this progression is the application frameworks that came next and are the most recent part of this story, such as Next.js, which we will be using. React is super flexible and quite bare bones; it doesn’t come with a lot of features like form validation or routing between different sections of your app. The assumption is that if you're using React, you pick and choose which frameworks you want to add together. This is great for flexibility but means there are many different ways to build React apps. Next.js is a higher-level framework built on top of React that bundles together many useful tools so that you don't need to make lots of different decisions—you can just use Next.js and go. It has routing and data fetching built-in, supports server-side rendering, and comes with a bunch of tools built-in, making it very quick to get started.

This completes the narrative of the three tiers of technology that have formed modern front end development.

# **I) Day 2 - Building Full-Stack AI Apps with React, FastAPI, and NextJS**

Now, if you're thinking there's a lot of talking going on in this and you're wanting to get to action, never fear. We're about to get to action. Give me one more second. A couple more slides, particularly the front end. People are probably getting pretty bored at this point. But we'll get there. We'll get there.

Uh, react a few words about what React is. It is, of course, this kind of JavaScript front-end framework that is component-based. It's made of building blocks. Each block has markup, styles, and logic packaged together in such a way that you can assemble user interfaces by bringing together these different components. It's what's called declarative, which means the way that you write a piece of React is you just describe what your UI should look like given a particular state of the world, given a state of your information. This is how the UI should be represented.

The way React works behind the scenes is that every time any state changes, it’s recalling your code to figure out what you now think the UI should look like. It doesn't redraw the whole UI because that would look really clumsy on the screen, but it automatically looks at what's changed in the DOM before you change the state and afterwards. Then it only updates the parts of the UI that have changed. That's really ingenious. In the old days, you had to write tons and tons of logic when something changed to try and figure out what on the UI had to be updated. You don't need to do that anymore. You simply describe the whole screen, and the React framework takes care, every time something changes, of figuring out what needs to be updated on your UI.

React has two concepts that you'll see come through when we use it quite a lot: props and state. Props is short for properties, and this represents information about your user interface that gets passed down from higher-level components to smaller components and controls the way that they should present themselves. Those are called props, properties. Don't worry if it sounds abstract—it will hopefully come together when you see examples. State is exactly what it sounds like. That is representing the kind of information, the state, the status of the information that you're presenting to the user. That's something your components are responsible for managing, and React figures out how to redraw your screen as state changes.

JSX and TSX, for JavaScript and TypeScript respectively, are special types of documents that are a kind of hybrid between HTML and JavaScript/TypeScript. When you see them, you'll notice it's kind of curious—it’s like a mixture of the two. There's some HTML in there and then suddenly some code in there. It's a really convenient format. Before this format existed, you had to have lots of JavaScript or TypeScript code that forced in strings with different bits of markup at various points, which was very clumsy. JSX and TSX are just nice, elegant ways of doing it that make your life easy. You'll see we'll be using TypeScript (TSX) everywhere, and you'll get very comfortable with it once you've seen it a thousand times.

The world of React is rich and can't be overstated. There are so many React frameworks and components that you can include and then just throw onto your screen. Component libraries, which are suites of components, are especially useful. Material UI is perhaps the most famous, and Chakra is becoming increasingly popular. These libraries are full of components that work nicely together, allowing you to build a user interface very quickly.

To complete the picture, let me tell you about Next.js, the application framework built on top of React. It brings together a number of other frameworks so you can hit the ground running with React. Next.js is actually built by Vercel, the company behind the cloud AI deployment we did yesterday and are going to do again today. It’s a Silicon Valley-based, developer-centric company. Next.js is great because it brings so much functionality out of the box.

Next.js includes two different implementations of routing functionality, which controls what gets drawn when a user clicks different sections of your application. The first is the pages router, which you can recognize by a subdirectory called pages. This is the simpler, more trusted, and very common approach. The other is the app router, recognizable by a directory called app. It's the newer flavor, more powerful, and now recommended by Next.js. For this course, we'll mix and match. We'll start with the pages router because one of the frameworks we're using for authentication only supports it. Pages themselves can be rendered on the client side in the browser or increasingly on the server side, creating the final web page on the server before serving it to the client. For this course, we'll stick with the client-side approach as it's simpler and fits better with what we're doing.

Next.js also includes tooling for transpiling, which converts modern TypeScript into vanilla JavaScript, and bundling, which packages your code efficiently for the browser. You only need to focus on writing great TypeScript; Next.js handles everything else.

Most people taking this course are familiar with backend development. Three popular Python backend frameworks are Django, Flask, and FastAPI. Django is heavyweight and “batteries included,” with ORM, authentication, templating, and an admin UI. Flask is a micro-framework, super simple and quick to get started, but you have to add other frameworks as needed. FastAPI sits in between these two, modern, async, and optimized for writing servers that service API endpoints. It's incredibly popular and is what we’ll use throughout this course.

A final piece of admin before we get to the lab: the repo situation. How I’m handling code for this course is more involved than previous courses. Previously, there was one repo for the entire course. This time, there will be a different repo for every week of the course. This gives you experience setting up a repo for a project and building it from scratch. We'll also use GitHub Actions for deployment. For this week, we'll start with a main repo called production. The first step is to git clone that repo so you have a local copy. We'll then build another repo for today’s course, called SaaS (Software as a Service), which contains a folder called week one with instructions for each day.

The SaaS repo also has a guides folder with self-study guides covering topics like Docker, front end, and more. This will be useful for extra research. There's also a community contributions folder. You can submit contributions such as troubleshooting tips or a repo you’ve set up. You can create a markdown file with your name and description of what you’ve done, link your repo, and submit a PR. Instructions for this will be provided in the guides.

All right, that's enough of the admin stuff. It's now time to go to the lab and get coding. Roll up your sleeves, and I will see you in the course.

# **J) Day 2 - Building Your First Full-Stack AI SaaS with NextJS and FastAPI**

Oh, welcome to the lab for day two. I love the labs. The first thing I've done is bring up a web browser and go to github.com. This is where we've already been, but this is where we're going for this production repo, which is the repo for the whole course. We'll be making lots of specific ones, and you'll see a lot more than this because I haven't pushed everything to GitHub yet. If you're not sure about GitHub and git, there's a guide on that—please do read it. It's important to have that foundational knowledge.

Once you're here, go to the green Code button, click it, choose HTTPS, and copy this to the clipboard. This copies a link to the repo into your clipboard. Then, open up Cursor. You don't need to use Cursor for this course; you can use any IDE you like. Any VS Code clone will work—it’s going to look very similar, so VS Code itself, Cursor, Windsurf, or even PyCharm will work fine. I'm just in the same instant project we used last time, but you can be in any project in Cursor.

Open a terminal in Cursor by pressing Ctrl + Backtick, which toggles the terminal on and off. If you press Ctrl + Shift + Backtick, you get a second new terminal, and you can stack multiple terminals on the right-hand side. Right now, we're in a directory called instant, and I want to go up one to my projects directory. You probably have a similar projects directory, and if not, you might want to create one. Again, there’s a guide that talks you through command prompt basics. One thing to keep in mind is that your projects directory is best if it’s not part of a cloud directory like OneDrive (Windows) or iCloud (Mac). You don’t want to replicate your projects to the cloud unnecessarily because they’re already on GitHub.

Once in your projects directory, type git clone <production-repo-url> and press Enter. The first time, you might have to handle authentication. After this, you’ll have cloned the repo and can cd into it to see that it’s all there. You now own a local copy of the repo and can open it as a project. In Cursor, go to the File menu, choose New Window, then press Open Project. Navigate to your projects directory, find production, and press Open. This opens it as a new window.

On the left is the file explorer. If you don’t see it, open it from the View menu. Exit any AI chat panel for a clean view. Inside, there is a week-one directory. Open it, and you’ll see files for each day of the week. Click on day-two.md (or similar) to see the instructions. Initially, it appears in raw markdown, so right-click and select Open Preview to see the nicely formatted version. You might need to install a markdown extension if prompted, but often it’s built-in. Here are the instructions for day two. Enough chit-chat—let's get to it and build our SaaS AI application.

Today, we’re building a business idea generator— a simplistic app that generates a new business idea using an LLM. You can modify this to do something else if you like; the goal is to learn and experiment. We'll use a modern React frontend built with Next.js, the pages router (not app router), and TypeScript. The frontend will connect to a FastAPI Python backend, use streaming to render AI-generated content nicely, and be deployed to production.

The first step is opening a new terminal. We will create a new project using the command:

npx create-next-app@latest sass --typescript


Here, sass stands for Software as a Service, a commercial app for users to access via subscription. --typescript specifies we want TypeScript rather than JavaScript. During setup, you'll be asked some questions. Choose ESLint as the linter. When asked about Tailwind CSS, choose yes—it's a powerful styling framework. When asked about putting code inside a source directory, choose no; we don’t need it for now. For the app router question, choose no to use the pages router (required for this week’s authentication framework). When asked about Turbo Pack or customizing the input alias, choose no.

After the command runs, your Next.js app will be created inside your projects directory as sass. Make sure it’s not in OneDrive or iCloud; it should be directly on your computer. Once created, open it in Cursor the same way we did for the production repo: File → New Window → Open Project → navigate to projects/sass → Open. You now have a fresh Next.js TypeScript project ready to develop your SaaS application.

# **K) Day 2 - Building Your First FastAPI Backend for Production LLM Deployment**

And so now I’m going to go in cursor to “File → New Window,” and up it comes. Then I go to “Open Project,” navigate into my projects directory, and there is the folder called sass. I press open, and here is our new Sass project. Let me make this bigger for you so we can take a closer look at our pride and joy.

We’ve got a directory called “pages” because we’re using the Pages Router, a directory called “public,” another called “styles,” and then a bunch of different configuration files. This is going to be our new home for the rest of this week. I’m going to start by bringing up a terminal with the shortcut “Ctrl + backtick ( ` ),” if you remember that one. I also closed down an AI thing that was here — you can keep it open and ask it questions if you wish.

Now before we go on, we’ve got another project called “production,” which I have running in another window. That project has our recipe for what we’re going to do today. You can click between the two windows, but that might be a bit awkward. So I’m actually going to copy across all the markdown files that contain the instructions for what we’re going to do this week. You don’t need to do this; you can just refer back to the other window, or even use a File Explorer or Mac Finder and copy the folder manually if you wish.

I’m doing this only for convenience. I’ll create a new folder and call it “week1.” Inside it, I’ll run a simple command — this is a Mac command — but as I said, you can just do it via the user interface. I’ll go up one directory, then into “production/week1,” take all those files, and copy them into the new “week1” folder that I’ve just created. That’s done. Now when I open that folder, you’ll see that all the files are there.

I’m doing this just so we don’t have to flip between two different windows. You can do this however you prefer. I’ll now open the preview of “day2,” close this screen here for now, and we’re back in the workspace. We’re still in Step 1 — Creating your Next.js project.

Now that we’ve opened the project, we can see a little description of what we have here. Indeed, we’ve got the “pages” subdirectory just as described. Within it, we have “_app.tsx” — remember, these “.tsx” files combine TypeScript and HTML into a single file type. We’ve also got “_document.tsx,” “index.tsx,” and various other things. There’s also an “api” folder with a file called “hello.ts.”

But we’re going to be removing that, just as the guide says. Since we’ll be using a Python backend, not a Next.js (JavaScript) backend, this “api” folder is redundant. So right-click it and select “Delete.” It’ll ask, “Are you sure?” — choose “Yes,” and it’s gone. Great, we’ve cleaned that up.

Next, a quick introduction to Tailwind CSS. I didn’t cover this earlier, but Tailwind is a CSS framework. In the old days, we had to manually write a lot of styling code — and while you could get good at it, styling was always a bit of a dark art, as front-end developers know all too well. Tailwind gives you a pre-built set of styles you can apply using simple, descriptive class names. You’ll see examples like “bg-blue-500,” “text-center,” or “p-4,” and you’ll quickly get used to this syntax. It makes styling much easier — just mimic, copy, and paste the classes you like.

Alright, onwards to Step 2. The rest of this setup will be similar for all of Weeks 1 and 2 — we’ll mostly follow instructions, set things up, and paste in code. It might feel like everything is environment setup, and that’s true — because production deployment is all about setup. You’ll get used to this mode of working soon enough.

The first thing we want to do now is create a new folder called “api.” You might say, “But we just deleted an ‘api’ folder!” True — we deleted the one inside “pages.” Now, we’re creating a top-level folder. So right-click in the main project area, choose “New Folder,” and name it “api.” It should appear at the top level of the project structure, directly under “sass.”

Next, we’ll create another top-level file — not a folder — called “requirements.txt.” (Make sure to spell it exactly like that.) This is the file that lists all Python packages that need to be installed automatically using pip. You’ll notice we have three packages to install: “fastapi,” “uvicorn,” and “openai.” These go into the requirements.txt file — they’re the dependencies for our backend.

Now, let’s populate the “api” folder we just created. Inside it, create a new file named “index.py.” It must be named exactly “index.py” — if not, things will break later. This precision matters. Open that file and paste in the following FastAPI code:

“from fastapi import FastAPI
from openai import OpenAI

app = FastAPI()

@app.get('/api')
async def root():
client = OpenAI()
prompt = 'Come up with a new business idea for AI agents.'
response = client.chat.completions.create(
model='gpt-5-nano',
messages=[{'role': 'user', 'content': prompt}]
)
return response.choices[0].message.content”

So what is this doing? This is our FastAPI code. We start by creating an app instance using “app = FastAPI().” In FastAPI, we describe backend routes like this — when someone sends a request to our web address at “/api,” this Python function (“root”) gets called. Whatever this function returns becomes the HTTP response. We also specify that it’s a plain-text response type.

Inside the function, we instantiate the OpenAI client using “client = OpenAI().” Then we define a “prompt” — in this case, the message “Come up with a new business idea for AI agents.” This is what our backend will send to the OpenAI API.

Next, we call “client.chat.completions.create()” with the model “gpt-5-nano,” which is the ultra-cheap variant of GPT-5, passing in our prompt. We then return the output using “response.choices[0].message.content,” which extracts the model’s text reply.

That’s it — we’ve got our backend route “/api” defined in “index.py.” It makes a call to a large language model and returns its response.

If you don’t want to use OpenAI (for example, to avoid the $5 upfront credit), you can substitute any of the alternatives mentioned in the guides. Gemini currently has a free plan (at least as of this recording), and OpenRouter also offers many free models you can run. You’ll find detailed instructions in the setup guides for those.

So that completes our setup for now — a working backend route in FastAPI that sends a prompt to an AI model and returns its response. This is the only AI-related code we’ll write today — everything else from here will focus on deployment and configuration. But for now, enjoy this small piece of AI code, because it’s the heart of what our backend will do.

# **L) Day 2 - Deploying Full-Stack AI Apps with Next.js Frontend and FastAPI Backend**

Back in our instructions, we’re now on Step 3: Creating your first page.

Before we start coding, there’s a short explanation about the Pages Router. By default, components in a Next.js project can run both on the server and on the client. But since we’re not using a JavaScript server — our server is going to be Python FastAPI — we need to make sure the code for our pages only runs in the browser. To do that, we include the special directive "use client" at the very top of each page file. That tells Next.js that this code should be executed on the client side only.

Alright, the first thing we’re going to do is replace the default contents of our main page, which is the file "index.tsx". This file is what gets served when someone visits our website’s root URL. By default, it just says something like “Welcome to a new Next.js app.” So, open index.tsx, press Ctrl + A to select everything, delete it all, and paste in the new code from our instructions.

So, what does this code do? At the very top, it has "use client", since this page is going to run fully in the browser. It also imports "useEffect" from React, which allows us to run some code whenever React decides it’s needed — typically when the page is first loaded.

Inside useEffect, we’re calling the Next.js function "fetch". This lets the frontend make an API call to the backend. The URL it fetches from is "/api". The response that comes back — which will be the business idea generated by our FastAPI backend — is then stored in a React state variable called "idea".

So, in plain terms: when the page first loads, it sends a request to our Python backend at /api, gets a response back from GPT, and displays that as the “business idea.”

The rest of the code defines the layout of the web page. This is where you see the magic of TSX, where TypeScript and HTML blend together. After the logic, there’s a "return (...)" statement — and suddenly it’s all HTML-like code. We have a <h1> heading that says “Business Idea Generator”, and below it, we display the idea itself.

You’ll notice the HTML tags have Tailwind CSS classes, like "text-center", "mt-10", or "font-bold". Instead of writing long, custom CSS, we’re using Tailwind’s descriptive class names to style elements instantly.

When you open the page in a browser, at first it’ll show the word “Loading…” — because that’s what we’ve set as the default state before the API call completes. Then, when the backend sends back the generated idea, the page automatically updates and displays it. That’s React doing its reactive magic.

If the front-end logic feels a bit fast for you, don’t worry. This isn’t a front-end course — just focus on the idea that we now have a page written in TSX that talks to our backend API and shows dynamic results. You’ll get more comfortable with these files over time.

Now, heading back to the instructions, the next thing to do is update the "_app.tsx" file. So, open _app.tsx, select all its contents, delete them, and paste in the new version. This file basically imports our styles and renders the app — nothing too fancy here.

Next, go back again to the instructions and scroll down to the step for "_document.tsx". This is the global HTML structure of the entire site — it defines the overall document, the <html> and <body> tags, and metadata. So open _document.tsx, select everything, delete it, and paste in the new code.

You’ll see inside it something like "export default function Document()" returning an HTML-like block with <Html>, <Head>, and <Body> tags. It sets the title to “Business Idea Generator” and includes a description meta tag. This is the file that shapes the top-level layout of your app.

Okay, now we’re ready to configure and deploy our project.

We’re deploying again to Vercel, just like in Day 1. You might remember that previously we created a "vercel.json" file to tell Vercel how to handle the frontend and backend. The good news is — this time, we don’t need it. Because we’ve followed all of Vercel’s defaults (for example, naming our backend file "index.py" and having "requirements.txt" at the root), Vercel will automatically detect everything. It knows we have a FastAPI backend, a Next.js frontend, and the right dependencies. It’s all just going to work.

So, let’s link this project to Vercel and deploy it.

Open a new terminal window. Hopefully, you already installed the Vercel CLI in Day 1. If not, you’ll need to go back and do that. Assuming it’s installed, type the command "vercel link".

This command connects your local project to a project in Vercel’s cloud. The CLI will ask:

“Set up and link project sass?” — choose Yes.

“Which scope should contain your project?” — pick the default.

“Link to existing project?” — answer No, since we’re creating a new one.

“What’s your project’s name?” — type "sass".

“In which directory is your code located?” — just press Enter, since it’s right here.

And then — bam! It’s done. The project is now created in Vercel and linked to your local files.

Next, we need to add our OpenAI API key so that the backend can authenticate when calling GPT.

In the terminal, type "vercel env add OPENAI_API_KEY".

Be extremely careful with this — it must match the variable name used in your code exactly. If you accidentally type "OPEN_API_KEY" or "openai_key", it won’t work, and it’ll be hard to debug.

When prompted, paste your actual API key (the one from the OpenAI platform) and hit Enter. It’ll ask which environments to apply it to — select them all. You can do that by pressing A for “All,” then Enter.

Obviously, don’t show this key to anyone — treat it like a password.

Once that’s done, there’s just one command left: "vercel ."

That dot at the end tells Vercel to deploy the current directory as the project. Press Enter, and the magic begins.

Vercel now packages your app, recognizes it’s a Next.js frontend with a FastAPI backend (thanks to our "index.py" and "requirements.txt" files), installs all dependencies, and deploys everything to the cloud.

Vercel automatically sets up two environments: a preview environment for testing changes and a production environment for live deployment. Since this is our first deploy, it’ll go straight to production. Future deployments will go to preview first.

You’ll see logs showing that the build is running, and then — it’s deployed!

Now let’s open the live app.

In Cursor (or VS Code), you can Command + Click (on Mac) or Control + Click (on Windows) the link that appears after deployment to open it in your browser.

Drumroll, please… The app loads, and you’ll see your front end saying “Business Idea Generator”. At first, it displays “Loading…” — and a few seconds later, you’ll see a full business idea generated by GPT-5 Nano.

For example, one possible output might be:

“The Nexus Agent — an Agent-as-a-Service platform that lets small and medium-sized businesses deploy autonomous AI agent teams to run end-to-end business processes across their apps with governance, safety, and explainability.”

It’s quite a detailed idea — whether it’s a good one or not, I’ll let you decide!

But what matters is this: you’ve now got a fully deployed production app running in Vercel. The frontend is built with Next.js, the backend runs on FastAPI in Python, and the two are communicating perfectly.

It’s simple, but it’s also powerful — because this is your foundation. From here, you can keep expanding: add routes, new pages, smarter prompts, and real backend logic. And we’ve built and deployed it all by Day 2.

# **M) Day 2 - Adding Real-Time Streaming and Professional UI to Your LLM App**

But wait — there’s a bit more to finish off today. The instructions suggest running "vercel --prod", but technically it’s not required because we’ve already deployed to production. You can do it if you wish, and we’ll run it again later. For now, the focus is on adding real-time streaming and making the results display nicely in Markdown, so they look more elegant than plain text.

First, we need to install a few packages. One of the great things about React is the massive ecosystem of libraries. For showing Markdown in the front end, we can use some pre-built components. In the "sass" folder, run "npm install" with the required packages, and Node will install them all. Think of "npm install" as the frontend equivalent of Python’s "pip install" — it brings in all the dependencies we need.

Next, we update "index.tsx" to make the frontend juicier. Open "index.tsx", select all, delete, and paste in the new code. The main change is that this version handles streaming back information from the server. It also uses a component called "ReactMarkdown", which renders Markdown nicely instead of just showing raw text. This is a classic example of the kind of React component you can just drop in from the ecosystem.

If you check the code, you’ll notice that the backend streaming logic is now supported by the frontend: React listens for chunks from the backend and appends them in real time. The Markdown component takes care of rendering headings, bullet points, and formatted text elegantly.

We also need to ensure that Tailwind works properly with the Markdown content. Sometimes Tailwind overrides standard HTML styles, hiding default <h2> and <h3> formatting. To fix this, open "globals.css" inside "public/styles", scroll to the end, and paste in traditional HTML styles. Don’t replace what’s already there — just append these so Markdown renders correctly.

Next, update the backend "index.py" to stream results. Open "index.py", select all, and paste in the new version. Here, "client.completions" now has "stream=True", and the FastAPI response uses "StreamingResponse" to send the data back to the frontend in chunks. This ensures the frontend sees the content as it’s generated, rather than waiting for the entire response to finish.

Once that’s done, we can deploy again. In the terminal, run "vercel ." to deploy the current project. Since this is the second deployment, it will go to the preview environment rather than production. This way, the original production link remains untouched, and you can test the new features safely. Preview deployments are handy because you can experiment with streaming, styling, and Markdown without affecting the live site.

When the deployment finishes, Command + Click (Mac) or Control + Click (Windows) the preview link. The page loads and initially shows "Loading...". Then, as GPT-5 generates the business idea, it streams back, and you’ll see the content appear live in chunks.

To make the results more structured, update the prompt in "index.py" to encourage Markdown formatting. For example, change the prompt to something like: "Reply with a new business idea for AI agents formatted with headings, subheadings, and bullet points". This encourages the LLM to produce structured, attractive Markdown output.

Finally, polish the frontend further. Open "index.tsx" again, replace its contents with the new version from the instructions, save, and that’s it. The page now shows streaming Markdown results in a visually appealing layout with Tailwind styling. Even if you’re not an expert in front-end development, this approach gives you a professional-looking interface with minimal effort.

Once ready, deploy to production with "vercel --prod". The command pushes the updated app to the live environment. Open the production link, and now you’ll see the fully styled, streaming business idea generator. It displays a heading like "AI-powered innovation at your fingertips" and dynamically updates the business idea in real-time, formatted with headings, bullets, and sections. You might even see additional details like a team blueprint.

At this point, congratulations! You now have a full-stack application deployed to production: a Next.js frontend using Tailwind CSS and ReactMarkdown, a FastAPI backend streaming GPT-5 responses, and two environments on Vercel — preview and production.

Looking ahead: tomorrow we’ll add authentication, sign-in, and subscription so users can pay to access the business idea generator. On Day 4, we’ll expand the app into a healthcare SaaS, and on Day 5, we’ll redeploy to AWS to compare platforms.

So celebrate this milestone: you’re already 10% of the way through the course, with a solid foundation in production deployment, streaming back-end responses, Markdown rendering, and polished frontend presentation. This is just the beginning, and it’s going to get even juicier.

# **N) Day 3 - Adding User Authentication to Your Production AI Application**

I’m so glad you’ve decided to stick around for another day. Hopefully, I didn’t scare you off yesterday with our first — or rather, second — production deployment!

To recap, yesterday we built both a front end and a back end, combined them, and successfully deployed the application. Today, we’ll be focusing on authentication and subscription — two topics that might sound intimidating at first, but I promise, they’re going to be much easier than you might think.

This week is particularly focused on using frameworks that make deployment incredibly straightforward. For example, deploying to Vercel is almost effortless. But don’t be lulled into thinking it’s always this easy — in the next few weeks, we’ll be working with the major cloud platforms: AWS, Google Cloud Platform, and Azure. That’s going to be a completely different experience, so get ready for a whole new level of complexity.

For now, though, things will stay simple.

As a quick recap: we built a full-stack application — that is, an app with both a front end and a back end. The front end runs in the user’s browser and includes HTML, CSS, and JavaScript. The back end contains the business logic that runs on the server. The front end communicates with the back end through API calls — for example, sending a request to an endpoint on the server, which responds with data (usually in JSON format). In our case, we returned plain text, but typically this would be JSON, which the client then uses to update and re-render the page dynamically through React.

We used Next.js with React for our front end and FastAPI with Python for the back end. For styling, we used Tailwind CSS, which helps you write clean, efficient styles without having to deal with tons of custom CSS. We deployed our project on Vercel’s cloud platform, which provided us with two environments — a preview environment and a production environment.

Let’s also quickly revisit the repository setup. It’s a bit intricate, so stick with me. We started by cloning a repository called production, which contains all the instructions, documentation, and guides for this and next week’s work. Inside it, there’s a “week one” folder that outlines what we’ll be doing each day.

We then created a new repository from scratch called sass. I did this intentionally so that you’d get into the habit of creating new projects from the ground up. We could have simply added it as a folder inside the production repo, but that would’ve made things messier. So now you have two separate repos — production, which holds all the documentation and guides, and sass, which is where our actual application code lives.

I also showed a quick trick for copying the guides folder across from production to sass, so it’s easier to reference while working. The production repo also has a community contributions folder — and this is where I’d love to see your input! If you’ve discovered something interesting, built your own repo, or have some helpful notes or code snippets, create a Markdown file with your name, write up your insights, and submit a pull request. That way, others can benefit from your work. Take a look at the folder yourself — you might find some useful content shared by others as well.

In weeks three and four, we’ll move on to different repositories that I’ve already prepared. So, yes — there are going to be lots of repos! But I’ll make sure to keep things organized and easy to follow.

Now, for today’s session, we’re going to be using a service called Clerk — a simple yet powerful authentication platform that helps manage user sign-ups and logins with very little code. There are many authentication solutions available — for instance, AWS Cognito provides a robust, enterprise-grade authentication system — but we’ll use Clerk today because of its simplicity and effectiveness.

The goal is to help you understand the basic principles of authentication. Once you’ve seen how Clerk works, you’ll be able to quickly grasp other systems if you encounter them in your projects. If you’re starting a new project from scratch, I’d highly recommend Clerk for its ease of setup and use — and you’ll see exactly why in a moment.

So, let’s get started with the hands-on part — less chit-chat, more action. Let’s return to our lab environment and continue working on our Business Idea Generator project — but this time, let’s give it some user authentication.

Welcome back to Cursor, our coding environment. Make sure you’re in the sass project, not the production one. I’ve still got the “week one” folder here because I copied it across, but you can always refer back to the original in the production repo if needed. Open the day3.md file to follow along with today’s session — and don’t forget, there’s also a part two for Day 3 that we’ll get to later.

Today’s focus is on user authentication, which will allow users to sign in before using our Idea Generator. They’ll be able to sign in using their email or via social authentication (like Google or GitHub). Behind the scenes, this works by passing JWT tokens (JSON Web Tokens) to the backend to confirm that a valid, signed-in user is making the request.

JWTs are a fascinating topic with lots of depth — if you’re curious, I highly recommend looking them up (ChatGPT can explain them beautifully). But for our purposes, you can just think of them as the secret ingredient that allows platforms like Clerk to securely verify users.

Now, to set up Clerk, we’ll start by creating a Clerk account. Head over to Clerk’s website and click Sign Up. I’ll use an incognito tab for this demo since I’m already logged in. When you first visit the site, click Sign In, then choose Don’t have an account? Sign Up, and create your free account. You can use Google or GitHub to sign in. I used Google during my first setup. You’ll be asked a few quick questions (like whether you’re signing up individually or for work), and once done, you’ll land in the Clerk Dashboard.

This dashboard is where you’ll create and manage your applications. Click Create Application and name it SaaS. You’ll be able to customize which authentication options to allow — for example, email, Google, and GitHub sign-ins. Then click Create Application.

Since I’ve already done this, I won’t recreate mine, but once you do, you’ll see your new app listed in your dashboard.

Next, we’ll install Clerk’s SDK (Software Development Kit) into our Next.js project. Open a terminal and run:

npm install @clerk/nextjs

This is the JavaScript equivalent of pip install in Python. Once that’s done, we’ll also install another helpful package called fetch-event-source, which lets us stream results with authentication support:

npm install @microsoft/fetch-event-source

Now, we need to set up some environment variables. These include:

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY (the public key anyone can know)

CLERK_SECRET_KEY (your private key)

You can find these in your Clerk Dashboard under Configure → API Keys. Copy both keys — Clerk will hide the secret key for security, but you can copy it using the clipboard icon. While you’re there, also copy the JWT Template URL; we’ll need it shortly.

Next, go back to your project in Cursor and create a new file in your project root called .env.local. Paste the keys you just copied into that file.

Make sure .env.local is listed in your .gitignore file so these secrets aren’t pushed to your repository — but don’t worry, Next.js already includes that by default. You can verify this because the file will appear slightly grayed out in your editor, indicating that it’s being ignored by Git.

Once that’s done, your environment variables are ready. I’ll add my keys off-screen, and we’ll continue from there in just a moment.

# **O) Day 3 - Adding User Authentication to Production AI Apps with Clerk**

In this step, we began by updating our front-end application code. Specifically, we replaced the contents of the _app.tsx file inside the pages directory with new code that imports and wraps our entire application in a React component called ClerkProvider. This ClerkProvider component provides authentication context and shared functionality across all React components within the application. Essentially, it ensures that authentication and user-related operations are consistently available throughout the app. While this is a simplified explanation, the key idea is that ClerkProvider makes user authentication accessible to all components within our React app.

Next, we created a new page named product.tsx inside the pages directory. This page is a protected route, meaning it’s only accessible to authenticated (logged-in) users. The product.tsx file combines TypeScript and HTML in a React-compatible format. It includes the use client directive at the top, ensuring that the page runs client-side. This page contains the complete functionality for our Business Idea Generator, incorporating components for Markdown rendering, code streaming, and event handling. In essence, this is the main page that users will interact with once they’ve logged in to the platform.

After that, we modified the index.tsx file to serve as a new landing page with sign-in functionality. Previously, index.tsx contained the entire main content of the application, but we’ve now moved most of that to product.tsx. The updated index.tsx acts as the entry point for users who are not yet logged in. It includes authentication components such as SignInButton, SignedIn, and SignedOut. These components determine what content should be displayed depending on the user’s login state. If a user is signed in, the SignedIn component content will render; otherwise, the SignedOut content will appear. Thanks to Clerk, all of this logic is handled automatically without any custom backend logic. This drastically simplifies what used to be a very time-consuming process—something that could have taken weeks or even months to build manually, especially when implementing social login features.

With the front-end setup complete, the next step involved adding our JDBC URL to the .env.local file. This is an important configuration step where we retrieve the database connection string from the “Configure” → “API Keys” section and paste it into the .env.local file. It’s essential that the variable names and formatting exactly match the expected syntax, or the application will fail to connect properly later on.

Following this, we updated our backend dependencies by editing the requirements.txt file. We added a new package called fastapi-clerk-auth, which allows the FastAPI backend to verify that only authenticated users can access specific API routes. This integration ensures that our backend routes are secure and that only logged-in users can send or retrieve data.

Next, we modified the backend route in index.py. This file now imports authentication helpers from fastapi-clerk-auth, and when defining our API route, it checks for valid credentials before processing any request. This ensures that only authenticated users can access the backend endpoints. There’s also an example line in the code showing how to extract the user ID from the credentials—useful for cases where different users might have different permissions or subscription plans. Additionally, a small bug fix was implemented to improve how streamed responses are formatted, ensuring the output displays correctly.

After the backend configuration, we moved on to setting environment variables in Vercel (our hosting platform). We added three key-value pairs—the same ones defined in the .env.local file—using the vercel env add commands. Each variable must match exactly in both name and value to avoid deployment errors. Once these are configured for all environments (by pressing “A” to apply them to all), the deployment environment will have access to the same configurations as our local setup.

Finally, we ran the project locally using the command vercel dev. This command launches the frontend on localhost:3000, allowing us to test the application in development mode. Note that this setup only runs the JavaScript (frontend) part locally—the Python backend isn’t active in this mode. However, this still lets us verify that the frontend is correctly connected to Vercel and that Clerk authentication is functioning properly.

Once the app is running, you’ll see a clean, modern landing page titled “Generate Your Next Big Business Idea” with a sign-in button and “Get Started Free” option. When you’re logged out, this landing page appears; upon signing in through Clerk (using, for example, your Gmail account), the protected product page becomes accessible. You can experiment by signing in or out and observing how Clerk dynamically manages session states and displays the appropriate page content.

# **P) Day 3 - Adding Subscription Billing to Your Production AI SaaS Application**

Before deploying the application to production, we first returned to Vercel, our hosting platform, to finalize some important configuration settings. Inside the SaaS production project, Vercel provides a quick preview of our current production deployment. The instructor navigated to the Settings section and then to Deployment Protection. Since we’re already using Clerk for authentication and access control, we don’t want Vercel to add its own protection layer on top of that. Therefore, under Deployment Protection, the Vercel authentication feature was turned off, and the change was saved. This ensures that our app remains accessible on the internet, but still securely protected through Clerk’s authentication system.

Once that was configured, we proceeded to deploy the application to production by running the command
vercel --prod.
This command pushes the finalized version of our SaaS application live to the internet. Alternatively, if we wanted to deploy it first to a preview environment for testing, we could use vercel . (dot) to preview before going live. With the production deployment complete, we launched the live application to see it in action. Upon opening the deployed app, the landing page displayed the familiar message: “Generate Your New Business Idea.” From there, the instructor clicked Sign In, logged in using an existing Clerk account, and confirmed that everything worked perfectly.

Once signed in, the user could interact with the app by clicking Generate Business Idea. Behind the scenes, this triggered a call to the protected backend route—the same route we secured using FastAPI and Clerk authentication earlier. The front-end and back-end exchanged a verification handshake, ensuring that the request came from an authenticated user. We could even see the authentication trace being printed in the backend logs, confirming that the handshake was working correctly. Then, the AI-generated business idea began streaming back to the browser in real time, formatted neatly on the page. The instructor demonstrated how refreshing the page or clicking the button again generated a new business idea, proving that the system was fully functional.

At this point, the application had officially become a secure, full-stack SaaS product, deployed in production with integrated authentication. Although still simple in functionality, it represented a complete working model of a cloud-based SaaS system—something users could log into and interact with live on the internet.

With this, the instructor wrapped up Part 1 of the project, which focused on building the base application, implementing Clerk authentication, and securing both the front-end and back-end. Moving forward, we began Part 2, which introduces subscription management—a critical feature for monetizing the app. In this next phase, we would allow users to subscribe to our Business Idea Generator through paid plans.

To get started, the instructor opened the Week 1 → Day 3, Part 2 folder in Cursor. This section focuses on transforming our SaaS application by integrating Clerk Billing. The goal is to make the Business Idea Generator accessible only to users who have an active subscription. Clerk, in addition to handling user authentication, also provides an integrated billing platform. It can either use its own built-in payment gateway or connect seamlessly to Stripe, which is ideal for real-world payment processing.

The first step to enable billing was to go back to the Clerk Dashboard. On the overview screen for our SaaS app, we could now see a confirmation message that said, “Congratulations, your application has users!”—reflecting our previous logins. In the dashboard’s sidebar, the instructor navigated to Configure → Billing Settings and then to Subscription Plans. For first-time users, a Get Started button would appear, prompting them to enable billing. Clicking this button brings up two payment configuration options: the Clerk Payment Gateway (the simpler, built-in option that we’ll use for testing) and Stripe, which can be used for real transactions if you plan to launch a real paid product. For the purposes of this tutorial, no real money is processed; it’s all test-mode billing.

After enabling billing, the next step was to create subscription plans. Under the “Subscription Plans” section, the instructor demonstrated creating two plans: a Free Plan and a Premium Subscription Plan. To create one, you click Create Plan and then fill in details such as the Plan Name, Key, Description, and Base Fee. The plan key must not contain hyphens—underscores are acceptable. For example, the premium plan key was defined as premium_subscription, with a name of “Premium Subscription.” The monthly base fee was set to $100 per month, and an optional annual discount of $90 per month (for users committing to a yearly plan) was also enabled. The plan was set to be publicly available so that users could see and subscribe to it.

Finally, the instructor pointed out the Features section within each subscription plan. This is where developers can define which features are tied to each plan—allowing different tiers of functionality for free and premium users. In the backend, this can later be implemented by checking the user’s credentials and determining which subscription plan they’re on. That logic would let developers restrict or unlock parts of the app based on the subscription level.

Once everything was configured, we were instructed to take note of the Plan ID, as we would use it in the next step of development. With this setup complete, the instructor concluded the segment by noting that the subscription infrastructure was now ready, and in the upcoming lesson, we would integrate these billing plans directly into our application to enable real subscription-based access.

# **Q) Day 3 - Adding Authentication and Billing to Production AI Applications**

Now that the subscription plans were set up in Clerk, the next step was to update the application code to check subscription status before granting access to premium features. On the Products page (product.tsx), the instructor replaced the existing code with a new version that includes a Protect element. This component ensures that only users with the correct subscription plan—matching the plan ID set up in Clerk, e.g., premium_subscription—can access the idea generator. If the user does not have the required subscription, a fallback view is displayed, which includes a pricing table and a call to choose a subscription plan. The idea generator itself, the main UI for generating business ideas, is only rendered once the subscription check succeeds. Once the changes were saved, the landing page (index.tsx) was also updated to include subscription information and a pricing preview for users who are signed in.

With these updates in place, the instructor deployed the application to production and opened it to verify that everything worked. The landing page displayed the subscription details and pricing, although the hardcoded preview did not yet match the exact prices configured in Clerk (e.g., $100/month). Signing in with an existing account showed the manage account and billing information, confirming the user was already subscribed to the premium plan. Accessing premium features then successfully triggered the idea generator, confirming that the subscription check and protected route were working correctly.

Next, the instructor demonstrated signing in with a new account that had no subscription. This involved Apple authentication, two-factor verification, and using the “Hide My Email” feature to prevent account duplication. Upon signing in, the user was prompted to choose a plan. The Clerk billing system handled the test payment flow, allowing the user to subscribe to the monthly premium plan using a test card. Once the subscription was confirmed, the user could access the premium features and generate business ideas. This workflow confirmed that both the authentication and subscription systems were fully integrated and functioning as intended.

The instructor emphasized how remarkable this was compared to traditional development. Historically, implementing social login, subscription management, and Stripe integration would have taken several months and multiple developers. With Clerk, the entire flow—including authentication, subscription verification, and billing—was implemented in a matter of hours. Users can now manage subscriptions, authenticate with multiple providers, and access protected features seamlessly.

In conclusion, Day Three successfully covered both user authentication and subscription integration, taking the application from a simple, secure SaaS prototype to a fully production-ready platform with subscription-based access. The instructor encouraged learners to review the code, experiment with the front-end, and consider deploying their own apps. The next day would introduce business functionality, focusing on applying AI to the healthcare vertical. Learners were reminded to celebrate progress, noting they were already 15% of the way to production expertise, and to start thinking about extending the app further.

