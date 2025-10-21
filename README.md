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

**R) Day 4 - Building Your First Commercial AI App: From Prototype to Business**

**S) Day 4 - Building Healthcare AI Apps with FastAPI and Structured Prompts**

**T) Day 4 - Deploying Your Complete AI Healthcare App to Production on Vercel**

**U) Day 4 - Building a Production Healthcare AI SaaS with Streaming LLMs**

**V) Day 5 - AWS Setup and IAM for Production AI: Your First Cloud Deployment**

**W) Day 5 - Setting Up AWS Cost Monitoring for Production AI Deployments**

**X) Day 5 - Setting Up Secure IAM Users for Production AI Deployments on AWS**

**Y) Day 5 - Containerizing AI Apps with Docker for Cloud Deployment**

**Z) Day 5 - Migrating Your AI App from Vercel to AWS for Production Scale**

**AA) Day 5 - Containerizing Your AI App: Docker Images for Production Deployment**

**AB) Day 5 - Deploying Dockerized AI Apps to AWS with ECR and App Runner**

**AC) Day 5 - Deploying Your AI App Live on AWS App Runner with Auto-Scaling**

**AD) Day 5 - From Vercel to AWS: Deploying Production LLM Apps at Scale**

**II) Week 2**

**A) Day 1 - AWS Foundations for Production AI: From Console to Infrastructure**

**B) Day 1 - Cloud Deployment Architectures for Production AI Applications**

**C) Day 1 - AWS Cloud Components for Production AI: S3, Lambda, and Bedrock**

**D) Day 1 - Building Your Digital Twin: AWS Lambda + Bedrock Architecture Setup**

**E) Day 1 - Building Your AI Digital Twin: Production Setup with NextJS App Router**

**F) Day 1 - Building Your First Full-Stack AI App with FastAPI and React**

**G) Day 1 - Building Conversational Memory for Production AI Chat Applications**


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

# **R) Day 4 - Building Your First Commercial AI App: From Prototype to Business**

And welcome back. Welcome to day four of week one. The first thing I want to mention is a little detail that maybe I’ve already mentioned, but when I start with these intro and outro slides, the strip of color that you see here is a cue for what kind of day it’s going to be. This is a blue day, which means it’s a day about project work, about commercial projects, about applications of AI. And we’re going to use this to turn our app into a business app. It’s going to be a very simple business app, but the idea will be for you to take it as a springboard to build in more functionality and make it something juicier. It’s going to be applied to healthcare—that is the game of the day.

First of all, I do want to bring you back to that reminder of the agreement that you made with me—the agreement that hopefully some of you verbalized and, as such, it is a binding commitment—which is that you wouldn’t get frustrated with environment issues. You’re probably getting a flavor for how much of this course is going to be about setup. It’s not like we’re going to be doing as much coding. In fact, so far it’s been, except at the very beginning, mostly copy and paste, because much of what we’re doing with production deployments is going to be platform engineering—configuring stuff, setting it up—and things will go wrong.

On my current courses, I get hundreds of questions, sometimes like a hundred a day, on stuff like environment variables being wrong—at least that’s what it turns out to be. Or there was someone that had a lot of problems connecting to an API that sends emails, and that someone was getting really frustrated. It turned out it was due to some privacy limitations that his company had with a VPN, so that they couldn’t make a secure outbound connection. So each of these problems has come up with relatively little environment configuration in my other courses. This course is going to have a lot of it, so you do need to have a lot of petrol in the tank to put up with the grief you’re going to get setting up environments. Just remember that’s part of the fare.

Building expertise in production and deployments involves a lot of bashing your head against a wall with environment errors until you figure them out, and that is a skill that you get better and better at. I’m here to tell you that every time you spend several hours trying to debug something—which always ends up having some silly explanation at the end of it—it’s so frustrating when you find that, but you’ll be better prepped next time to debug. So that’s part of the skills.

All right, so I’m here to tell you that first of all, do keep an eye on the docs. I try and document everything very carefully, and you’ll find that the documentation for what to do will change from what I show you in the videos, because I’m going to be constantly updating it with the latest stuff. So please don’t be alarmed if the instructions don’t look identical to what I do in the course, because as people hit problems in different systems and different environments, I’ll try and add that to the course. Look out for extra troubleshooting tips that get added in.

Keep experimenting yourself when you hit a roadblock, keep trying and ask LMS, but always verify what they tell you. Don’t trust LMS off the bat—ask two different LMS or make sure it explains its reasoning to you. As I said before, they tend to go with the most obvious bandaid to a particular problem and not take a step back and think of root causes. And try your best not to get frustrated. That was the commitment that you made to me.

Also, I do want to mention again that as we hit rabbit holes, as you come up with things that you don’t know about, don’t let that get you confused—embrace it as an opportunity. I threw in there mention of JWT; you should go and Google that if you’re interested. Stripe—if you’re new to that—then find out more about what Stripe is and what it does and why it is so greatly loved. And server-side routing—I mentioned briefly at one point—that’s something you could look into. It’s a very modern, popular technique, and it’s worth learning more about it if it interests you.

There will be many more things like this where we are just going to scratch the surface of what you could find out about. There are so many different ways that I could explore things in more depth, and I’m sticking to the main line here, but you can explore others and experiment, add things in, and submit stuff—link to it in Community Contributions with your notes on what you’ve discovered.

Okay, with that, it’s time for us to build our healthcare app, shown here by our astronaut who we’ve been following, wearing a stethoscope. So our healthcare app is going to start by being something very simple, which you can then use to build up. But the idea is that we want to build an app to be used in doctors’ offices. Something that’s quite common is that doctors have a consultation with a patient and they take down some rough notes, and those rough notes need some actions taken as a result. Maybe some prescription has to be filed, and then an email has to be sent to the patient giving a summary of what was discovered from that appointment.

And that’s a whole ton of administrative work. So this is going to be a SaaS app to be used by doctors’ offices so that the doctor’s notes can be put into a field, and it will generate the to-dos and the email to go to the patient in a professional way that could then be copied and pasted by the practice into an email to the patient. That’s the story—that’s what we’re going to build. You can see it’s pretty simple; it’s quite a natural extension of what we’ve already built. It’s just got one call in there, but hopefully you can also see how that is something that could be the foundation of a much more sophisticated healthcare app, should you wish to go in that direction.

Okay, and with that, it’s time for us to go to the lab, go back to Casa, and get going with our first commercial project. See you there.

# **S) Day 4 - Building Healthcare AI Apps with FastAPI and Structured Prompts**

And here we are in the SaaS project. I open up the Week One guides. These will be in the production repo as well, and I’m going to open the preview on Day Four so we get to see what we’re doing here. We’re building a healthcare consultation assistant. As I told you, it’s going to take the doctor’s consultation notes as input, generate professional summaries, create actionable next steps, and draft patient-friendly emails.

All right, so let’s start then with step one. We’ve got some new front-end dependencies to install, and we use npm install for that. Let me take this first one here — I’ll copy that. I’m going to bring up a new terminal. Here it is. And now I’m going to paste that in. There it goes, and it installs. And now we’ll do the second one here, which is the associated types, and I paste that there. And I run, and that installs too. Okay. Now let’s hide the terminal.

