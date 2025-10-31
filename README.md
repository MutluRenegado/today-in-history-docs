🕰️ Today Engine

Automate History, Every Day.
(A.k.a. Daily Archive Publisher — your always-on storyteller)


(Example banner: sleek gradient with clock icon & tagline)

🌍 Overview

Today Engine automatically generates and publishes daily historical events from Wikipedia’s On This Day feed.
It’s an intelligent content engine that transforms data into stories — ready to share on your blog, GitHub Pages, or social media.

Build it once. Let it publish the past — forever.

✨ Features

✅ Daily Automation via GitHub Actions or Cloud Scheduler
✅ Beautiful Markdown Posts — fully formatted and linked
✅ Fun Facts Generator adds personality to your posts
✅ Multi-Platform Publishing (Blogger, WordPress, Medium, Notion)
✅ Free Hosting via GitHub Pages or custom domain
✅ Zero Maintenance — 100% automated after setup

⚙️ How It Works

Wikipedia Feed → Collects daily historical events via API

Filtering & Formatting → Curates key highlights before 1800

Markdown Generation → Creates a post like posts/YYYY-MM-DD.md

Publishing → Automatically posts to Blogger (or your chosen platform)

Archiving → Keeps all posts neatly stored in your repository

🧩 Example Output
😄 October 31

⚔️ 1517 – Martin Luther posts his 95 Theses on the Castle Church door in Wittenberg. [Wikipedia](https://en.wikipedia.org/wiki/Martin_Luther)  
🏰 1620 – The Pilgrims depart England aboard the Mayflower. [Wikipedia](https://en.wikipedia.org/wiki/Mayflower)

✨ Fun Fact  
🎩 In 1752, Britain skipped 11 days. People thought the government stole their lives!

😄 October 31 is celebrated as:  
- Halloween 🎃  
- World Cities Day 🌆

🚀 Quick Setup (GitHub)
1️⃣ Fork the Repository

Click Fork on the top right to clone it into your account.

2️⃣ Add Secrets

Go to
Settings → Secrets and variables → Actions → New repository secret

Add the following keys:

Name	Description
CLIENT_ID	Google OAuth client ID
CLIENT_SECRET	Google OAuth client secret
REFRESH_TOKEN	Blogger refresh token
BLOG_ID	Your Blogger blog ID
3️⃣ Enable GitHub Actions

Go to the Actions tab → “Today in History Automation” → Enable Workflow.

4️⃣ Watch It Work

Your first Markdown file will appear under:

posts/YYYY-MM-DD.md

🪄 Optional: Publish to Blogger

This project includes a ready-to-use Blogger publishing script:

python scripts/publish_to_blogger.py


You can adapt this for:

WordPress (via REST API)

Medium

Notion

LinkedIn or X (via API)

📦 Folder Structure
today-engine/
├── .github/
│   └── workflows/
│       └── today_in_history.yml     # Automation workflow
├── posts/                           # Generated daily Markdown posts
├── scripts/
│   ├── generate_history.py          # Wikipedia event scraper & formatter
│   ├── publish_to_blogger.py        # Blogger publisher
│   ├── get_token.py                 # Google OAuth helper
│   └── client_secret.json           # Ignored credentials
├── index.html                       # GitHub Pages front-end
├── requirements.txt                 # Python dependencies
└── README.md                        # You’re reading this

🧠 Tech Stack

Language: Python 3.11

Scheduler: GitHub Actions

Data Source: Wikipedia REST API

Deployment: GitHub Pages / Blogger

License: Apache 2.0

🗺️ Roadmap
Stage	Feature	Status
✅	Daily Markdown Generator	Complete
✅	Blogger Auto-Publish	Complete
⚙️	WordPress Integration	In Progress
⚙️	Medium / Notion Publishing	Planned
💡	AI Summaries (“Today in 1 Minute”)	Upcoming
🌐	SaaS Multi-User Dashboard	Future Release
💬 Tagline

“History doesn’t repeat — it auto-publishes.”

🪙 License

Licensed under the Apache License 2.0
You’re free to use, modify, and resell with attribution.

Copyright 2025 Mutlu Renegado

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

🧑‍💻 About the Creator

Created by Mutlu Renegado

→ Developer · Designer · Automation Enthusiast

“The past writes the stories — I just built the machine to tell them.”

⭐ Support the Project

If this project helped or inspired you:

⭐ Star the repository

🍴 Fork it and create your version

💬 Share it on social media

Together, we can make history — literally.
