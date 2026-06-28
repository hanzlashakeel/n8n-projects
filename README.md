# My N8n AI Projects

I'm Hanzla Shakeel, a CS student at UET Lahore from Narowal. I got interested in AI automation and started learning n8n a few weeks ago. These are the projects I've built so far.

---

## Zaiqa — Restaurant Chatbot

I built this for a demo restaurant called "Taste of Pakistan". The idea was simple — instead of a human answering the same questions over and over, an AI does it 24/7.

What it can do:
- Tell customers what's on the menu and the prices
- Help with table reservations
- Answer in Urdu or English depending on who's asking
- Remember what was said earlier in the conversation

Stack: n8n, Groq, Llama 3.3

---

## ShopBot — Online Store Assistant

Built this for a demo clothing store. Covers products for men, women, kids, and elderly. The bot can actually take orders, apply discount codes, and handle complaints.

What it can do:
- Show products with prices across 4 categories
- Take orders and generate a confirmation ID
- Apply discount codes automatically
- Handle returns and complaints
- Reply in English, Urdu, or Roman Urdu

Stack: n8n, Groq, Llama 3.3

---

## What I use
n8n, Groq API, Python, Llama 3.3

---

## Let's connect
hanzlashakeel49@gmail.com  
linkedin.com/in/hanzla-shakeel-08a7b4393
----

## ARIA — Personal Assistant Bot

Honestly, I built this one out of frustration. Every time I needed something different, I had to open a different website or app. So I thought — why not build one thing that handles everything?

ARIA is not just a chatbot. It actually thinks through your problem, remembers what you said earlier, and gives you a proper answer — not a generic one.

---

### What you can ask ARIA:

**Everyday Productivity:**
- Make me a to-do list for today with priorities
- Help me plan my week — I have exams on Friday
- Build me a study schedule for 3 subjects
- Track my daily habits
- Help me set a SMART goal

**Money & Finance:**
- Convert 100 dollars to PKR right now
- Help me make a monthly budget on Rs. 30,000
- Calculate my loan installment for Rs. 500,000
- How much should I save each month to reach Rs. 1,000,000?
- Explain the 50/30/20 budgeting rule

**Writing & Language:**
- Write a professional email to my professor
- Review my CV and suggest improvements
- Write a cover letter for a software internship
- Translate this paragraph to Urdu
- Fix the grammar in this email

**Education & Learning:**
- Explain recursion to me like I'm 10
- Help me debug this Python code
- What topics should I focus on for my OOP exam?
- Summarize this concept in simple words
- Suggest a roadmap to learn web development

**Health & Fitness:**
- Calculate my BMI — I'm 70kg and 5'9
- Make me a diet plan to lose 5kg in 2 months
- Give me a 30-minute home workout with no equipment
- How do I manage stress during exams?
- I'm not sleeping well — what should I do?

**Business & Career:**
- Give me 5 online business ideas for Pakistan
- How do I start freelancing on Fiverr with no experience?
- Prepare me for a software engineer interview
- How do I negotiate salary?
- Review my LinkedIn headline

**Tech & Programming:**
- Help me with this Python error
- Explain what an API is in simple words
- What's the difference between SQL and NoSQL?
- How do I build a simple web scraper?
- Suggest free resources to learn Machine Learning

**Just for Fun:**
- Tell me a joke — make it actually funny
- Give me a motivational quote for today
- Write me an Urdu ghazal about life
- Tell me a fun fact I probably don't know
- Give me a brain teaser

---

### How ARIA handles real-time info:

For live data like weather, currency rates, and breaking news — ARIA doesn't guess. It tells you exactly which website to check:

- Weather → weather.com / accuweather.com
- Dollar rate → xe.com / pakexchangerates.com  
- News → geo.tv / dawn.com / bbc.com/urdu
- Gold rates → goldpricepakistan.com

---

**Built with:** n8n · Groq API · Llama 3.3-70b · Wikipedia Tool · Simple Memory

---

## Auto Email Responder — Webhook + AI + Gmail

I used to spend 20-30 minutes every day just replying to emails. Same questions, different people. So I automated it.

Now when someone fills out a contact form, they get a professional personalized reply in seconds. No human needed.

---

### How it actually works:

1. Someone fills a contact form — name, email, subject, message
2. Webhook receives the data the moment they hit submit
3. AI reads their message and understands what they need
4. AI writes a personalized reply — not a template, an actual thoughtful response
5. Gmail sends it automatically from my email