It’s time for us to update the backend API. So basically it’s the same backend API, except now we’re going to have some more detailed prompting. So let me copy this and paste it in, and then we’ll talk it through. There it is. Okay. So over we go to the API. And this is something which is going to replace the index.py, which is right here. So I select all and I paste.

And let me quickly explain this to you. It’s very similar to before — we’re still using OpenAI. The main difference here is that we have a bigger system prompt. “You’re provided with notes written by a doctor from a patient’s visit. Your job is to summarize the visit for the doctor and provide an email reply with exactly three sections with the headings.” And here are the three sections.

Now, the people from, say, my Agentic course will know well that a nicer way of doing this would be to have it reply with structured outputs, and then take that JSON and return it to the front end. But I want to take things a step at a time. If you want to update this to use structured outputs and to respond with JSON, that would be a much better implementation, and I would encourage you to do so. But for now, we’re just going to have it respond in markdown with these headings.

And so then, otherwise, things are very similar. We’ve changed it from being a GET to being a POST endpoint, so this is now a POST to /api. Also, in addition to the creds that we had before, which are the credentials coming from Clerk, we have another argument here — visit, which is an object of type Visit. And Visit here is a Pydantic object. That means that it is a subclass of BaseModel — Pydantic BaseModel.

Just go to the top — show you. There we go. There it’s imported: from pydantic import BaseModel. And that means that this is one of these Pydantic classes that’s used to describe the schema of a Python object. Its purpose is to describe what a Python object is — which fields it should have. It’s similar to a dictionary, except you’re using real attributes that have a type.

So we’ve got, in this case, a patient_name, a date_of_visit, and notes as the three bits of information here that form this Visit object. And we’ve got that here as the first argument for this endpoint. And the magic of FastAPI is that when you do it this way, FastAPI just builds the right route and expects the right JSON object to be provided in this POST, and it will automatically populate this Pydantic object, Visit, with all of the right fields. So you don’t need to worry about how this JSON object comes in the request and how to pluck out the values and put them into a Python object — FastAPI handles all of that for you, and that’s why people love it.

Okay, so with that out, we can just use visit in our code. This user_prompt populates the information — the patient’s name, date of visit, and their notes — and that is what we will send to GPT-5-nano. The system_prompt that we wrote above the user_prompt, which has got all these details that were passed in in the Visit object, and then we stream back results exactly as we did before. Nothing else has changed.

Okay. And now we’re on to changing the front end. First of all, before we change the actual pages themselves, we’re going to update those two front-end files and documents to reflect some of the changes here. So start with app.tsx. Let’s go find app.tsx in pages. There it is. And replace here. And all we’ve done is added in this import.

We’re importing something called React DatePicker, which is something that we just npm installed — it’s going to give us a date picker, a calendar. And this is a great example of how easy it is to get off-the-shelf React components to add something like a date picker to your webpage. In the days before React, it would be a chore to have a date picker — there would be a lot of JavaScript involved in that. And now it’s just so easy.

All right, back here again. And now we’re going to go to the document.tsx, and we’re going to use that to change the page title and heading. Here’s document.tsx. Let’s paste. There we go — “AI-Powered Medical Consultation Summaries. Healthcare Consultation Assistant.”

Okay, and now back to the instructions. And now the meat of the front-end changes. We’re going to update the products with our new product. And I will take all of this. And now, there’s a fair bit more — front-end code can look quite unwieldy sometimes. There’s a lot to it, but much of this is boilerplate.

Go over to product.tsx and replace everything with our new product. Let’s just take a look at a few things, but this is an exercise for you to look through it. So there’s this idea of state, which are the variables which our front end depends on, that React will automatically refresh the relevant parts of the UI as state changes. And we’ve got a patient name, a visit date, and notes.

And then we’ve got stuff to do with the streaming — much as we had it before — and this is how we’re handling the streaming back. Then this is where we have these forms for the patient name, the date of visit, and the consultation notes. You can see how very easy to read these React components are. It’s a textarea — it’s called notes, it’s required, it’s got eight rows, and it’s got all of the information here.

I also want to show you the date picker. The date picker — this is the React component that we’ve taken off the shelf for picking dates, and you just say you want a date picker and you give it the information that you need.

Okay, and this is the main part of it. This is where it has the title, the heading, the pricing table — sorry, this is the fallback if we’re not signed in — and this is the form if we are. Okay. So that is the front-end code updated. We’re closing in. We’ve got one step to go.

# **T) Day 4 - Deploying Your Complete AI Healthcare App to Production on Vercel**

The last big change for the front end then is the landing page. So this is pages/index.tsx. Here we go. It’s mostly just the reframing of what this is about. So let’s take this — here it is — copy that. So we’re going to index.tsx, paste, and save. Let’s take a look at this. It’s got just better formatting. You can take a look through the Tailwind CSS classes. It’s got a nice heading. It’s got the usual stuff. You’ll see here that the “signed out” section is what you see if the user is signed out, and the “signed in” section is what you see if the user is signed in. This is where it links to the /product route, and it’s got some footer text at the end which says it’s HIPAA compliant, secure, and professional — which, of course, it is not HIPAA compliant. But this is, of course, a demo, so you’ll forgive me for this extra piece to it. I’m sure whatever you build will be.

Okay, so I think with this, let’s go back to the instructions and see what we’ve got left to do. Oh yes, we just have one tiny thing. We did include pydantic classes there, so we have to add pydantic to our requirements.txt. That’s not going to work otherwise. So back here — that would have been a gotcha if we’d forgotten to do that. Save that. Be sure — remember, if you see that white dot there, you have to save it. If you don’t save it, then everything will fail horribly. Hopefully, you have saved it, which means that all that’s left for us to do is vercel --prod.

Can it really be this easy? We’ll see. So we’ll do prod, we’ll let that run, and I will speak to you in a second.

Okay, so it’s time for us to try this out. Let’s go to production. Let’s see — here it goes, opening it up. And here’s our landing page. Nice, right? It’s very professional looking. Transform your consultation notes — professional summaries, action items, patient emails. Very clear, and MediNotes Pro is what it’s called. And here are those “HIPAA compliant” claims that you should take off if you’re going to take this anywhere. Then press Sign In.

I’m going to log in as myself. Here we go — this is already authenticated. Continue using Clerk’s user authentication. I can look at my profile up here, go to Manage Account, and I can see under Billing that I’ve got my payment method set and my subscription is a premium subscription — $1,080 a year, and a bargain at that price.

And in we go. Let’s go to App. Let’s get started. This is the professional-looking consultation notes application. The patient’s name — let’s add Donna. The date of visit — up comes this beautiful pop-up, a date picker. This would have been hard work in the old days, but now it’s just adding in a React component. We’ll pick today’s date.

“Ed complained of a headache. I told him to take two Tylenol and come back in two days if it hasn’t gone away.” There we go — that’s our very casual doctor’s notes. And now we press the Generate Summary button, which turns light blue. It’s now making a POST API request to that API route, which is our FastAPI server. It’s passing in a JSON of this form, and FastAPI is bringing that in as pydantic.

