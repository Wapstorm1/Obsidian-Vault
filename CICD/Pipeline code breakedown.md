* #### **agent any**
🤖 This tells Jenkins:
> “Use **any available agent (machine)** to run this pipeline.”
💡 Jenkins picks a worker node (or Docker container) to execute the pipeline steps.

* #### **environment { ... }**
🌎 This block defines **environment variables** you’ll use throughout the pipeline.

---
#### **NETLIFY_SITE_ID = 'YOUR NETLIFY SITE ID'**
This variable holds the unique ID for your Netlify site.

📨 Netlify CLI uses this to know **which site to deploy to.**

---
#### **NETLIFY_AUTH_TOKEN = credentials('netlify-token')**
🔐 This pulls a **secure credential** (your Netlify token) from Jenkins’ credentials store.
That way, your token stays safe and is not hard-coded.

---
#### **REACT_APP_VERSION = "1.0.$BUILD_ID"**
This defines a **custom version number** for your app.

$BUILD_ID is a built-in Jenkins variable that auto-increments with every run.
💡 This version could be used in your app or in your deployment label.


* #### **reuseNode true**
This means:
> “Keep using the same Jenkins workspace folder for all stages on this agent.”
This helps later stages (like Tests or Deploy) reuse files like the build/ folder.

* #### **npm test**
🎯 Runs your unit tests — based on the "test" script in package.json:


* #### **post { always { junit ... } }**
📊 This **publishes your test results** to Jenkins
Even if the test fails, Jenkins will still attach the results!

* #### **npm install serve**
📦 This installs the serve package — a tiny tool that can serve your built site (in the build/ folder) on a local web server.
> Your Playwright tests need the website to **actually run**, so this makes it live at something like http://localhost:3000

* #### **node_modules/.bin/serve -s build &**

🌐 This starts the local web server **in the background**:

--s build means:
    
    > “Serve the build/ folder as a static website”
    
- & means:
    > “Run this in the background so the next command can also run”
Without &, the script would stop here and wait forever.