---

### What the AI understands:

**Project inquiries** — asks for details, mentions relevant skills, sounds excited
**Job/internship offers** — professional, enthusiastic, confirms availability
**General questions** — answers directly, offers further help
**Spam** — politely declines without wasting time

---

### Why this is useful for businesses:

Most small businesses lose clients because they reply too late. This system replies in under 30 seconds, 24 hours a day, 7 days a week — even when you're asleep.

---

### What I learned building this:

- Connecting Gmail to n8n using Google OAuth
- Setting up Webhooks for real-time triggers
- Passing dynamic data between nodes
- Making AI context-aware using form data

---

**Built with:** n8n · Groq API · Llama 3.3-70b · Gmail API · Google OAuth · Webhook

---

### Update — Lead Capture System Added

Originally this workflow just replied to emails. But then I realized — what happens to all those inquiries? They just disappear into your inbox. So I added Google Sheets to fix that.

Now every single lead is captured automatically. The moment someone submits the form, three things happen at the same time:
- Their details are saved to Google Sheets permanently
- AI reads their message and writes a personalized reply
- Gmail sends the reply within seconds

**What gets saved in Google Sheets:**

| Field | Example |
|-------|---------|
| Name | Ahmed Ali |
| Email | ahmed@gmail.com |
| Subject | Project Inquiry |
| Message | I need an AI chatbot for my business |
| Date | 2026-06-28 07:20 |

**Why this matters for businesses:**

Before this, leads would get lost in emails. Now the business owner can open Google Sheets any time and see every person who ever reached out — their name, what they wanted, and when they contacted. No CRM software needed. No manual data entry. Just automatic.

**What I learned adding this:**

- Enabling Google Drive + Sheets APIs in Google Cloud Console
- OAuth credential reuse across multiple Google services
- Mapping dynamic webhook data to spreadsheet columns
- Building multi-step workflows where each node passes data to the next

**Full updated stack:** n8n · Groq API · Llama 3.3-70b · Gmail API · Google Sheets API · Google Drive API · Google OAuth · Webhook

---

## WhatsApp AI Bot — Hanzla Bot

Most businesses lose customers because they reply too late on WhatsApp. I built HanzBot to fix that — an AI that replies instantly, 24/7, like a real person.

This was the hardest project so far. WhatsApp doesn't just let you plug anything in. You need a Meta Developer account, a verified business portfolio, OAuth tokens, webhook configuration, and approved phone numbers. Took time to figure out but got it working.

---

### How it works:

1. Customer sends a WhatsApp message
2. Webhook catches it the moment it arrives
3. AI reads the message — understands the language, tone, and intent
4. AI writes a personalized reply — short, conversational, WhatsApp style
5. Reply lands in customer's WhatsApp in seconds

No human needed. No delays. No missed messages.

---

### What makes HanzBot different:

Most WhatsApp bots reply with fixed templates — boring, robotic, and unhelpful. HanzBot reads the actual message and responds to exactly what was said. Every reply is generated fresh by the AI.

If someone writes in Urdu, it replies in Urdu. If someone writes in Roman Urdu, it matches that too. If someone is angry, it stays calm and empathetic. If someone asks a question, it actually answers it.

---

### What HanzBot handles:

**Customer Support:**
- Product and service inquiries
- Order status questions
- Complaint handling with empathy
- Escalation to human when needed

**Information:**
- General knowledge questions
- Business hours, location, pricing
- Booking and appointment requests

**Language:**
- English, Urdu, Roman Urdu
- Switches automatically based on customer

**Personal Help:**
- Calculations and conversions
- Translation between languages
- General advice and guidance

---

### The technical side:

Getting WhatsApp Business API working from scratch required:
- Creating a Meta Developer account and app
- Setting up a verified Business Portfolio
- Generating and managing OAuth access tokens
- Configuring webhooks for real-time message delivery
- Setting up WhatsApp Business Cloud node in n8n
- Understanding Meta's 24-hour messaging window policy

None of this was straightforward. Every step had its own setup process. But once it clicked, the whole thing came together.

---

### What I learned:

- How WhatsApp Business API actually works behind the scenes
- Meta's messaging policies and template vs free-form message rules
- OAuth token management for third-party API access
- Real-time webhook event handling
- Building conversational AI that feels human, not robotic

---

**Built with:** n8n · Groq API · Llama 3.3-70b · WhatsApp Business Cloud API · Meta Developer Platform · Webhook

---