And before I can even finish this explainer, we get back the results — the summary for the doctor’s records: Editor: Donna. Chief Complaint: Headache. Assessment and plan documentation shows a headache without any explicit diagnosis or workup noted. Plan documented as analgesic management with acetaminophen, which is the proper name for Tylenol — Panadol for the Brits — two tablets now with instruction to return in two days if symptoms have not resolved. So, super professional medical terminology and next steps for the doctor.

We’ve got information here. Here’s the draft of the email to go back to me:

“Hi Ed, thank you for coming today about your headache. Here’s the plan. We discussed medication. Please take two Tylenol (acetaminophen) now, following directions on the package. If the headache does not improve in about two days, please contact the clinic or come back for a follow-up.”

So anyway, with the details at the end, you can see it’s polished. It’s worked. It’s a nice healthcare app. We did what we intended, and it was so very easy. I hope you enjoyed this. I hope you have fun with it. And of course, remember — the main to-do for you is to consider this just your canvas on which you can build.

It doesn’t need to just give this summary and an email — it could do all sorts of things. For people who want to really experiment with it, you could also, if you’ve taken my LLM Engineering course and you know about things like taking audio input, make this multimodal — so that it could listen in to the doctor’s visit or take a recording from it and then build the notes or the summary.

For people that have done my course, you could have it so that it emails this to the practice, perhaps using SendGrid or Resend — it could email it automatically so that that email can be forwarded directly to the patient. All of those ideas would be cool, and you could have them be features that are only exposed in Clerk for people that are on a paid subscription tier.

So I hope you enjoy that, and I will see you back for the wrap-up.

# **U) Day 4 - Building a Production Healthcare AI SaaS with Streaming LLMs**

Well, that's not bad for four days’ work. We've got quite a lot done. We started by building a front end using React, built with the Next.js application framework. We used the TypeScript flavor of it rather than the vanilla JavaScript, and we used the Pages Router rather than the App Router. We're rendering on the client side, not on the server side. For styling, we used Tailwind CSS, and it was great — so easy to work with.

We also built a backend using FastAPI. Most recently, we used a Pydantic object as the argument to a FastAPI route, and that way we were able to make it so that when the client posts a JSON object, it automatically gets packaged into the right kind of object on the server side. It’s very easy to define APIs using FastAPI. We then deployed using Vercel, the AI cloud deployment platform that is also responsible for creating the Next.js framework. We've deployed on Vercel — first briefly to dev when we did vercel dev, where we just had a sort of front-end-only app. We also deployed to preview by doing vercel ., and then to production by doing vercel prod. That’s deployed on the internet, available to anyone over SSL. If you saw that, it was a proper secure website, and we did all of that with just a couple of commands.

We used Clerk to authenticate users and to have different subscription plans, and we built a little healthcare app that could easily be extended into quite a powerful assistant for a medical office. That’s very much my ask for you — you should take this as a springboard. Add in functionality and try to make this into something you really feel could be monetized, something that a medical office might actually pay for. Then, for sure, you can use your Clerk functionality, promote it out there, and see if you can make some revenue from this. That’s the idea — showing you how easy it is to build an actual SaaS app that you could then charge for.

And maybe I should mention, by the by, that at the same time as doing this, we also did actually call an LLM — there was some AI involved here. We called an LLM and streamed back results. There was AI behind the scenes. But the point I want to make is that the AI is a bit of a side note here. All of the learning — everything that you've learned this week about quickly deploying an app that you could monetize on the internet — has really been core platform engineering and DevOps-type work: configuration, deployment, and understanding all the nuts and bolts of having an app with a front end and a back end connected together. The LLM call on our server could have been anything — it could have been reading a flat file; it’s just the same. So while we are looking at AI-related concerns like the OpenAI API key and streaming back results, much of what we're learning is generally applicable to building apps. We're just doing it through the AI lens. I hope that makes sense.

Okay, so that concludes Day Four of the healthcare SaaS app and brings us to Day Five. You may have noticed that Day Four has been somewhat shorter than an hour, whereas these sessions are often an hour long. I do need to prepare you that tomorrow — deploying to AWS — is going to be a different kind of deal. There’s going to be a lot of sweat tomorrow, so be ready for that. Make sure you get plenty of sleep and that you’re in a very patient mood, because using AWS for the first time involves a lot of gritting of teeth, so be prepared for that.

The main bulk of this course is about deploying apps to major cloud providers, where they are built for massive scale in a production way. What we’ve done so far this week has been the rapid deployment to a platform called a PaaS platform — a Platform as a Service type of platform — where it’s incredibly quick and easy to get things done. I wanted to equip you so that you could start building SaaS apps and charging subscriptions for them, making money already. This ticks the boxes for the entrepreneur in you who wants to do this fast. But most of this course is going to be the heavy-lifting part — deploying apps that can scale in a big way, like apps running on AWS. That is what we’ll be turning to tomorrow.

As we go through this, we’ll be taking the same app and deploying it into AWS. It will give you an opportunity to compare what it’s like to deploy quickly to a platform like Vercel, where we can get things up there fast, versus AWS, where we have so much flexibility, security, and monitoring — it’s industrial grade. So prepare yourself for industrial grade; prepare yourself for tomorrow. But for now, take a moment to revel in the success of being 20% complete with the course. Congratulations — and I will see you tomorrow.

# **V) Day 5 - AWS Setup and IAM for Production AI: Your First Cloud Deployment**

So with any luck, you are now mentally prepared for day five. It's a big day. It's a day that requires, as I say, some grit. But I happen to find using AWS and deploying to these major cloud providers to be very satisfying as well. It's a big deal and it's exciting to be deploying on something that can take such massive scale and be close to the kind of bare metal of a cloud deployment. So it can be enjoyable. And, as I've warned you a million times, it can also be a bit frustrating. So here we are. We're coming to the conclusion of the first week of the SaaS Gen AI product. We're now going to go to production on AWS.

I do want to make the point that today is going to be about a preview of AWS. Next week is going to be the full AWS week, when we will really go deep on many components. We're not going to cover every component today, but many of the core components of AWS. Think of it more as a teaser. Today is a teaser of what's to come. You don’t need to pick up everything—you just need to get a flavor for it.

One of the things that one gets very used to with AWS is what's known as IAM—Identity and Access Management. It's something that's quite grueling with AWS in particular, more so than other providers like GCP (Google Cloud Platform) and Azure from Microsoft. AWS, Amazon Web Services, has a very granular, very powerful system for managing who can access what on the AWS platform. It's quite a headache the first time you get to use it, but it is one of the core strengths of AWS. So, it's a mixed blessing. Generally speaking, I think it is a net positive, but it's important to understand it.

IAM is very granular, and while it’s tiresome when you first use it, there is a good reason behind it. It's a great and important commercial skill to pick up. One of the reasons we look at AWS is to give you the ability to build software that scales in a big way and also to prepare you for industry, so that you have the kind of skill set you might expect to see in a job description. Being slick with AWS permissions is a big skill.

Here’s how it works. We start by setting up a new AWS account, assuming you don’t already have one, and you get a root user. The root user is the all-powerful user that can do anything, and as a result, the root user should, in practice, do almost nothing. You want to almost never log in as the all-powerful root user. The only two things that we ever use the root user for are assigning permissions (so that we can set up other accounts with more limited permissions) and budgeting, to ensure we are aware of spending and have controls around it.

