# 🚀 Topic : Internet Basics

**Welcome to your web development journey!** Start here if you're new to computers and programming.

## ✅ Your Learning Checklist

### Week 1: Computer and Internet Basics
- [ ] **1**: File systems, folders, operating system navigation
  
  **🎯 Learning Objectives:** By the end of today, you'll understand how your computer organizes files and how to navigate using both visual and command-line interfaces.
  
  **📖 Theory (20 minutes):**
  
  **What is a File System?**
  - Your computer organizes all files and folders in a tree-like structure
  - Every file has a specific location called a "path"
  - Think of it like a mailing address for your files
  
  **File Paths Explained:**
  - **Absolute Path**: Complete address from the root (e.g., `/Users/yourname/Documents/project.txt`)
  - **Relative Path**: Address relative to current location (e.g., `./Documents/project.txt`)
  - **Root directory**: The top-level folder (Windows: `C:\`, Mac/Linux: `/`)
  
  **Common File Extensions:**
  - `.txt` - Text files
  - `.html` - Web pages
  - `.css` - Stylesheets
  - `.js` - JavaScript code
  - `.png/.jpg` - Images
  - `.pdf` - Documents
  
  **Command Line Basics**
  
  **Windows (Command Prompt):**
  # Open Command Prompt (Win+R, type cmd, Enter)

  ```cmd
  dir                    # List files in current directory
  cd Documents           # Change to Documents folder
  cd ..                  # Go up one level
  mkdir WebDev-Practice  # Create a new folder
  cd WebDev-Practice     # Enter the folder
  echo. > hello.txt      # Create an empty file
  dir                    # See your new file
  ```
  
  **Mac/Linux (Terminal):**
  # Open Terminal (Cmd+Space, type "terminal", Enter)

  ```bash
  ls                     # List files in current directory
  cd Documents           # Change to Documents folder
  cd ..                  # Go up one level
  mkdir WebDev-Practice  # Create a new folder
  cd WebDev-Practice     # Enter the folder
  touch hello.txt        # Create an empty file
  ls                     # See your new file
  pwd                    # See current path (print working directory)
  ```
  
  **💡 Key Takeaways:**
  - [x] I understand the difference between absolute and relative paths
  - [x] I can navigate using command line/terminal
  - [x] I know common file extensions and their purposes
  - [x] I can create folders and files using command line
  - [x] I understand the concept of "current directory"
  - [x] I know how to see where I am in the file system (`pwd` or current path)

- [ ] **2**: Client-server model, HTTP, URLs, domains, hosting
  
  **🎯 Learning Objectives:** Understand how the internet works, what happens when you visit a website, and the basic architecture of web communication.
  
  **📖 Theory (25 minutes):**
  
  **The Client-Server Model:**
  - **Client**: Your browser (Chrome, Firefox, Safari) that requests information
  - **Server**: A computer that stores websites and sends them back to you
  - **Communication**: They talk to each other using protocols (rules)
  
  **What Happens When You Type google.com:**
  1. **DNS Lookup**: Your browser asks "What's the address of google.com?"
  2. **Server Request**: Browser sends a request to Google's servers
  3. **Server Response**: Google's server sends back the website code
  4. **Browser Renders**: Your browser displays the website
  
  **Understanding URLs (Uniform Resource Locators):**
  ```
  https://www.example.com:443/path/to/page?param=value#section
  ^^^^    ^^^  ^^^^^^^  ^^^  ^^^^^^^^^^^^  ^^^^^^^^^^^^ ^^^^^^^
   |       |      |     |        |            |           |
  Protocol Sub   Domain Port    Path       Parameters   Fragment
  ```
  
  **Common Protocols:**
  - `http://` - Hypertext Transfer Protocol (not secure)
  - `https://` - HTTP Secure (encrypted, safe)
  - `ftp://` - File Transfer Protocol
  
  **Domain Name System (DNS):**
  - Converts human-readable names (google.com) to IP addresses (172.217.14.206)
  - Like a phone book for the internet
  - Managed by domain registrars (GoDaddy, Namecheap, etc.)
  
  **Web Hosting Types:**
  - **Shared**: Multiple websites share one server (cheap, basic)
  - **VPS**: Virtual Private Server (more control, medium cost)
  - **Dedicated**: Entire server for your website (expensive, full control)
  - **Cloud**: Multiple servers working together (scalable)
  
  **🛠️ Practical Exercises (35 minutes):**
  
  **Exercise 1: URL Dissection**
  1. Visit: `https://www.youtube.com/watch?v=dQw4w9WgXcQ`
  2. Break down this URL and identify:
     - Protocol: `https://`
     - Domain: `www.youtube.com`
     - Path: `/watch`
     - Parameters: `?v=dQw4w9WgXcQ`
  3. Try removing `www.` - does it still work?
  
  **Exercise 2: DNS Investigation**
  
  **Windows:**
  ```cmd
  # Open Command Prompt
  nslookup google.com    # Find Google's IP address
  ping google.com        # Test connection to Google
  tracert google.com     # See the route to Google
  ```
  
  **Mac/Linux:**
  ```bash
  # Open Terminal
  nslookup google.com    # Find Google's IP address
  ping google.com        # Test connection to Google (Ctrl+C to stop)
  traceroute google.com  # See the route to Google
  ```
  
  **Exercise 3: Browser Developer Tools**
  1. Visit any website (try `https://httpbin.org/get`)
  2. Press `F12` to open developer tools
  3. Go to the "Network" tab
  4. Refresh the page (F5)
  5. Watch the requests being made
  6. Click on the first request and examine:
     - Request Headers
     - Response Headers
     - Status Code
  
  **Exercise 4: Understanding Response Codes**
  Try visiting these URLs and note the response codes:
  - `https://httpbin.org/status/200` (Success)
  - `https://httpbin.org/status/404` (Not Found)
  - `https://httpbin.org/status/500` (Server Error)
  - `https://httpbin.org/redirect/3` (Redirect)
  
  **📚 Resources:**
  - [How DNS Works - Cloudflare](https://www.cloudflare.com/learning/dns/what-is-dns/)
  - [HTTP Status Codes - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
  - [What is a Web Server? - MDN](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server)
  - [Interactive: How the Internet Works](http://www.internetlivestats.com/)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Difficulty: [Easy/Medium/Hard]
  IP addresses I discovered: [Google, YouTube, etc.]
  Response codes I found: [200, 404, etc.]
  Most interesting discovery: [What surprised you?]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I understand the client-server model
  - [ ] I can break down a URL into its components
  - [ ] I know the difference between HTTP and HTTPS
  - [ ] I can use command line tools to investigate DNS
  - [ ] I understand what happens when I visit a website
  - [ ] I can use browser dev tools to see network requests
  - [ ] I know common HTTP status codes (200, 404, 500)

- [ ] **3**: Web browsers and developer tools
  
  **🎯 Learning Objectives:** Master browser developer tools to inspect, understand, and debug websites like a professional web developer.
  
  **📖 Theory (20 minutes):**
  
  **Browser Engines (How Browsers Work):**
  - **Chrome/Edge**: Blink engine (Google's rendering engine)
  - **Firefox**: Gecko engine (Mozilla's rendering engine)
  - **Safari**: WebKit engine (Apple's rendering engine)
  - Each engine may display websites slightly differently
  
  **What Browsers Do:**
  1. **Parse HTML**: Read the website's structure
  2. **Apply CSS**: Style the content with colors, fonts, layout
  3. **Execute JavaScript**: Run interactive code
  4. **Render**: Display the final webpage
  
  **Developer Tools Overview:**
  - Built into every modern browser
  - Essential for web development
  - Keyboard shortcut: `F12` or `Ctrl+Shift+I` (Windows), `Cmd+Option+I` (Mac)
  
  **🛠️ Practical Exercises (40 minutes):**
  
  **Exercise 1: Basic Developer Tools Navigation**
  1. Visit `https://www.wikipedia.org`
  2. Open developer tools (`F12`)
  3. Explore these tabs:
     - **Elements**: See HTML structure
     - **Console**: Run JavaScript commands
     - **Sources**: View website files
     - **Network**: Monitor requests (we used this yesterday!)
     - **Application**: View cookies, storage
  
  **Exercise 2: HTML Inspection**
  1. Visit `https://example.com` (simple website)
  2. Open Elements tab
  3. Hover over HTML elements - watch them highlight on page
  4. Click the arrow ▶️ next to `<html>` to expand
  5. Find the `<title>` element - this is what shows in browser tab
  6. Find the `<body>` element - this is what you see on page
  
  **Exercise 3: CSS Investigation**
  1. Right-click any text on the page
  2. Select "Inspect" or "Inspect Element"
  3. Look at the right panel - these are CSS styles
  4. Try changing something:
     - Click on a color value
     - Change font size number
     - Toggle checkboxes on/off
  5. Notice changes happen live on the page!
  
  **Exercise 4: Console Experiments**
  1. Click the "Console" tab
  2. Type these commands (press Enter after each):
  ```javascript
  alert("Hello from the console!")
  console.log("This appears in console")
  document.title = "I changed the title!"
  document.body.style.backgroundColor = "lightblue"
  ```
  3. Watch what happens to the page!
  
  **Exercise 5: Network Monitoring**
  1. Go to Network tab
  2. Visit `https://httpbin.org/json`
  3. Watch the network request
  4. Click on the request to see:
     - Headers (request info)
     - Response (what server sent back)
     - Timing (how long it took)
  
  **Exercise 6: Mobile Device Simulation**
  1. In dev tools, click the device icon 📱 (Toggle device toolbar)
  2. Try different devices: iPhone, iPad, etc.
  3. Notice how the website changes for different screen sizes
  4. This is called "responsive design"
  
  **📚 Resources:**
  - [Chrome DevTools Guide - Google](https://developers.google.com/web/tools/chrome-devtools)
  - [Firefox Developer Tools - MDN](https://developer.mozilla.org/en-US/docs/Tools)
  - [DevTools Tips](https://devtoolstips.org/) - Daily tips for developer tools
  - [Web Inspector - Apple](https://webkit.org/web-inspector/) (Safari)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Difficulty: [Easy/Medium/Hard]
  Favorite dev tool tab: [Elements/Console/Network/etc.]
  Cool thing I discovered: [What impressed you?]
  Website I inspected: [Which sites did you explore?]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I can open developer tools using F12
  - [ ] I understand the main dev tools tabs (Elements, Console, Network)
  - [ ] I can inspect HTML elements by right-clicking
  - [ ] I can see and modify CSS styles in real-time
  - [ ] I can run JavaScript commands in the console
  - [ ] I can simulate different devices/screen sizes
  - [ ] I understand how browsers render websites
  - [ ] I can monitor network requests and responses

- [ ] **4**: Text editors and IDEs
  
  **🎯 Learning Objectives:** Choose and set up a professional code editor that will be your primary tool for web development.
  
  **📖 Theory (15 minutes):**
  
  **What is a Code Editor?**
  - Specialized text editor designed for writing code
  - Features that regular text editors don't have:
    - Syntax highlighting (colors for different code parts)
    - Auto-completion
    - Error detection
    - File management
    - Extensions/plugins
  
  **Popular Code Editors:**
  - **VS Code** (Free, Microsoft) - Most popular, great for beginners
  - **Sublime Text** (Paid, fast and lightweight)
  - **Atom** (Free, GitHub) - Being discontinued
  - **WebStorm** (Paid, JetBrains) - Full IDE with many features
  - **Vim/Neovim** (Free, advanced users only)
  
  **IDE vs Text Editor:**
  - **Text Editor**: Just for writing code
  - **IDE** (Integrated Development Environment): Editor + debugger + compiler + more
  
  **🛠️ Practical Exercises (45 minutes):**
  
  **Exercise 1: Install VS Code (Recommended)**
  1. Go to `https://code.visualstudio.com/`
  2. Download for your operating system
  3. Install it (follow default options)
  4. Open it - you should see a welcome screen
  
  **Exercise 2: Basic VS Code Navigation**
  1. Create a new file: `Ctrl+N` (Windows) or `Cmd+N` (Mac)
  2. Save it as `hello.html`: `Ctrl+S` or `Cmd+S`
  3. Type this simple HTML:
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>My First Page</title>
    </head>
    <body>
      <h1>Hello World!</h1>
      <p>This is my first HTML page.</p>
    </body>
  </html>
  ```
  4. Notice the syntax highlighting (colors)!
  
  **Exercise 3: Essential Keyboard Shortcuts**
  Practice these shortcuts in VS Code:
  ```
  Ctrl/Cmd + N        → New file
  Ctrl/Cmd + O        → Open file
  Ctrl/Cmd + S        → Save file
  Ctrl/Cmd + Z        → Undo
  Ctrl/Cmd + Y        → Redo
  Ctrl/Cmd + F        → Find in file
  Ctrl/Cmd + H        → Find and replace
  Ctrl/Cmd + D        → Select next occurrence
  Ctrl/Cmd + /        → Comment/uncomment line
  Alt + Up/Down       → Move line up/down
  ```
  
  **Exercise 4: File Explorer**
  1. Create a folder called "my-first-website"
  2. Open this folder in VS Code: File → Open Folder
  3. Create new files using the sidebar:
     - `index.html`
     - `style.css`
     - `script.js`
  4. Notice how VS Code shows your project structure
  
  **Exercise 5: Extensions**
  1. Click the Extensions icon in the sidebar (or `Ctrl/Cmd+Shift+X`)
  2. Install these helpful extensions:
     - "Live Server" (preview HTML files)
     - "Auto Rename Tag" (HTML helper)
     - "Prettier" (code formatter)
  3. After installing Live Server, right-click your HTML file and select "Open with Live Server"
  
  **📚 Resources:**
  - [VS Code Documentation](https://code.visualstudio.com/docs)
  - [VS Code Keyboard Shortcuts PDF](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
  - [Essential VS Code Extensions](https://marketplace.visualstudio.com/VSCode)
  - [Alternative Editors Comparison](https://www.slant.co/topics/1686/~best-programming-text-editors)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Difficulty: [Easy/Medium/Hard]
  Editor I chose: [VS Code/Sublime/Other]
  Extensions I installed: [List them]
  Favorite shortcut: [Which shortcut impressed you?]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I have a professional code editor installed and configured
  - [ ] I understand the difference between text editors and IDEs
  - [ ] I can create, save, and organize files in my editor
  - [ ] I know essential keyboard shortcuts for efficiency
  - [ ] I can install and use extensions to enhance my editor
  - [ ] I can preview HTML files using Live Server or similar
  - [ ] I understand syntax highlighting and its benefits

- [ ] **5**: Version control introduction
  
  **🎯 Learning Objectives:** Understand version control concepts and why every developer needs to track changes to their code.
  
  **📖 Theory (25 minutes):**
  
  **What is Version Control?**
  - System that tracks changes to files over time
  - Like "save states" in video games - you can go back to any previous version
  - Essential for collaboration with other developers
  - Backup system for your code
  
  **Why Do We Need It?**
  - **Safety**: Never lose your work
  - **History**: See what changed and when
  - **Collaboration**: Multiple people working on same project
  - **Experimentation**: Try new features without breaking existing code
  - **Blame/Credit**: See who made what changes
  
  **Git vs GitHub (Common Confusion):**
  - **Git**: The version control system (software on your computer)
  - **GitHub**: Online service to store Git repositories (like Google Drive for code)
  - Other alternatives: GitLab, Bitbucket
  
  **Key Git Concepts:**
  - **Repository (Repo)**: A project folder tracked by Git
  - **Commit**: A saved snapshot of your project
  - **Branch**: Different versions/features of your project
  - **Clone**: Download a repository from online to your computer
  - **Push**: Upload your changes to online repository
  - **Pull**: Download changes from online repository
  
  **🛠️ Practical Exercises (35 minutes):**
  
  **Exercise 1: Install Git**
  
  **Windows:**
  1. Go to `https://git-scm.com/download/win`
  2. Download and install (use default options)
  3. Open "Git Bash" from start menu
  
  **Mac:**
  ```bash
  # Option 1: Install Xcode Command Line Tools
  xcode-select --install
  
  # Option 2: Use Homebrew (if you have it)
  brew install git
  ```
  
  **Linux (Ubuntu/Debian):**
  ```bash
  sudo apt update
  sudo apt install git
  ```
  
  **Exercise 2: First Git Setup**
  ```bash
  # Configure your identity (use your real name and email)
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  
  # Check your configuration
  git config --list
  ```
  
  **Exercise 3: Create Your First Repository**
  ```bash
  # Create a new folder for your project
  mkdir my-first-repo
  cd my-first-repo
  
  # Initialize Git in this folder
  git init
  
  # Check status
  git status
  ```
  
  **Exercise 4: Track Changes**
  ```bash
  # Create a simple file
  echo "Hello Git!" > README.txt
  
  # See what Git thinks about this new file
  git status
  
  # Add the file to staging area
  git add README.txt
  
  # Commit (save) the changes
  git commit -m "Add README file"
  
  # See your commit history
  git log
  ```
  
  **Exercise 5: Make More Changes**
  ```bash
  # Edit the file (add more content)
  echo "This is my first Git repository!" >> README.txt
  
  # See what changed
  git status
  git diff
  
  # Add and commit the changes
  git add README.txt
  git commit -m "Update README with description"
  
  # See all commits
  git log --oneline
  ```
  
  **📚 Resources:**
  - [Git Official Tutorial](https://git-scm.com/docs/gittutorial)
  - [GitHub Git Handbook](https://guides.github.com/introduction/git-handbook/)
  - [Interactive Git Tutorial](https://learngitbranching.js.org/)
  - [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Difficulty: [Easy/Medium/Hard]
  My first commit message: [What did you write?]
  Git commands I learned: [List them]
  Most confusing concept: [What needs more practice?]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I understand what version control is and why it's important
  - [ ] I have Git installed and configured on my computer
  - [ ] I know the difference between Git and GitHub
  - [ ] I can create a new Git repository with `git init`
  - [ ] I can track changes with `git add` and `git commit`
  - [ ] I can check the status of my repository with `git status`
  - [ ] I can see my commit history with `git log`
  - [ ] I understand the basic Git workflow: edit → add → commit

- [ ] **Day 6**: Package managers and dependencies
  
  **🎯 Learning Objectives:** Understand how modern software uses external libraries and how package managers help organize code dependencies.
  
  **📖 Theory (20 minutes):**
  
  **What are Packages/Libraries?**
  - **Package**: Pre-written code that solves common problems
  - **Library**: Collection of functions you can use in your code
  - **Framework**: More structured, tells you how to organize your code
  - Instead of writing everything from scratch, use existing solutions
  
  **Why Use Packages?**
  - **Save Time**: Don't reinvent the wheel
  - **Quality**: Tested by thousands of developers
  - **Security**: Maintained and updated regularly
  - **Standards**: Industry-proven solutions
  
  **Package Managers by Language:**
  - **JavaScript**: npm (Node Package Manager), yarn
  - **Python**: pip (Pip Installs Packages)
  - **Ruby**: gem
  - **PHP**: Composer
  - **Java**: Maven, Gradle
  
  **Dependency Concepts:**
  - **Dependency**: A package your project needs
  - **Transitive Dependencies**: Dependencies of your dependencies
  - **Version**: Different releases of the same package
  - **Semantic Versioning**: Major.Minor.Patch (e.g., 2.1.3)
  
  **🛠️ Practical Exercises (40 minutes):**
  
  **Exercise 1: Explore npm (Node Package Manager)**
  1. Visit `https://www.npmjs.com/`
  2. Search for popular packages:
     - "lodash" (utility library)
     - "express" (web framework)
     - "react" (UI library)
  3. Look at each package page and notice:
     - Download numbers per week
     - Version history
     - Documentation
     - Dependencies section
  
  **Exercise 2: Understanding package.json**
  Create a simple `package.json` file to understand structure:
  ```json
  {
    "name": "my-first-project",
    "version": "1.0.0",
    "description": "Learning about packages",
    "dependencies": {
      "lodash": "^4.17.21"
    },
    "devDependencies": {
      "prettier": "^2.8.0"
    }
  }
  ```
  
  **Exercise 3: Python pip Exploration**
  If you have Python installed:
  ```bash
  # Check if pip is installed
  pip --version
  
  # Search for packages
  pip search requests
  
  # See installed packages
  pip list
  ```
  
  **Exercise 4: Understanding Semantic Versioning**
  Practice reading version numbers:
  - `1.2.3` = Major.Minor.Patch
  - `^1.2.3` = Compatible with 1.2.3, up to 2.0.0
  - `~1.2.3` = Compatible with 1.2.3, up to 1.3.0
  - `1.2.3` = Exactly 1.2.3
  
  **Exercise 5: Investigate a Real Project**
  1. Visit a popular GitHub project: `https://github.com/facebook/react`
  2. Look for `package.json` file
  3. Count how many dependencies it has
  4. Notice the version constraints
  
  **📚 Resources:**
  - [npm Documentation](https://docs.npmjs.com/)
  - [Semantic Versioning](https://semver.org/)
  - [Package.json Guide](https://docs.npmjs.com/cli/v8/configuring-npm/package-json)
  - [Dependency Management Best Practices](https://docs.npmjs.com/cli/v8/using-npm/dependency-selectors)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Difficulty: [Easy/Medium/Hard]
  Interesting package I found: [Name and what it does]
  Package managers I know about: [npm, pip, etc.]
  Biggest insight: [What made sense about dependencies?]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I understand what packages and libraries are
  - [ ] I know why developers use external dependencies
  - [ ] I'm familiar with different package managers (npm, pip, etc.)
  - [ ] I understand semantic versioning (Major.Minor.Patch)
  - [ ] I can read a package.json file
  - [ ] I know the difference between dependencies and devDependencies
  - [ ] I understand that packages can have their own dependencies

- [ ] **Day 7**: Review and practice
  
  **🎯 Learning Objectives:** Consolidate your learning from Week 1 and set up a complete development environment ready for Week 2.
  
  **📖 Review Session (20 minutes):**
  
  **Quick Self-Assessment:**
  Go back through Days 1-6 and check off any items you missed. Focus on:
  - [ ] Can I navigate my computer using command line?
  - [ ] Do I understand how websites work (client-server)?
  - [ ] Am I comfortable with browser developer tools?
  - [ ] Is my code editor set up and configured?
  - [ ] Do I understand Git basics?
  - [ ] Do I know what package managers do?
  
  **🛠️ Practical Exercises (40 minutes):**
  
  **Exercise 1: Complete Development Environment Setup**
  Create your development environment checklist:
  
  ✅ **Essential Software:**
  - [ ] Web Browser (Chrome/Firefox with dev tools)
  - [ ] Code Editor (VS Code with extensions)
  - [ ] Git (configured with your name/email)
  - [ ] Terminal/Command Line access
  
  ✅ **VS Code Extensions (if using VS Code):**
  - [ ] Live Server
  - [ ] Auto Rename Tag
  - [ ] Prettier
  - [ ] GitLens (helps with Git)
  
  **Exercise 2: Create Your Learning Project Structure**
  ```bash
  # Create your main learning folder
  mkdir WebDev-Journey
  cd WebDev-Journey
  
  # Initialize Git
  git init
  
  # Create weekly folders
  mkdir Week1-Basics Week2-Internet Week3-WebTech Week4-Modern
  
  # Create a main README
  echo "# My Web Development Journey" > README.md
  echo "" >> README.md
  echo "## Week 1: Computer and Internet Basics" >> README.md
  echo "- [x] Day 1: File systems and navigation" >> README.md
  echo "- [x] Day 2: Client-server model" >> README.md
  echo "- [x] Day 3: Browser developer tools" >> README.md
  echo "- [x] Day 4: Code editors" >> README.md
  echo "- [x] Day 5: Version control basics" >> README.md
  echo "- [x] Day 6: Package managers" >> README.md
  echo "- [x] Day 7: Environment setup" >> README.md
  
  # Add and commit
  git add .
  git commit -m "Initial project setup and Week 1 completion"
  ```
  
  **Exercise 3: Command Line Practice Challenge**
  Complete this sequence without looking at notes:
  ```bash
  # Navigate to your home directory
  cd ~
  
  # Create a test folder
  mkdir command-practice
  cd command-practice
  
  # Create some files
  touch index.html style.css script.js
  
  # List files
  ls    # (Mac/Linux) or dir (Windows)
  
  # Create a subfolder
  mkdir assets
  cd assets
  
  # Create an image placeholder
  touch logo.png
  
  # Go back up
  cd ..
  
  # See your full path
  pwd   # (Mac/Linux) or cd (Windows)
  
  # Clean up
  cd ..
  rm -r command-practice  # (Mac/Linux) or rmdir /s command-practice (Windows)
  ```
  
  **Exercise 4: Browser Tools Practice**
  1. Visit `https://httpbin.org/html`
  2. Open developer tools
  3. Complete these tasks:
     - Find the `<h1>` element
     - Change its text color to red
     - Add a new paragraph element
     - Check the Network tab for the request
     - Use the console to run: `alert("Week 1 Complete!")`
  
  **Exercise 5: Create Your First Web Page**
  In your code editor, create a simple HTML file:
  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Week 1 Complete!</title>
      <style>
        body {
          font-family: Arial, sans-serif;
          max-width: 600px;
          margin: 0 auto;
          padding: 20px;
        }
        .celebration {
          color: #28a745;
          font-size: 2em;
        }
      </style>
    </head>
    <body>
      <h1 class="celebration">🎉 Week 1 Complete!</h1>
      <h2>What I Learned:</h2>
      <ul>
        <li>File systems and command line navigation</li>
        <li>How the internet works (client-server model)</li>
        <li>Browser developer tools</li>
        <li>Code editor setup and shortcuts</li>
        <li>Version control with Git</li>
        <li>Package managers and dependencies</li>
      </ul>
      
      <h2>Ready for Week 2:</h2>
      <p>I'm prepared to dive deeper into internet infrastructure and protocols!</p>
      
      <script>
        console.log("Week 1 learning journey complete!");
      </script>
    </body>
  </html>
  ```
  Save as `week1-complete.html` and view in browser!
  
  **📚 Resources:**
  - [Developer Roadmap](https://roadmap.sh/frontend) - See the bigger picture
  - [freeCodeCamp](https://www.freecodecamp.org/) - Continue learning
  - [MDN Learn Web Development](https://developer.mozilla.org/en-US/docs/Learn)
  
  **📝 My Notes:**
  ```
  Date completed: [Add date when you finish this day]
  Time spent: [Track your learning time]
  Week 1 difficulty: [How was the overall week?]
  Proudest achievement: [What are you most proud of?]
  Area needing more practice: [What should you review?]
  Excitement level for Week 2: [1-10 scale]
  ```
  
  **💡 Key Takeaways:**
  - [ ] I have a complete development environment set up
  - [ ] I can navigate confidently using command line
  - [ ] I understand the basic flow of how websites work
  - [ ] I'm comfortable using browser developer tools
  - [ ] I have Git configured and understand basic workflow
  - [ ] I created my first web page with HTML, CSS, and JavaScript
  - [ ] I'm ready to dive deeper into internet technologies
  - [ ] I have a system for tracking my learning progress

### Week 2: Internet Infrastructure and Protocols
- [ ] **8**: How the internet works
  - Internet vs World Wide Web
  - ISPs, routers, and data transmission
  - IP addresses and how they work

- [ ] **9**: Domain Name System (DNS)
  - How domain names are resolved
  - DNS records (A, CNAME, MX, etc.)
  - DNS propagation and caching

- [ ] **10**: HTTP and HTTPS protocols
  - HTTP methods (GET, POST, PUT, DELETE)
  - HTTP status codes (200, 404, 500, etc.)
  - Headers and request/response structure

- [ ] **11**: Web servers and hosting
  - What is a web server?
  - Static vs dynamic hosting
  - Shared, VPS, and dedicated hosting

- [ ] **12**: APIs and data exchange
  - What is an API?
  - REST API basics
  - JSON and XML data formats

- [ ] **13**: Databases fundamentals
  - What are databases?
  - SQL vs NoSQL overview
  - How web apps store data

- [ ] **14**: Review and exploration
  - Use browser dev tools to examine HTTP requests
  - Look up a website's DNS records
  - Practice understanding URL structure

### Week 3: Web Technologies and Browsers
- [ ] **15**: HTML fundamentals
  - Document structure and semantic elements
  - How browsers parse HTML
  - HTML validation and best practices

- [ ] **16**: CSS fundamentals
  - How styles are applied to HTML
  - CSS specificity and cascade
  - Browser default styles

- [ ] **17**: JavaScript basics
  - What JavaScript does in browsers
  - Client-side vs server-side scripting
  - JavaScript execution in browsers

- [ ] **18**: Web standards and compatibility
  - W3C and web standards
  - Browser differences and compatibility
  - Progressive enhancement

- [ ] **19**: Responsive web design
  - Mobile vs desktop web
  - Viewport and media queries
  - Touch vs mouse interaction

- [ ] **20**: Web accessibility
  - What is web accessibility?
  - Screen readers and assistive technology
  - WCAG guidelines basics

- [ ] **21**: Review and hands-on
  - Create a simple HTML page
  - Test it in different browsers
  - Use accessibility tools

### Week 4: Security, Performance, and Modern Web
- [ ] **22**: Web security basics
  - HTTPS and SSL/TLS certificates
  - Common security vulnerabilities
  - Safe browsing practices

- [ ] **23**: Web performance
  - Why website speed matters
  - Browser caching and optimization
  - Image optimization and compression

- [ ] **24**: Modern web development
  - Single Page Applications (SPAs)
  - Progressive Web Apps (PWAs)
  - Mobile-first development

- [ ] **25**: Content Delivery Networks
  - What is a CDN?
  - How CDNs improve performance
  - Popular CDN services

- [ ] **26**: Monitoring and analytics
  - Website analytics basics
  - Performance monitoring tools
  - Error tracking and debugging

- [ ] **27**: Future of the web
  - Web3 and blockchain concepts
  - AI integration in web development
  - Emerging web technologies

- [ ] **28**: Final review and next steps
  - Review key concepts
  - Assess your learning
  - Plan your next learning phase

## 📚 Essential Resources

### Documentation and References
- [MDN Web Docs](https://developer.mozilla.org/) - Comprehensive web development documentation
- [W3Schools](https://www.w3schools.com/) - Beginner-friendly tutorials
- [Can I Use](https://caniuse.com/) - Browser compatibility checker

### Tools for Learning
- **Browser Developer Tools** - Built into Chrome, Firefox, Safari, Edge
- **Text Editors** - VS Code, Sublime Text, Atom
- **Online Playgrounds** - CodePen, JSFiddle, Repl.it

### Books for Deeper Learning
- "How the Internet Works" by Preston Gralla
- "HTTP: The Definitive Guide" by David Gourley
- "Web Performance in Action" by Jeremy Wagner

## 🎯 Next Steps After Completion

Once you complete this internet basics course, you'll be ready to dive into:

1. **HTML & CSS Fundamentals** - Start building actual web pages
2. **JavaScript Basics** - Add interactivity to your websites  
3. **Version Control with Git** - Learn professional development workflows
4. **Command Line Mastery** - Become more efficient with terminal commands

## 📋 Study Tips

- **Take Notes**: Write down key concepts in your own words
- **Practice Regularly**: Set aside 30-60 minutes daily
- **Ask Questions**: Use forums like Stack Overflow when stuck
- **Build Projects**: Apply what you learn with small projects
- **Stay Curious**: Explore topics that interest you beyond the checklist

---
*Keep this file updated with your progress! Check off completed items and add your own notes.*