Next, we create an IAM user, which is a user with more restricted permissions. In an ideal production setting, you’d create many IAM users with different roles. You might have different users for different environments or projects, each with access to specific resources. For this course, we won’t be that finicky. We'll create one user called AI Engineer, which will be our workhorse for the rest of the course. This user will have permissions to do all the things we need during the course. However, you’ll also be equipped to give more fine-grained permissions yourself for production or commercial projects.

Now, we move straight into some lab work. We’ll set up an AWS account and some IAM configurations. We'll start by signing up for a new AWS account, if you don’t already have one. Go to AWS Amazon.com, click to create an AWS account, enter your email, choose a password, and select a personal account type. You will need to enter payment information—AWS requires a credit card—but we’ll discuss managing costs in a moment. Choose basic support (free). Once this is done, you will have an AWS root account, which has all the powers in the world but is dangerous if used carelessly.

We'll then sign in to AWS with the root user. Because we’ve set up multi-factor authentication (MFA), you’ll be prompted for a code from your authenticator app. Once signed in, you’ll see your account ID, which is a 12-digit number uniquely identifying your AWS instance. Keep this number handy. Next, go to security credentials to set up MFA for the root account. This ensures the account is very secure and only accessible by you. While here, you’ll notice Amazon Resource Names (ARNs)—unique identifiers for AWS objects—you’ll see these repeatedly over the course of your work with AWS.

With MFA set up, sign out and sign back in to ensure everything works correctly. By now, you have an AWS root account that is secure, IAM concepts in place, and a preview understanding of how AWS allows for granular permission management. In the upcoming days, we’ll explore AWS in depth, covering Docker, AWS fundamentals, App Runner, and budget protection, giving you the professional cloud deployment skills necessary for production-level SaaS AI products.

# **W) Day 5 - Setting Up AWS Cost Monitoring for Production AI Deployments**

I want to say a few words about API costs in AWS before we go and set up some alerts. I'm conscious that I have already talked about this before, so this is just a refresher. API costs are your responsibility—you need to be aware of, monitor, and understand them at every step of our journey together. AWS offers a number of promotions for new sign-ups, depending on your region, student status, or other eligibility factors. One common offer is three months of free credits. However, some AWS activities still incur costs. For example, registering your own domain name requires a payment to a domain registrar, depending on the domain you choose.

For this first week’s project, the estimated cost is between $1 and $5. If you leave it running for the entire month, that’s the potential cost, but if you run it just for a couple of days and then shut it down, the cost should be minimal. It’s incumbent on you to monitor this. API costs should always be your choice throughout the course. While platforms like Vercel can be hobbyist-friendly, AWS is industrial-strength and used by major corporations. Understanding how to manage and monitor costs is part of the professional skill set expected by many employers, making this an important aspect of your learning.

We’re now going to set up alerts, which will allow us to monitor spending and understand what’s going on. AWS and other platforms provide granular alerting functionality, but there is no hard cap. That is, there is no built-in way to automatically shut down services once a certain spend threshold is reached. Their rationale is that AWS serves enterprise clients, and automatically cutting off services due to a billing issue could disrupt major operations like Netflix, which would be unacceptable. While it might seem strange that there’s no opt-in cap feature, it’s likely technically complex to implement. Nonetheless, you must understand this limitation, set up alerts, and regularly monitor your costs. Unlike OpenAI, where a $5 upfront cap limits risk, AWS theoretically allows unlimited liability if you inadvertently create massive infrastructure. Therefore, keeping track of costs is serious business and entirely your responsibility.

Now, let’s return to the AWS console. When you log in at AWS Amazon.com as your root user, you can see your account ID at the top. This identifies the account you are logged in as. Next, use the search box in the top-left corner to navigate AWS services—it’s your go-to tool and you’ll use it repeatedly. Type in “billing” and select “Billing and Cost Management.” This page shows your costs up to the current moment. You might notice high costs in some of my accounts because I experimented with Amazon OpenSearch Service, which was expensive, but your spending should be much lower. Regardless, check this page regularly to monitor your own costs.

On the left-hand menu, scroll down to “Budgets” under “Budgets and Planning.” This is where we will create alerts. Initially, you won’t see any budgets. Click the yellow “Create Budget” button. Start by selecting a user template and creating a zero-spend budget. This means you’ll be notified as soon as any spending above $0.01 occurs. Name it “Zero Spend” and enter your email address carefully, as this is your safety net. Press “Create Budget” and it will be set up.

Next, create another budget using the “Monthly Cost Budget” template. Name it “Monthly Check” and set the amount you are comfortable spending this month—$5, $1, or any amount you prefer. Enter your email address. AWS will notify you at three points: when actual spending reaches 85% of your budget, when it reaches 100%, and if the forecast predicts you will exceed your budget. Press “Create Budget” to finalize this alert. You can create additional budgets if needed, but having the zero-spend check is particularly useful to ensure notifications are working. Until you receive these alerts and verify them, make sure to regularly revisit the Billing and Cost Management section to stay on top of your spending.

# **X) Day 5 - Setting Up Secure IAM Users for Production AI Deployments on AWS**

This next part is extremely important and is all about IAM—Identity and Access Management. We will be using the root user we just set up, which for me is called Ed, to create a new user called AI Engineer. This user will have limited permissions and will be the identity we use throughout the course over the next few weeks.

On the AWS console, you’ll see the console home on the right after logging in, and on the left, you can follow along with the Day Five guide from the production repository. We’re on step four: creating the IAM user for our daily work. You should never use your root account for daily tasks, as it has permissions to do anything, which is risky. Instead, we create a more limited user. Currently, I’m logged in as the root user (named Ed) and will create a new user.

Start by using the search box in the console to find the IAM section. On the IAM dashboard, go to “Users” in the side navigation. You’ll notice I’ve already created a couple of users; you won’t have any yet. Press the orange “Create User” button and name it AI Engineer (or AI Engineer 2 if you already have one). Select “Access to console” and ensure it’s an IAM user. Choose “Custom Password” and enter a strong password. Uncheck “User must create a new password” since you are setting it now. Then press “Next” and “Create User.” I’ll cancel here since I’ve already created it.

Rather than adding permissions directly to the AI Engineer user, which has limitations, we create a user group. User groups allow you to manage permissions for multiple users, even though we only have one right now. Go to “User Groups” and create a group called Broad AI Engineer Access. I already have one, so I’d add a “2,” but you should stick with the original name. Add the AI Engineer user to this group.

Next, we attach permission policies to the user group. These policies define what AI Engineer is allowed to do. Add the following four policies:

AWS App Runner Full Access

Amazon EC2 Container Registry Full Access

CloudWatch Logs Full Access

IAM User Change Password

You type the name in the search bar, check the box, and don’t press the yellow button yet. Once all four policies are selected, press “Create User Group.” I’ll cancel here since I’ve already done this. You can view your user group, see the associated users, and check the permissions tab to verify that these four policies are assigned. As the course progresses, you might add more policies, but these four are sufficient for now.

It’s worth noting that granting full access for each of these services may be more than strictly necessary. AWS allows very fine-grained control over permissions, but for this course, assigning full access to specific services is sufficient. You can refine permissions further if needed for production environments.

Now that the user has been set up, with a username, password, and permissions, we can log into AWS as the IAM user instead of the root. First, sign out from the root user. Then, on the AWS landing page, press “Sign In to Console” and choose “IAM User Sign In.” Enter your 12-digit AWS account ID (the one you saved earlier), your IAM username, and password, then press “Sign In.” You are now logged in as your IAM user.

As an IAM user, you will notice access-denied messages in areas like cost and usage, because only the root user has access to manage budgets and view overall spending. You can see your IAM username and account ID at the top of the console.

Another key point is the AWS region, displayed in the top-right. Different regions are essentially different installations of the cloud, with their own services. Your default region may differ from mine (US East 1). It’s important to spell the region correctly (e.g., us-east-1) to avoid errors, as typos can cause obscure issues.

With this, you now have a functioning IAM user, with controlled permissions, logged in to AWS. You are ready to begin using AWS safely without relying on the root account for day-to-day tasks. Congratulations—you’ve successfully set up and logged in as your IAM user!

# **Y) Day 5 - Containerizing AI Apps with Docker for Cloud Deployment**

You’ve already mastered IAM quickly, and now it’s time to introduce something new: Docker. Many of you may already be familiar with Docker, but for some, this will be new. I won’t go deep into all the details, just enough to get the basic intuition. Docker allows you to run a computer within your computer—a box within a box.

Previously, we had virtual machines, which emulated an entire operating system and isolated processes on your computer. These were heavy and resource-intensive. Docker achieves a similar outcome but is much more lightweight, sharing the same operating system instead of replicating it. Essentially, Docker provides an isolated environment that is portable and reproducible. Once you build a Docker container, it can run identically on many different machines.

There are three key concepts in Docker: Dockerfile, image, and container.

Dockerfile: A simple text file with instructions for installing and configuring your container. It acts as a recipe, defining step-by-step how to build the environment.

Image: A snapshot or blueprint of a complete environment, created from a Dockerfile. Docker images can be built on top of existing images, layering changes incrementally.

Container: A live instance of a Docker image. You can create multiple containers from the same image. Containers can be started, stopped, and managed independently.

To summarize: Dockerfile → Image → Container. A Dockerfile creates an image, and images can spawn many containers.

Next, we’ll look at three AWS services that you’ll use this week:

AWS App Runner: The easiest way to deploy a Docker container to the cloud. You can test your container locally and then push it to AWS, where it runs as is.

Amazon ECR (Elastic Container Registry): A storage location for Docker images, ready to be deployed.

CloudWatch: A logging and monitoring service to track activity and logs across your AWS services. It is especially useful for observing agent behavior in a centralized place.

You’ve also already seen IAM and cost & billing management, making a total of five AWS services introduced so far.

Our next task is to take the healthcare app, package it into a Docker container, test it locally, and deploy it to AWS—all in one day.

The first step is installing Docker Desktop. This allows you to package your application into a container, like a shipping container for software. Go to Docker.com, download the correct version for your OS (Mac or Windows), run the installer, and follow prompts. Windows users will also install WSL2, a small Linux subsystem, since Docker requires a shared OS. After installation, start Docker Desktop and, if necessary, restart your computer.

To verify installation, open a terminal and run:

docker --version

This checks that Docker is installed. Next, test if it’s running with:

docker run hello-world

If successful, you’ll see a “Hello from Docker” message. This confirms that Docker pulled an image from Docker Hub, created a new container, and ran it. This output demonstrates the concepts of images and containers in action.

There’s a lot more to Docker beyond this introduction, but for now, this is sufficient to start packaging applications, testing them locally, and deploying them to AWS. For deeper exploration, you can refer to Docker’s official documentation or ask your preferred AI assistant for guidance.

# **Z) Day 5 - Migrating Your AI App from Vercel to AWS for Production Scale**

On Day Five, Part Three, we focus on getting our SaaS application ready to deploy to AWS. If you like your current Vassal application, it’s a good idea to take a backup of your SaaS folder and save it somewhere else—perhaps call it SaaS_Vassal. This precaution is important because we haven’t pushed the project to GitHub, so it’s just a local directory. Making a copy ensures you have a safe version to revert to as we prepare the application for deployment, which may overwrite existing files. At this point, your project should include the following folders: pages, api, styles, and public.

The first step is to convert the frontend into a static website. Previously, the frontend was rendered dynamically on demand. Now, we want to generate a static export so that the frontend consists purely of pre-built HTML, JavaScript, and stylesheets generated from the Next.js app. To do this, open the next.config.js file and add the necessary configuration to output a static site. This allows your frontend to be served as static files, which is essential for deployment to AWS. Once this configuration is added and saved, the frontend is ready for the next step.

Next, we need to update the frontend API calls. Previously, the frontend posted requests to /api. Now, because everything will run on the same server, we need to modify these calls to /api/consultation. To implement this, open pages/product.tsx (or wherever the fetch call occurs), locate the line that calls /api, and update it to /api/consultation. This ensures that frontend requests correctly target the new backend endpoint. Save the changes after updating the fetch call.

We now move on to creating a new backend file. The old index.py file will no longer be used, although you can keep it for reference. Create a new file called server.py in the api folder. This new backend file contains several key updates. First, it sets up a FastAPI app as before. It also includes CORS middleware, which ensures that only the correct frontend can call the backend, preventing unauthorized sites from making requests to your API. While CORS can be a deep topic, for now, we can use this as-is to prevent frontend errors. The AI-related routes remain unchanged, and the /api/consultation route is updated to reflect the new endpoint.

In addition, a new health check route is added at /health, which returns a JSON object: {"status": "healthy"}. This is important because AWS will use this endpoint to verify that the service is running correctly. Another significant update is that the backend can now serve the static frontend site. When someone accesses the root URL (/), the server will return index.html from the static export of the frontend. This allows a single backend to handle API requests, health checks, and serve the complete frontend, consolidating everything into one deployable service.

The next step is to create a .env file for secrets required during deployment. Start by copying the existing .env file from your project, which should already include the following keys: NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY, CLERK_SECRET_KEY, CLERK_API_URL, and OPENAI_API_KEY. For AWS deployment, you now need to add two additional keys: AWS_DEFAULT_REGION and AWS_ACCOUNT_ID. The default AWS region should be the one closest to you. Common choices include eu-west-1 (Ireland) for Europe, ap-south-1 (Mumbai) for Asia Pacific, and us-west-1 or us-west-2 for the US West coast. When you first log in to AWS, the console typically defaults to the nearest region, but you can verify it or choose a preferred one using the AWS regions page. The AWS_ACCOUNT_ID is the 12-digit number visible in the AWS console under your user details. Both of these values should be added to the .env file along with your other secrets.

Once this .env file is properly configured, the application is fully prepared for deployment. The backend can serve both API requests and the frontend static site, includes a health check for AWS, and the frontend API calls are updated to match the new routes. With this setup complete, you are ready to move on to the next stage: packaging the application into a Docker container and deploying it to AWS.

# **AA) Day 5 - Containerizing Your AI App: Docker Images for Production Deployment**

Now comes the exciting part: creating our own Docker image, starting with the Dockerfile. I already have a Dockerfile prepared, so the first step is to copy this text and create a new file called Dockerfile in the project root. Paste the contents into this file. The Dockerfile is essentially a set of instructions describing how to build a Docker image. For those who have used Docker before, this will feel familiar, but for first-timers, it’s an introduction to the workflow. The Dockerfile we’re using actually creates two Docker images—one temporary and one final.

The process begins with the temporary image. Using the FROM command, we start with a Node 22 Docker image pulled from Docker Hub. Several commands are then run, including setting environment variables and running npm run build. This command generates a static version of the frontend from our Next.js app, producing a set of HTML, JavaScript, and stylesheet files.

Next, we create the main Docker image using a slim Python 3.12 image as a base. The image is adapted to our project by first installing all Python dependencies from requirements.txt using pip. Then, the backend file api/server.py is copied into the image. Additionally, the static frontend built from the temporary image is copied into the new image. A health check is included to regularly hit the /health endpoint, and the server is configured to run on port 8000. Finally, the Dockerfile specifies that the server should be started using Uvicorn with the host and port settings, completing the Dockerfile definition.

After saving the Dockerfile, a best practice is to create a .dockerignore file. This file functions similarly to .gitignore by excluding unnecessary files from the Docker image build. Once created and saved, the .dockerignore file ensures that only relevant files are included in the image.

The next step is to build the Docker image. Scripts are provided for Mac/Linux and Windows to load environment variables from the .env file into the terminal. Once the environment variables are set, the docker build command is run. This command reads the Dockerfile and builds the Docker image according to its instructions. Depending on your system, this may take a few minutes the first time, as Docker executes each step: installing Python packages, building the frontend, and copying files. Subsequent builds will be much faster due to Docker caching previous steps. During the build, you may see warnings regarding environment variables. These warnings, related to public publishable keys, can be safely ignored.

At this point, we have successfully built a Docker image that packages both the backend and frontend of our application. As part of the process, a temporary container was also created and run to assist in building the final image. The build process may take 2–3 minutes initially, but rerunning it will be almost instant. Congratulations—you now have a Docker image that encapsulates your application.

The final step is to run a Docker container from this image. Using the provided docker run command for Mac or Windows, we launch the container. This container starts the server using the image we just built and performs a health check to ensure it is running correctly. Once started, the frontend becomes accessible locally, displaying the user interface. The container recognizes previous login sessions, confirming that both the backend and frontend are functioning as expected inside the Docker container. This marks the successful creation and execution of your first Docker container.

# **AB) Day 5 - Deploying Dockerized AI Apps to AWS with ECR and App Runner**

All right. Now, Control + C out of this Docker process. It's time to deploy to AWS App Runner. First of all, we need to set up our Docker container in the Elastic Container Registry (ECR). A Docker image, which is the blueprint for containers, needs to go into the Elastic Container Registry. So first things first, we need to go back to the AWS console. Let's do that right away. Here we are. Go to the AWS console and sign in. Make sure that you're signed in as the AI Engineer user and not some other user. Then go to the Elastic Container Registry. I just typed ECR in the search bar, and it came up for us right here.

Ignore the fact that I already have some things in here, including what we've got right now, because I may have done this before. We are now going to upload your container to the Elastic Container Registry. First, make sure you have the correct region selected — whatever region is closest to you. You can see different regions like the US East and West Coast, Mumbai, Singapore, Canada, and Europe. EU West 1 is very popular, and there is also SA East 1. Make sure this region matches what you have in your .env file. Then press Create repository. We are going to call this exactly consultation-app. It has to be exactly that because we will use it later. Everything else can be left as default. Press Create. I won’t press it because I already have one created. Once you’ve done this, you’re ready to continue to the next instructions.

Next, we need to configure the AWS CLI, which is the command-line interface for interacting with AWS from a terminal. First, go back to the AWS console and navigate to the Security Credentials section to set up access. Sign in as the AI Engineer IAM user, click on your account name, and select Security Credentials. Scroll down to the Access Keys section and press Create Access Key. Select Command Line Interface. AWS recommends other options, but we have every reason to use CLI for Docker. Tick the box to acknowledge the recommendations, give it a description like Docker push access, and press Create access key. You’ll be able to download a CSV with your credentials. Take note of both the Access Key ID and the Secret Access Key. After that, click Done.

Now it’s time to set up the AWS CLI. On Mac, you can install it using brew install aws-cli. For Windows, follow the instructions provided on the AWS link. Once installed, type aws configure. You might need to open a new terminal if you just installed the CLI. It will prompt you for your access key and secret access key. Paste both of them from the CSV you downloaded. For the default region, enter the region you selected earlier, and leave the output format as none. With that, the AWS CLI is set up, and you can now access AWS from your terminal. Congratulations!

Next, we will push our Docker image to the consultation-app repository. Make sure your environment variables are loaded. On Mac, run the commands to load them again, and follow the Windows version if you're on Windows. The first step is to authenticate Docker to ECR. This uses your environment variables to log in. Once successful, it should say Login succeeded. Now, build the Docker image. You may wonder why we’re building it again. This is particularly important for Mac users with Apple Silicon (M1/M2 chips). The previously built Docker image is specific to Apple Silicon and may not work on AWS. So, we need to build it specifically for a Linux backend. The build process will create the front-end export in Next.js, generating optimized production files — raw HTML, JavaScript, and CSS — ready to be served. Once the build completes, we tag the Docker image as consultation-app:latest and then push it to ECR. After the push, it will be ready for deployment.

Now it’s time to launch App Runner and deploy our service. We have the Docker image tested locally, and it’s now uploaded to the Elastic Container Registry. Go to the AWS console, search for App Runner, and click Create Service. Choose Container Registry, then Amazon ECR, and browse to select consultation-app:latest. For deployment settings, select Manual, and choose Create new service role. Click Next. The service name will be Consultation App Service. I’m calling mine Consultation App Service 2 because I already have a service running. For compute resources, select a small configuration: a quarter CPU and half a gigabyte of memory — lightweight but sufficient. Next, add the required environment variables: CLERK_SECRET_KEY, CLERK_URL, and OPENAI_API_KEY. Copy these from your .env file and add them as plain text variables. With that, our App Runner service is configured and ready to launch.

# **AC) Day 5 - Deploying Your AI App Live on AWS App Runner with Auto-Scaling**

Okay, so my secrets have now been saved. They’re just up there, off the top of the console. This is very important: where it says Port, you need to change it to 8000, because that is the port the app is listening on. Next is Auto Scaling. You need to create a new Auto Scaling Configuration (ASC). Give it a name — I’m going to call mine basic. Set how many requests can run concurrently at any one time — let’s say no more than ten. Set the minimum number of instances to one, and the maximum to one as well, so we will not have more than one running. This is where you could scale up if you were building a platform requiring high scalability. Once done, add this scaling configuration.

Next, add Health Check information. I’ve already filled mine in, but you would need to select a protocol — choose HTTP — and give it a path, which in our case should be /health. Set a timeout of five seconds and an interval of 20 seconds. This means it will wait up to five seconds before deciding the service isn’t healthy, and it will perform the health check every 20 seconds. If five checks fail in a row, the service is considered unhealthy. If a couple of checks succeed, it is considered healthy. These health checks help ensure that your service is running correctly.

Once that is configured, press Next. You get a chance to review everything one more time, including your secrets. I won’t show that here, but make sure everything looks correct. Confirm that the CPU is a quarter and the memory allocation is half a gigabyte, and make sure you’re comfortable with all the details. Once you’re ready, press the button to deploy your container to App Runner. This process will take a few minutes to run. Once you press it, you should see a screen similar to mine, though your service name will likely be Consultation App Service instead of Consultation App Service 2, because I already have a service running.

As it deploys, you’ll notice AWS App Runner is taking the Docker image we built and tested locally, which we uploaded to Elastic Container Registry. It’s now creating a live App Runner service using that Docker image. On the App Runner screen, you’ll see an ARN (Amazon Resource Name) — every AWS resource has one. The ARN includes the service type (App Runner), the region, the account ID, and other relevant details. The Source section points to the container image in Elastic Container Registry, which is being used for this App Runner instance.

Once the deployment finishes, your service will be running live on AWS. It will provide a domain with HTTPS access. This is the moment of truth — you can click on the domain to access the app on the internet. This confirms that the Docker container is deployed live on AWS using App Runner. You can sign in with your user ID. Once signed in, you can press Open Consultation Assistant, and the service will be fully functional.

The app client is now calling the server running in AWS App Runner. The server, in turn, calls OpenAI, and the response is returned. In this demonstration, it generates a doctor’s summary, next steps for the doctor, and even drafts an email to the patient. Everything is fully whirring in the cloud, demonstrating a complete, authenticated, deployed application. It’s running in a Docker container on AWS, with App Runner handling scaling, health checks, and deployment. Congratulations — this is a live AWS deployment!

# **AD) Day 5 - From Vercel to AWS: Deploying Production LLM Apps at Scale**

Well, I imagine some of you are feeling a bit like a deer caught in headlights with everything that just happened. Don’t worry — go with it. This is about absorbing more information as we go. There is a lot to AWS, and I imagine you’ve seen the enormous contrast. It was so easy to deploy to Vercel and get something running; it almost felt too good to be true. Experiencing that was really cool. Then AWS feels like almost the opposite experience. Setting up a user ID, managing permissions, user policies, attaching policies, and handling user groups — it can feel overwhelming. There’s so much terminology: ECR, App Runner, CloudWatch, and more. Don’t let it become too much. We didn’t even look at CloudWatch yet, but we will. You could click around to see some of the logging available in CloudWatch, which is useful.

Here’s a quick recap of what we did. We built a front end using React with the Next.js application framework. We used TypeScript rather than JavaScript, the pages router rather than the app router, and styled everything using Tailwind CSS. For the backend, we used FastAPI. Clark handled user authentication and subscription plans. We packaged everything into a Docker container using an approach where the front end is compiled into a static front end and served by the backend, all in one Docker container. We tested this locally, running both front end and back end together successfully.

After that, we took the Docker image and pushed it to the Elastic Container Registry (ECR). From there, we deployed it to AWS App Runner. App Runner is AWS’s simple approach for deploying containers to the cloud — one of the easiest ways to go live on AWS. And we did it! Congratulations. It’s worth noting that an LLM was involved in the application — we called OpenAI and streamed results back. So, although much of this week felt like configuration in the AWS console, with permissions and clicking around, there was a fully functional AI backend at the end of it.

If this feels like a lot, go back and review it. Explore the AWS console. A good practice is to log in as your root user and check costs in the Billing and Cost Management section. At this point, there should be no material costs, but it’s good practice to verify this.

For your assignment, go back and enhance this app. Add more functionality, and deploy it to Vercel — which is very quick and easy. Then, take a deep breath and deploy it to AWS. Now that you’ve handled all the configuration, IAM setup, and permissions, the final steps of building the Docker container, pushing it to ECR, and deploying with App Runner are straightforward once you’ve done them a couple of times. Be sure to document your results in a repository and share them in community contributions so everyone can see your work and the different approaches you took to build this app.

Wouldn’t it be amazing if you turned this into a proper SaaS product? Reach out to a few healthcare contacts or doctors’ offices and pitch your automated assistant to help make their practice more efficient. That would be really cool.

And with that, we conclude a massive day five. I warned you after day four that day five would be intense. Your brain might be fried, but you’ve learned an incredible amount. This concludes week one. We built a SaaS product, deployed it to production, and experienced both the ease of Vercel and the complexity of AWS. We got it live, scalable, and robust — an industrial-strength deployment on AWS. You should be proud of your progress. You’re now 25% of the way to becoming an expert in production deployment.

Next week, in week two, we’ll dive even deeper into AWS. You’ve dipped your toe into the AWS waters; next week, we’ll take the big plunge. Be ready for it. I’m really excited, and I’ll see you in week two.

# **II) Week 2**

# **A) Day 1 - AWS Foundations for Production AI: From Console to Infrastructure**

Well, do you have your sleeves rolled up? I hope you have your sleeves rolled up. I’m wearing a polo shirt, so my sleeves are naturally rolled up, but I hope you’ve got your sleeves firmly rolled up. We’ve got a huge week ahead—absolutely gigantic. I’ve got so much to show you, and there’s no time to waste. Let’s get straight into it. This week is all about AWS, and I can tell you it’s going to be a bit gruelling, but overall it’s going to be extremely fun. We have a lot to build, and by the end of the week, you’re going to be like a pro at AWS. I wouldn’t say you’re necessarily an expert yet—we’ll wait until the end of the full four weeks before we reach that point—but you’re going to be a pro, you’re going to know this stuff, and it’s going to be great.

What you see here is a preview of everything I have in store for you this week, including building a product using Bedrock, Terraform, GitHub Actions, and so much more. But first, we need to look back at what happened last week and the new skills that you’ve acquired as a result. We built a front-end app—it was a React app using the Next.js application framework, specifically the TypeScript variant. We used the pages router, though this week we’re going to use the app router, and we used Tailwind for styling.

We also built a backend app using the fabulous FastAPI. We used Clerk for user authentication and for building subscription plans that could be hooked up to Stripe. We are not going to be using that this week, but it might make a comeback in the future. While building this, we packaged the app into a Docker container. For those new to Docker, we covered some basics and tested it locally, and it worked—the front end and back end were running in one container. Then, we deployed that container to the cloud using AWS App Runner. After how easy it was to deploy with Clerk, going through all of these steps was a bit of a sweat—but this is core AWS learning.

At the same time, we called an LLM and streamed back results. While it may have felt like 80% of what we were doing was core platform engineering work, there was an AI angle too. I gave you an assignment to beef up the app with more functionality and capabilities—something that could actually be commercially useful in a medical practice. Hopefully, you did that. Maybe you shared a link to it, did a PR for community contributions, or posted about it on LinkedIn. If you tagged me, I would have checked it out and amplified your success.

Before doing anything else, we took a moment to go back into AWS as the root user and check our costs, ensuring there were no surprises. Signing in as root, we went to Billing and Cost Management. Ideally, you should have spent very little or nothing at this point, thanks to the free introductory plan. I personally spent $105, which was mostly due to preparing for this course and exploring cost-efficient ways to use AWS services. After checking costs, the next step was to ensure that the various services we built were no longer running.

We started by checking AWS App Runner, which we used for deployment last time. Some of my services were still running—ignore any unrelated apps. For the consultation services, we deleted them by selecting the service, going to Actions, and pressing Delete, confirming the deletion. Of course, if you want to keep a service running because it’s valuable, you can, but generally, it’s best to delete unused services to keep things clean. Next, we checked ECR (Elastic Container Registry) for any Docker images that might incur minimal costs. Again, selecting and deleting these ensures a clean AWS environment. Later this week, we’ll explore a way to see all resources in your AWS account to confirm exactly what you’re paying for.

Now, let’s take a moment to be self-congratulatory. We’re 25% of the way through the course. Think about the skills you’ve picked up so far. As an entrepreneur, you can now deploy an AI web app using Vercel with authentication and subscriptions. You know how to build your own app and deploy it, front end and back end included—a big milestone. For enterprise learners, you now have foundational AWS knowledge, understanding root and IAM users, permissions, containers using AWS App Runner, and ECR. You’ve also become familiar with the AWS console, navigating accounts, IDs, and cost numbers.

This week, we have an enormous amount to cover. We’ll be building and deploying an AI app on AWS, working with Lambda, Bedrock, S3, API Gateway, CloudFront, Route 53, and more. You’ll be setting up resources both through the AWS console and using AWS commands. This process can be laborious, but it’s crucial to understand the AWS building blocks before using automated tools like Terraform. Terraform allows us to define infrastructure as code, making deployment easier and repeatable. AWS also has its proprietary version called CDK, but we’ll focus on Terraform because it’s widely used across industries and works across AWS, GCP, and Azure. Everything covered can be adapted to CDK if preferred, but Terraform is highly recommended.

We’ll also use GitHub Actions for CI/CD (continuous integration and deployment), which will make deploying apps much smoother. This knowledge is core expertise for enterprise roles and startup environments alike. For entrepreneurs, Vercel may seem sufficient for early-stage deployment, and it might be—especially for initial product launches. But learning AWS and understanding scalable cloud deployments is essential. Vercel abstracts a lot of this for you, but knowing the underlying frameworks positions you for future growth. Eventually, as your app scales, you may outgrow Vercel and need to deploy properly using AWS, GCP, or Azure. Understanding cloud architecture, deployment pros and cons, and when to scale is vital. Entrepreneurs and enterprise learners alike will find this knowledge equally valuable, whether actively deploying or simply observing.

# **B) Day 1 - Cloud Deployment Architectures for Production AI Applications**

And now, perhaps for the single most important topic of the entire course—cloud deployment architecture—I’m going to be talking for a bit. There’s going to be some theory today and some lab work, with a bigger lab scheduled for tomorrow. There are a number of different ways you can deploy software to the cloud, and it can be ambiguous and confusing. People often use terms like PaaS in different situations to mean different things. I’ll explain the most common and typical usage, but be aware that some people may use these terms differently, so you might need to ask pointed questions to fully understand what someone means.

First and foremost, the simplest way to deploy to the cloud, and the way it all began, is what some people call a traditional cloud server, also sometimes known as IaaS—Infrastructure as a Service. In this model, you simply rent a computer in the cloud. You have access to a server, and while you’re renting it, it’s yours to manage. You have to set up everything yourself: choose the operating system, install patches, set up software, configure it, and run your programs. Back in the day, this was how all cloud deployments were done. You’d get a bunch of compute servers, set them up, install a database on one, an app server on another, and all these servers would run remotely in the cloud, on AWS or another provider. That’s where cloud deployment began.

Next up is Platform as a Service, or PaaS. Here, you write the code for your application—your business logic and functionality—and everything else is handled by a platform that takes care of putting your app online. This model was popularized by Heroku, which was one of the first to bring this approach to the mainstream. Today, it’s very common, and you’re most familiar with it through Vercel. Last time, we wrote a bit of code and a Vercel JSON file, and the platform handled the rest, publishing our app online with a URL. Compared with the traditional approach, this was pretty magical.

Another model you’ve had experience with is Container as a Service, sometimes called CaaS. In this approach, you package your app into a Docker image—a process called containerization—and then the service handles deployment. We did this with AWS App Runner. While some people use CaaS and PaaS interchangeably in different contexts, this is the most common understanding.

Next is container orchestration, which is a more advanced, professional approach. Sometimes people confuse CaaS with container orchestration, but container orchestration typically refers to managing many containers that need to interact with each other. You need to manage messaging between containers, scaling, monitoring, restarting, and coordinating the entire system. This usually involves using a tool like Kubernetes, which is extremely popular for running large-scale containerized applications in the cloud. This is the most advanced approach and is used primarily in large-scale companies. We won’t cover Kubernetes in this course, though it can be used even at smaller startups, including my own.

Last but certainly not least is serverless architecture, or serverless functions, sometimes called Function as a Service (FaaS). This is currently very popular and involves a granular approach where you write individual functions—such as an API route or a specific FastAPI endpoint—that are uploaded to a platform and executed on demand. When a request comes in, a server is spun up to run that function and then shut down afterward. This can happen in parallel, scaling dynamically based on demand. You pay only for the CPU used while the function runs, making it highly flexible in terms of pricing and scalability. Serverless architecture is particularly attractive for companies that want to start small and grow fast. In this course, we’ll focus heavily on serverless functions along with containers as a service.

To summarize, these are the five main cloud deployment archetypes you’re likely to encounter: traditional cloud servers, PaaS, CaaS, container orchestration, and serverless architecture. To layer this with AWS components, the typical services are as follows: for traditional cloud servers, it’s EC2; for PaaS, AWS offers Beanstalk (though you also know Vercel, which isn’t an AWS product); for CaaS, we used AWS App Runner; for container orchestration, AWS provides ECS and EKS—the Kubernetes version; and for serverless functions, the hot AWS product is Lambda. You don’t need to memorize these yet—we’ll cover them in more detail later—but by the end of the course, these names will become second nature.

(i) Traditional Cloud Servers (IaaS – EC2)

a) You rent a virtual server in the cloud.

b) Responsible for installing OS, software, patches, and configuring everything.

c) Full control over the server.

(ii) Platform as a Service (PaaS – Beanstalk / Vercel)

a) You write your application code; the platform handles deployment, scaling, and infrastructure.

b) Simplifies going live without managing servers manually.

(iii) Container as a Service (CaaS – App Runner)

a) Package your app into a container (Docker image).

b) The service deploys and runs the container on demand.

(iv) Container Orchestration (ECS / EKS)

a) Manages multiple containers that interact with each other.

b) Handles scaling, monitoring, restarting, and coordination of containers.

c) Typically used for large-scale applications.

(v) Serverless Functions (Lambda)

a) You write individual functions that run on demand.

b) Automatically scales with requests; you pay only for the execution time.

c) No servers to manage—highly flexible and cost-efficient.

# **C) Day 1 - AWS Cloud Components for Production AI: S3, Lambda, and Bedrock**

# **D) Day 1 - Building Your Digital Twin: AWS Lambda + Bedrock Architecture Setup**

# **E) Day 1 - Building Your AI Digital Twin: Production Setup with NextJS App Router**

# **F) Day 1 - Building Your First Full-Stack AI App with FastAPI and React**

# **G) Day 1 - Building Conversational Memory for Production AI Chat Applications**
