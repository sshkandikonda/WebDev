# 🚀 Topic : Internet Basics

**Welcome to your web development journey!** Start here if you're new to computers and programming.

## Week 1: Computer and Internet Basics
### **1**: File systems, folders, operating system navigation
  
  **🎯 Learning Objectives:** By the end of today, you'll understand how your computer organizes files and how to navigate using both visual and command-line interfaces.
  
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
  - Open Command Prompt (Win+R, type cmd, Enter)

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
  - Open Terminal (Cmd+Space, type "terminal", Enter)

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
  
### **2**: Client-server model, HTTP, URLs, domains, hosting
  
  **🎯 Learning Objectives:** Understand how the internet works, what happens when you visit a website, and the basic architecture of web communication.
  
  **Computer Networking:** A computer network is a communication system where a group of computers and other devices/resources are connected. The data is shared among these devices in the group. A network also allows both resources to be shared and the data transfer among the systems connected. This concept of connecting a computer to others is called networking.

  **The Client-Server Model Or Components of the Network:**
  - **Client**: Your browser (Chrome, Firefox, Safari) that requests information; Computers that access shared network resources provided by the server
  - **Server**: A computer that stores websites and sends them back to you; Computers that provide shared resources to network users
  - **Communication**: They talk to each other using protocols (rules); The way in which computers are connected
  
  - **Modem**: When there is a wired transfer happening between computers, then the electronic signals are converted into electric signals through cables. This is where a modem (Modulator-Demodulator) helps. It converts the digital signals to modulation. It is a hardware device that does this job at the client's end (Modem modulates the signal). At the reciever's end, this analog signal is converted back to digital (modem demodulates the signal). This is how a wired communication works.

  **Types of Network**: 

  - **Local Area Network (LAN):** In this networking type, the devices are confined to a single location like in a building or complex. The maximum distance from one end of a network to another is limited by the signal strength or the network's built in limit for sending and receiving messages through a physical connection like cable.

  - **Wide Area Network (WAN):** When network is spread across cities, states or even countries, it is called Wide Area Network. Communication takes place either via telephone lines, satellites or microwave links rather than cables.

  - **Meltropolitan Area Network (MAN):** This type of network covers an entire city. best example is a cable television network. The information is carried in the form of computer signals using cables.

  **Network Topology**:
  
  Topology explains us how devices are arranged in a network and what devices act as controller or hub and what are the nodes.
  
  **Types of Network Topologies:**
  
  - **Bus Topology**: All devices are connected to a single central cable (backbone). Data travels in both directions along the bus. If the main cable fails, the entire network goes down. Simple but not fault-tolerant.
  
  - **Star Topology**: All devices are connected to a central hub or switch. This is the most common topology in modern networks (like your home WiFi router). If the central device fails, the network goes down, but individual device failures don't affect others.
  
  - **Ring Topology**: Devices are connected in a circular fashion, forming a closed loop. Data travels in one direction around the ring. Each device acts as a repeater. If one device fails, it can disrupt the entire network.
  
  - **Mesh Topology**: Every device is connected to every other device. Provides maximum redundancy and fault tolerance, but is expensive and complex to set up. Used in critical applications where reliability is essential.
  
  - **Tree/Hierarchical Topology**: Combines star and bus topologies in a hierarchical structure. Has a root node with multiple levels branching out. Common in large organizations with multiple departments. 

  **Internet and DNS essentials**

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
  
  **Detailed DNS Resolution Process:**
  1. **Browser Cache Check**: First checks if IP address is already stored locally
  2. **Operating System Cache**: Checks OS-level DNS cache
  3. **Router Cache**: Your home router may have the IP cached
  4. **ISP DNS Server**: Your internet provider's DNS server is queried
  5. **Root Name Servers**: If not found, query goes to root servers (13 worldwide)
  6. **TLD Servers**: Root servers direct to Top-Level Domain servers (.com, .org, etc.)
  7. **Authoritative Servers**: TLD servers point to the domain's authoritative name servers
  8. **Final Resolution**: Authoritative servers return the actual IP address
  
  **DNS Record Types:**
  - **A Record**: Maps domain name to IPv4 address (e.g., example.com → 93.184.216.34)
  - **AAAA Record**: Maps domain name to IPv6 address
  - **CNAME Record**: Maps alias to another domain (e.g., www.example.com → example.com)
  - **MX Record**: Specifies mail servers for the domain
  - **NS Record**: Identifies authoritative name servers for the domain
  - **TXT Record**: Stores text information (often used for verification)
  
  **Internet Infrastructure Components:**
  
  **Internet Backbone:**
  - High-capacity networks that carry internet traffic across continents
  - Operated by Tier 1 ISPs (AT&T, Verizon, Level 3)
  - Connected via undersea cables, fiber optic networks, and satellite links
  
  **Internet Exchange Points (IXPs):**
  - Physical locations where different networks connect and exchange traffic
  - Reduce latency and improve performance
  - Examples: DE-CIX in Germany, AMS-IX in Amsterdam
  
  **Content Delivery Networks (CDNs):**
  - Distributed network of servers that cache website content
  - Serve content from server closest to user's location
  - Examples: Cloudflare, AWS CloudFront, Akamai
  
  **Internet Protocols Hierarchy:**
  - **Physical Layer**: Cables, WiFi signals, fiber optics
  - **Data Link Layer**: Ethernet, WiFi protocols
  - **Network Layer**: IP (Internet Protocol) for routing
  - **Transport Layer**: TCP (reliable) and UDP (fast) protocols
  - **Application Layer**: HTTP, HTTPS, FTP, SMTP protocols
  
  **Web Hosting Types:**
  - **Shared**: Multiple websites share one server (cheap, basic)
  - **VPS**: Virtual Private Server (more control, medium cost)
  - **Dedicated**: Entire server for your website (expensive, full control)
  - **Cloud**: Multiple servers working together (scalable)
  
  **Domain Name Structure:**
  ```
  subdomain.example.com
  ^^^^^^^^^  ^^^^^^^  ^^^
      |         |      |
  Subdomain  Domain   TLD
             Name   (Top-Level Domain)
  ```
  
  **Internet vs World Wide Web:**
  - **Internet**: The global network infrastructure (hardware, protocols, connections)
  - **World Wide Web**: A service that runs on the internet (websites, web pages, browsers)
  - Think of Internet as the highway system, and the Web as the cars driving on it
  
  **DNS Investigation**
  
  **Windows:**
  ```cmd
  - Open Command Prompt
  nslookup google.com    # Find Google's IP address
  ping google.com        # Test connection to Google
  tracert google.com     # See the route to Google
  ```
  
  **Mac/Linux:**
  ```bash
  - Open Terminal
  nslookup google.com    # Find Google's IP address
  ping google.com        # Test connection to Google (Ctrl+C to stop)
  traceroute google.com  # See the route to Google
  ```
  
  **Browser Developer Tools**
  1. Visit any website (try `https://httpbin.org/get`)
  2. Press `F12` to open developer tools
  3. Go to the "Network" tab
  4. Refresh the page (F5)
  5. Watch the requests being made
  6. Click on the first request and examine:
     - Request Headers
     - Response Headers
     - Status Code
  
  **Understanding Response Codes**
  
  **HTTP Status Code Categories:**
  
  **1xx - Informational Responses:**
  - `100 Continue` - Server received request headers, client should continue
  - `101 Switching Protocols` - Server switching protocols per client request
  - `102 Processing` - Server received and processing request (no response yet)
  
  **2xx - Success Responses:**
  - `200 OK` - Request succeeded, most common success code
  - `201 Created` - Request succeeded, new resource was created
  - `202 Accepted` - Request accepted but not yet processed
  - `204 No Content` - Request succeeded but no content to return
  - `206 Partial Content` - Server delivering partial resource (range requests)
  
  **3xx - Redirection Messages:**
  - `300 Multiple Choices` - Multiple options for resource available
  - `301 Moved Permanently` - Resource permanently moved to new URL
  - `302 Found` - Resource temporarily moved (temporary redirect)
  - `304 Not Modified` - Resource not modified, use cached version
  - `307 Temporary Redirect` - Resource temporarily moved, method unchanged
  - `308 Permanent Redirect` - Resource permanently moved, method unchanged
  
  **4xx - Client Error Responses:**
  - `400 Bad Request` - Server cannot process due to client error
  - `401 Unauthorized` - Authentication required to access resource
  - `403 Forbidden` - Server understood but refuses to authorize
  - `404 Not Found` - Server cannot find the requested resource
  - `405 Method Not Allowed` - Request method not supported
  - `408 Request Timeout` - Server timed out waiting for request
  - `409 Conflict` - Request conflicts with current server state
  - `410 Gone` - Resource no longer available permanently
  - `413 Payload Too Large` - Request entity larger than server limits
  - `418 I'm a Teapot` - Server refuses to brew coffee (April Fools' joke RFC)
  - `429 Too Many Requests` - Client sent too many requests (rate limiting)
  
  **5xx - Server Error Responses:**
  - `500 Internal Server Error` - Generic server error message
  - `501 Not Implemented` - Server doesn't support requested functionality
  - `502 Bad Gateway` - Server received invalid response from upstream
  - `503 Service Unavailable` - Server temporarily overloaded or down
  - `504 Gateway Timeout` - Server didn't receive response from upstream
  - `505 HTTP Version Not Supported` - HTTP version not supported
  - `511 Network Authentication Required` - Client needs to authenticate
  
  **Most Common Codes You'll Encounter:**
  - **200**: Everything worked perfectly ✅
  - **301/302**: Page moved to different location 🔄
  - **404**: Page doesn't exist (broken link) ❌
  - **500**: Something broke on the server 💥
  - **503**: Server is temporarily down 🚧

### **3**: Web browsers and developer tools
  
  **🎯 Learning Objectives:** Master browser developer tools to inspect, understand, and debug websites like a professional web developer.
  
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

### **4**: Text editors and IDEs
  
  **🎯 Learning Objectives:** Choose and set up a professional code editor that will be your primary tool for web development.
  
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

### **5**: Version control introduction
  
  **🎯 Learning Objectives:** Understand version control concepts and why every developer needs to track changes to their code.
  
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

  **All Git commands:**
  
  **Repository Setup:**
  - `git init` - Initialize a new Git repository
  - `git clone <url>` - Clone a repository from remote URL
  - `git remote add origin <url>` - Add remote repository
  - `git remote -v` - View remote repositories
  
  **Basic Workflow:**
  - `git status` - Check repository status
  - `git add <file>` - Stage specific file for commit
  - `git add .` - Stage all files for commit
  - `git commit -m "message"` - Commit staged changes with message
  - `git commit -am "message"` - Stage and commit all tracked files
  
  **Viewing History:**
  - `git log` - View commit history
  - `git log --oneline` - View compact commit history
  - `git log --graph` - View commit history with branch graph
  - `git log --stat` - View commit history with file change statistics
  - `git log -p` - View commit history with full diff
  - `git show <commit>` - View specific commit details
  - `git diff` - View unstaged changes
  - `git diff --staged` - View staged changes
  
  **Branch Management:**
  - `git branch` - List all local branches
  - `git branch -r` - List remote branches
  - `git branch -a` - List all branches (local and remote)
  - `git branch <name>` - Create new branch
  - `git checkout <branch>` - Switch to branch
  - `git checkout -b <name>` - Create and switch to new branch
  - `git merge <branch>` - Merge branch into current branch
  - `git branch -d <name>` - Delete branch
  
  **Remote Operations:**
  - `git push` - Push commits to remote repository
  - `git push origin <branch>` - Push specific branch to remote
  - `git push -u origin <branch>` - Push and set upstream tracking
  - `git pull` - Fetch and merge changes from remote
  - `git fetch` - Fetch changes without merging
  - `git remote rm origin` - Remove remote repository
  
  **Undoing Changes:**
  - `git reset <file>` - Unstage file
  - `git reset --hard` - Discard all local changes
  - `git checkout -- <file>` - Discard changes to specific file
  - `git revert <commit>` - Create new commit that undoes previous commit
  
  **Configuration:**
  - `git config --global user.name "Name"` - Set username
  - `git config --global user.email "email"` - Set email
  - `git config --list` - View all configuration settings
  
  **File Operations:**
  - `git mv <old> <new>` - Move/rename file
  - `git rm <file>` - Remove file from Git and working directory
  - `git clean -n` - Preview untracked files to be deleted
  - `git clean -f` - Remove untracked files
  
  **Advanced Operations:**
  - `git commit --amend` - Modify last commit
  - `git cherry-pick <commit>` - Apply specific commit to current branch
  - `git blame <file>` - See who modified each line of a file
  - `git reset --soft <commit>` - Reset but keep changes staged
  
  **Rebasing:**
  - `git rebase <branch>` - Rebase current branch onto another branch
  - `git rebase -i <commit>` - Interactive rebase to edit commit history
  - `git rebase --continue` - Continue rebase after resolving conflicts
  - `git rebase --abort` - Cancel rebase and return to original state
  - `git pull --rebase` - Pull changes and rebase instead of merge
  
  **Stash Operations:**
  - `git stash` - Temporarily save changes
  - `git stash pop` - Restore and remove latest stash
  - `git stash list` - List all stashes
  - `git stash drop` - Delete latest stash
  - `git stash clear` - Delete all stashes
  
  **Tagging:**
  - `git tag <name>` - Create lightweight tag
  - `git tag -a <name> -m "message"` - Create annotated tag
  - `git tag -d <name>` - Delete tag
  
  **Conflict Resolution & Recovery:**
  - `git status` - See which files have conflicts during merge/rebase
  - `git add <file>` - Mark conflict as resolved after manual edit
  - `git merge --abort` - Cancel merge and return to pre-merge state
  - `git reflog` - View reference log (recover lost commits)
  - `git reset --hard HEAD@{n}` - Reset to specific reflog entry
  
### **6**: Package managers and dependencies
  
  **🎯 Learning Objectives:** Understand how modern software uses external libraries and how package managers help organize code dependencies.
  
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
  - **JavaScript**: npm (Node Package Manager), yarn, pnpm
  - **Python**: pip (Pip Installs Packages), conda, pipenv
  - **Ruby**: gem, bundler
  - **PHP**: Composer
  - **Java**: Maven, Gradle
  - **C#/.NET**: NuGet
  - **Go**: go mod
  - **Rust**: Cargo
  - **Swift**: Swift Package Manager
  - **C/C++**: vcpkg, Conan
  
  **How Package Managers Work:**
  
  **1. Package Repositories:**
  - **npm Registry**: Over 2 million JavaScript packages
  - **PyPI**: Python Package Index with 400,000+ packages  
  - **RubyGems**: Central repository for Ruby libraries
  - **Maven Central**: Java and JVM language packages
  - **NuGet Gallery**: .NET ecosystem packages
  
  **2. Dependency Resolution:**
  - Package manager reads your dependency file (package.json, requirements.txt, etc.)
  - Downloads requested packages and their dependencies
  - Resolves version conflicts automatically
  - Creates lock file for reproducible builds
  
  **3. Installation Process:**
  ```
  Read dependency file → Resolve versions → Download packages → Install locally
  ```
  
  **Dependency File Examples:**
  
  **JavaScript (package.json):**
  ```json
  {
    "name": "my-web-app",
    "version": "1.0.0",
    "dependencies": {
      "react": "^18.2.0",
      "express": "~4.18.2",
      "lodash": "4.17.21"
    },
    "devDependencies": {
      "webpack": "^5.75.0",
      "jest": "^29.3.0"
    },
    "scripts": {
      "start": "node server.js",
      "test": "jest",
      "build": "webpack"
    }
  }
  ```
  
  **Python (requirements.txt):**
  ```
  Django>=4.1.0,<5.0.0
  requests==2.28.1
  numpy>=1.23.0
  pandas~=1.5.0
  flask
  ```
  
  **Semantic Versioning Explained:**
  
  **Version Format: MAJOR.MINOR.PATCH (e.g., 2.1.3)**
  
  - **MAJOR** (2): Breaking changes - incompatible API changes
  - **MINOR** (1): New features - backward compatible functionality  
  - **PATCH** (3): Bug fixes - backward compatible fixes
  
  **Version Ranges:**
  - `^2.1.3` - Compatible with 2.1.3, allows 2.x.x (not 3.0.0)
  - `~2.1.3` - Compatible with 2.1.3, allows 2.1.x (not 2.2.0)
  - `2.1.3` - Exact version only
  - `>=2.1.0` - Version 2.1.0 or higher
  - `*` or `latest` - Any version (not recommended for production)
  
  **Dependency Types:**
  
  **Production Dependencies:**
  - Required for your application to run in production
  - Examples: web frameworks, databases, utility libraries
  - Installed with: `npm install package-name`
  
  **Development Dependencies:**
  - Only needed during development (testing, building, linting)
  - Examples: test frameworks, build tools, code formatters
  - Installed with: `npm install --save-dev package-name`
  
  **Peer Dependencies:**
  - Expected to be installed by the consuming application
  - Common in plugins and extensions
  - Prevents duplicate installations of large libraries
  
  **Lock Files (Ensuring Reproducibility):**
  - **package-lock.json** (npm): Exact versions of all dependencies
  - **yarn.lock** (Yarn): Yarn's version of lock file
  - **Pipfile.lock** (Python): Pipenv's lock file
  - **Gemfile.lock** (Ruby): Bundler's lock file
  
  **Security Considerations:**
  
  **Dependency Vulnerabilities:**
  - Packages can have security flaws
  - Use `npm audit` or `pip-audit` to check vulnerabilities
  - Keep dependencies updated regularly
  - Use tools like Dependabot for automated updates
  
  **Supply Chain Attacks:**
  - Malicious code injected into popular packages
  - Always review package reputation and maintainers
  - Use package lock files to prevent unauthorized updates
  - Consider using private registries for sensitive projects
  
  **Best Practices:**
  
  **Version Management:**
  - Pin exact versions for production applications
  - Use semantic versioning ranges for libraries
  - Regularly update dependencies for security patches
  - Test thoroughly after dependency updates
  
  **Dependency Hygiene:**
  - Regularly audit and remove unused dependencies
  - Prefer smaller, focused packages over large ones
  - Check package download statistics and community support
  - Read package documentation and changelogs
  
  **Popular Packages by Category:**
  
  **JavaScript:**
  - **Web Frameworks**: React, Vue, Express, Fastify
  - **Utilities**: lodash, moment, axios, uuid
  - **Testing**: Jest, Mocha, Cypress
  - **Build Tools**: Webpack, Vite, Parcel
  
  **Python:**
  - **Web Frameworks**: Django, Flask, FastAPI
  - **Data Science**: NumPy, Pandas, Matplotlib
  - **HTTP Requests**: requests, httpx
  - **Testing**: pytest, unittest
  
  **Java:**
  - **Web Frameworks**: Spring Boot, Spring MVC, Struts, Vaadin
  - **HTTP Clients**: Apache HttpClient, OkHttp, Retrofit
  - **JSON Processing**: Jackson, Gson, JSON-B
  - **Database**: Hibernate, MyBatis, JPA, JDBC
  - **Testing**: JUnit, TestNG, Mockito, AssertJ
  - **Logging**: Log4j, SLF4J, Logback
  - **Build Tools**: Maven, Gradle, Ant
  - **Utilities**: Apache Commons, Guava, Lombok
  
  **Package Manager Commands:**
  
  **npm (JavaScript):**
  ```bash
  npm init                    # Initialize new project
  npm install package-name    # Install package
  npm install -g package-name # Install globally
  npm uninstall package-name  # Remove package
  npm update                  # Update all packages
  npm list                    # Show installed packages
  npm audit                   # Check for vulnerabilities
  ```
  
  **pip (Python):**
  ```bash
  pip install package-name    # Install package
  pip install -r requirements.txt  # Install from file
  pip uninstall package-name  # Remove package
  pip list                    # Show installed packages
  pip freeze > requirements.txt    # Export dependencies
  pip show package-name       # Show package info
  ```
  
  **Maven (Java):**
  ```bash
  mvn archetype:generate      # Create new project
  mvn compile                 # Compile source code
  mvn test                    # Run tests
  mvn package                 # Create JAR/WAR file
  mvn install                 # Install to local repository
  mvn clean                   # Clean target directory
  mvn dependency:tree         # Show dependency tree
  ```
  
  **Gradle (Java/Kotlin/Groovy):**
  ```bash
  gradle init                 # Initialize new project
  gradle build                # Build project
  gradle test                 # Run tests
  gradle jar                  # Create JAR file
  gradle dependencies         # Show dependencies
  gradle clean                # Clean build directory
  gradle bootRun              # Run Spring Boot application
  ```
  
  **Common Issues & Solutions:**
  
  **Version Conflicts:**
  - Different packages require incompatible versions of the same dependency
  - Solution: Use dependency resolution tools or find alternative packages
  
  **Missing Dependencies:**
  - Package doesn't declare all its dependencies properly
  - Solution: Install missing dependencies manually
  
  **Platform Compatibility:**
  - Package works on one OS but not another
  - Solution: Look for cross-platform alternatives or use containers
  
  **Large Bundle Sizes:**
  - Too many dependencies make application slow to load
  - Solution: Use tree-shaking, code splitting, or lighter alternatives
  
### **7**: Review and practice
  
  **🎯 Learning Objectives:** Consolidate your learning from Week 1 and set up a complete development environment ready for Week 2.

## Week 2: Internet Infrastructure and Protocols

### **8**: How the internet works

**🎯 Learning Objectives:** Understand the fundamental infrastructure that makes global internet communication possible.

**The Internet Infrastructure:**

**Physical Layer:**
- **Undersea Cables**: 99% of international internet traffic travels through fiber optic cables on ocean floors
- **Fiber Optic Networks**: Light pulses through glass fibers carrying data at near light speed
- **Data Centers**: Massive facilities housing thousands of servers worldwide
- **Cell Towers**: Wireless internet access points for mobile devices

**Internet Service Providers (ISPs):**
- **Tier 1 ISPs**: Global networks that own international infrastructure (AT&T, Verizon, NTT)
- **Tier 2 ISPs**: Regional providers that buy access from Tier 1 providers
- **Tier 3 ISPs**: Local providers serving end users (your home internet)

**Internet Exchange Points (IXPs):**
- Physical locations where different ISPs connect and exchange traffic
- Reduce latency by creating shorter paths between networks
- Major IXPs: DE-CIX (Frankfurt), AMS-IX (Amsterdam), LINX (London)

**Routers and Routing:**
- **Routers**: Devices that direct internet traffic along optimal paths
- **Routing Tables**: Databases containing information about network paths
- **BGP Protocol**: Border Gateway Protocol determines how data travels between networks
- **Autonomous Systems**: Independent networks with their own routing policies

**Internet vs World Wide Web:**

**The Internet (Infrastructure):**
- Global network of interconnected computers
- Physical hardware: cables, routers, servers, data centers
- Protocols: TCP/IP, HTTP, SMTP, FTP
- Services: Web, email, file transfer, video streaming

**The World Wide Web (Service):**
- Information system running on the internet
- Web pages connected by hyperlinks
- Accessed through web browsers
- Uses HTTP/HTTPS protocol
- Created by Tim Berners-Lee in 1989

**Think of it this way:**
- Internet = Highway system (roads, bridges, signs)
- World Wide Web = Cars and trucks using those highways

**IP Addresses and Address Space:**

**IPv4 Addresses:**
- 32-bit addresses (4 bytes)
- Format: 192.168.1.1 (four numbers 0-255)
- Total possible addresses: ~4.3 billion
- Problem: Running out due to internet growth

**IPv6 Addresses:**
- 128-bit addresses (16 bytes)
- Format: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- Total possible addresses: 340 undecillion (practically unlimited)
- Gradual adoption worldwide

**Private vs Public IP Addresses:**

**Private IP Ranges** (not routable on internet):
- 10.0.0.0 - 10.255.255.255 (Class A)
- 172.16.0.0 - 172.31.255.255 (Class B)
- 192.168.0.0 - 192.168.255.255 (Class C)

**Public IP Addresses:**
- Assigned by Internet Assigned Numbers Authority (IANA)
- Must be unique globally
- Required for direct internet communication

**Network Address Translation (NAT):**
- Allows multiple devices to share one public IP address
- Your router translates private IPs to public IP
- Enables home networks with limited IPv4 addresses

**Data Transmission Methods:**

**Packet Switching:**
- Data broken into small packets
- Each packet routed independently
- Packets reassembled at destination
- More efficient than circuit switching

**TCP/IP Protocol Stack:**
1. **Application Layer**: HTTP, HTTPS, SMTP, FTP
2. **Transport Layer**: TCP (reliable) / UDP (fast)
3. **Network Layer**: IP (routing between networks)
4. **Link Layer**: Ethernet, WiFi (local network)

**Internet Governance:**
- **ICANN**: Manages domain names and IP addresses
- **IETF**: Develops internet standards and protocols
- **W3C**: Web standards organization
- **Regional Internet Registries**: Distribute IP addresses by region

**Internet Performance Factors:**
- **Latency**: Time for data to travel from source to destination
- **Bandwidth**: Amount of data that can be transmitted per second
- **Jitter**: Variation in latency (affects real-time applications)
- **Packet Loss**: Percentage of data packets that don't reach destination

### **9**: Domain Name System (DNS)

**🎯 Learning Objectives:** Master how domain names are converted to IP addresses and understand the DNS infrastructure that makes the internet user-friendly.

**What is DNS?**
- **Domain Name System**: Internet's phonebook that translates human-readable domain names to IP addresses
- **Purpose**: Makes internet more user-friendly (remember google.com instead of 172.217.164.142)
- **Distributed System**: No single point of failure, replicated worldwide

**Domain Name Hierarchy:**

**Top-Level Domains (TLDs):**
- **Generic TLDs**: .com, .org, .net, .edu, .gov, .mil
- **Country Code TLDs**: .uk, .ca, .de, .jp, .au
- **New TLDs**: .app, .dev, .blog, .shop, .tech

**Domain Structure:**
```
subdomain.second-level-domain.top-level-domain
www.      example.                com
```

**DNS Record Types:**

**Essential Record Types:**
- **A Record**: Maps domain to IPv4 address (example.com → 192.0.2.1)
- **AAAA Record**: Maps domain to IPv6 address
- **CNAME Record**: Maps alias to canonical domain name (www.example.com → example.com)
- **MX Record**: Specifies mail servers for domain
- **NS Record**: Identifies authoritative name servers
- **TXT Record**: Stores text information (SPF, DKIM, domain verification)

**Advanced Record Types:**
- **PTR Record**: Reverse DNS lookup (IP to domain)
- **SRV Record**: Service location (used for specific services)
- **CAA Record**: Certificate Authority Authorization
- **SOA Record**: Start of Authority (domain metadata)

**DNS Resolution Process (Step-by-Step):**

**1. User Types URL:** www.example.com
**2. Browser Cache Check:** Is IP address already stored?
**3. Operating System Cache:** Check OS-level DNS cache
**4. Router Cache:** Check local network router cache
**5. ISP Resolver:** Query Internet Service Provider's DNS server
**6. Root Name Server:** If not cached, query one of 13 root servers worldwide
**7. TLD Server:** Root server directs to .com TLD servers
**8. Authoritative Server:** TLD server points to example.com's name servers
**9. Final Resolution:** Authoritative server returns IP address
**10. Response Chain:** IP address travels back through all levels
**11. Browser Connects:** Finally connects to web server using IP address

**DNS Server Types:**

**Recursive Resolvers:**
- Perform full DNS lookups on behalf of clients
- Cache results to improve performance
- Examples: Google DNS (8.8.8.8), Cloudflare DNS (1.1.1.1)

**Authoritative Servers:**
- Hold actual DNS records for domains
- Provide definitive answers for domains they manage
- No caching, always return current records

**Root Name Servers:**
- 13 sets of servers worldwide (A through M)
- Highest level in DNS hierarchy
- Managed by different organizations globally

**DNS Caching:**

**Browser Cache:**
- Stores DNS responses for short periods (minutes)
- Improves page load speed for repeat visits
- Can be cleared manually

**Operating System Cache:**
- System-level DNS caching
- TTL (Time To Live) controls cache duration
- Cleared when computer restarts

**ISP Resolver Cache:**
- Internet provider caches popular domains
- Reduces load on upstream DNS servers
- Shared among all ISP customers

**DNS Propagation:**

**What is Propagation?**
- Time required for DNS changes to spread globally
- Not all servers update simultaneously
- Can take 24-48 hours for full propagation

**Factors Affecting Propagation:**
- **TTL Values**: Lower TTL = faster propagation but more queries
- **Server Locations**: Geographic distribution affects speed
- **Caching Policies**: Different servers have different update schedules

**TTL (Time To Live):**
- Specifies how long DNS records should be cached
- Measured in seconds (3600 = 1 hour, 86400 = 24 hours)
- Lower TTL = more flexibility, higher server load
- Higher TTL = less server load, slower changes

**DNS Security:**

**Common DNS Attacks:**
- **DNS Spoofing**: Fake responses redirect users to malicious sites
- **DNS Cache Poisoning**: Corrupt cached DNS data
- **DNS Amplification**: Use DNS servers to amplify DDoS attacks

**DNS Security Extensions (DNSSEC):**
- Adds cryptographic signatures to DNS records
- Prevents tampering with DNS responses
- Ensures authenticity of DNS data

**Popular Public DNS Servers:**

**Google Public DNS:**
- Primary: 8.8.8.8
- Secondary: 8.8.4.4
- IPv6: 2001:4860:4860::8888

**Cloudflare DNS:**
- Primary: 1.1.1.1
- Secondary: 1.0.0.1
- Focus on privacy and speed

**Quad9 DNS:**
- Primary: 9.9.9.9
- Blocks malicious domains
- Security-focused

**DNS Tools and Commands:**

**Command Line Tools:**
```bash
# Look up IP address
nslookup google.com

# Detailed DNS information
dig google.com

# Reverse DNS lookup
nslookup 8.8.8.8

# Trace DNS resolution path
dig +trace google.com

# Check specific record type
dig google.com MX
```

**DNS Management:**
- **Domain Registrars**: Where you buy domain names (GoDaddy, Namecheap, etc.)
- **DNS Hosting**: Where DNS records are stored (may be same or different from registrar)
- **DNS Zone Files**: Text files containing all DNS records for a domain

### **10**: HTTP and HTTPS protocols

**🎯 Learning Objectives:** Understand how web browsers and servers communicate, including request/response cycles, methods, status codes, and security.

**HTTP (HyperText Transfer Protocol):**
- **Application Layer Protocol**: Runs on top of TCP/IP
- **Stateless**: Each request is independent, no memory of previous requests
- **Client-Server Model**: Browser (client) requests, server responds
- **Port 80**: Default port for HTTP traffic
- **Plain Text**: Data transmitted without encryption (security risk)

**HTTPS (HTTP Secure):**
- **HTTP + SSL/TLS Encryption**: Secure version of HTTP
- **Port 443**: Default port for HTTPS traffic
- **Data Encryption**: All communication encrypted between client and server
- **Authentication**: Verify server identity with SSL certificates
- **Data Integrity**: Detect if data was tampered with during transmission

**HTTP Request Structure:**

**Request Line:**
```
GET /path/to/resource HTTP/1.1
[Method] [Path] [HTTP Version]
```

**Request Headers:**
```
Host: www.example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
Accept: text/html,application/xhtml+xml
Accept-Language: en-US,en;q=0.9
Cookie: session_id=abc123
```

**Request Body (for POST, PUT):**
```json
{
  "username": "john",
  "password": "secret123"
}
```

**HTTP Methods (Verbs):**

**Safe Methods (Read-Only):**
- **GET**: Retrieve data from server (most common)
- **HEAD**: Get headers only (no body)
- **OPTIONS**: Get allowed methods for resource

**Unsafe Methods (Modify Data):**
- **POST**: Create new resource or submit data
- **PUT**: Create or completely replace resource
- **PATCH**: Partially update existing resource
- **DELETE**: Remove resource from server

**Method Usage Examples:**
```
GET /users/123          # Get user with ID 123
POST /users             # Create new user
PUT /users/123          # Update/replace user 123
PATCH /users/123        # Partially update user 123
DELETE /users/123       # Delete user 123
```

**HTTP Response Structure:**

**Status Line:**
```
HTTP/1.1 200 OK
[HTTP Version] [Status Code] [Reason Phrase]
```

**Response Headers:**
```
Content-Type: text/html; charset=UTF-8
Content-Length: 1234
Set-Cookie: session_id=xyz789; HttpOnly
Cache-Control: max-age=3600
```

**Response Body:**
```html
<!DOCTYPE html>
<html>
<body>
  <h1>Welcome to Example.com</h1>
</body>
</html>
```

**HTTP Status Code Categories:**

**1xx Informational (Rare):**
- **100 Continue**: Server ready for request body
- **101 Switching Protocols**: Upgrading to different protocol

**2xx Success:**
- **200 OK**: Request successful
- **201 Created**: Resource created successfully
- **202 Accepted**: Request accepted for processing
- **204 No Content**: Success but no content to return

**3xx Redirection:**
- **301 Moved Permanently**: Resource permanently moved
- **302 Found**: Resource temporarily moved
- **304 Not Modified**: Use cached version
- **307 Temporary Redirect**: Temporary redirect, method unchanged

**4xx Client Errors:**
- **400 Bad Request**: Malformed request
- **401 Unauthorized**: Authentication required
- **403 Forbidden**: Access denied
- **404 Not Found**: Resource doesn't exist
- **405 Method Not Allowed**: HTTP method not supported
- **429 Too Many Requests**: Rate limiting in effect

**5xx Server Errors:**
- **500 Internal Server Error**: Generic server error
- **502 Bad Gateway**: Invalid response from upstream server
- **503 Service Unavailable**: Server temporarily unavailable
- **504 Gateway Timeout**: Timeout from upstream server

**HTTP Headers:**

**Request Headers:**
- **Host**: Target server (required in HTTP/1.1)
- **User-Agent**: Client information (browser, OS)
- **Accept**: Content types client can handle
- **Authorization**: Authentication credentials
- **Cookie**: Client-side stored data
- **Referer**: URL of referring page
- **If-Modified-Since**: Conditional request header

**Response Headers:**
- **Content-Type**: MIME type of response body
- **Content-Length**: Size of response body in bytes
- **Set-Cookie**: Send cookie to client
- **Cache-Control**: Caching directives
- **Location**: URL for redirects
- **Server**: Server software information
- **Last-Modified**: When resource was last changed

**HTTPS and SSL/TLS:**

**SSL/TLS Handshake Process:**
1. **Client Hello**: Browser sends supported encryption methods
2. **Server Hello**: Server chooses encryption method
3. **Certificate Exchange**: Server sends SSL certificate
4. **Certificate Verification**: Browser verifies certificate authenticity
5. **Key Exchange**: Generate session encryption keys
6. **Secure Communication**: All data now encrypted

**SSL Certificate:**
- **Digital Certificate**: Proves server identity
- **Certificate Authority (CA)**: Trusted organization that issues certificates
- **Certificate Chain**: Root CA → Intermediate CA → Server Certificate
- **Expiration Date**: Certificates have limited validity period

**HTTPS Benefits:**
- **Encryption**: Data can't be read if intercepted
- **Authentication**: Verify you're connected to correct server
- **Integrity**: Detect data tampering
- **SEO Boost**: Search engines prefer HTTPS sites
- **Browser Trust**: Modern browsers warn about non-HTTPS sites

**HTTP Versions:**

**HTTP/1.1** (Most Common):
- **Persistent Connections**: Reuse TCP connections
- **Chunked Transfer Encoding**: Send data in chunks
- **Host Header**: Support multiple domains on one server
- **Request Pipelining**: Send multiple requests without waiting

**HTTP/2** (Modern):
- **Binary Protocol**: More efficient than text-based HTTP/1.1
- **Multiplexing**: Multiple requests in parallel over one connection
- **Header Compression**: Reduce overhead
- **Server Push**: Server can send resources before client requests

**HTTP/3** (Latest):
- **QUIC Protocol**: Runs over UDP instead of TCP
- **Faster Connection Setup**: Reduces latency
- **Better Reliability**: Handles packet loss more gracefully

**Common HTTP Patterns:**

**RESTful APIs:**
```
GET /api/users          # List all users
GET /api/users/123      # Get specific user
POST /api/users         # Create new user
PUT /api/users/123      # Update user
DELETE /api/users/123   # Delete user
```

**Authentication Methods:**
- **Basic Auth**: Username/password in headers (insecure over HTTP)
- **Bearer Token**: JWT or OAuth tokens in Authorization header
- **Cookie-based**: Session ID stored in cookies
- **API Keys**: Secret keys for API access

**Content Types (MIME Types):**
- **text/html**: HTML web pages
- **application/json**: JSON data
- **application/xml**: XML data
- **image/jpeg**: JPEG images
- **text/css**: CSS stylesheets
- **application/javascript**: JavaScript files

**HTTP Caching:**

**Cache-Control Headers:**
- **max-age=3600**: Cache for 1 hour
- **no-cache**: Validate with server before using cached version
- **no-store**: Never cache this content
- **public**: Can be cached by any cache (CDN, proxy)
- **private**: Only cache on user's browser

**ETag (Entity Tag):**
- Unique identifier for resource version
- Client sends If-None-Match header
- Server returns 304 Not Modified if unchanged

### **11**: Web servers and hosting
  - What is a web server?
  - Static vs dynamic hosting
  - Shared, VPS, and dedicated hosting

### **12**: APIs and data exchange
  - What is an API?
  - REST API basics
  - JSON and XML data formats

### **13**: Databases fundamentals
  - What are databases?
  - SQL vs NoSQL overview
  - How web apps store data

### **14**: Review and exploration
  - Use browser dev tools to examine HTTP requests
  - Look up a website's DNS records
  - Practice understanding URL structure

## Week 3: Web Technologies and Browsers
### **15**: HTML fundamentals
  - Document structure and semantic elements
  - How browsers parse HTML
  - HTML validation and best practices

### **16**: CSS fundamentals
  - How styles are applied to HTML
  - CSS specificity and cascade
  - Browser default styles

### **17**: JavaScript basics
  - What JavaScript does in browsers
  - Client-side vs server-side scripting
  - JavaScript execution in browsers

### **18**: Web standards and compatibility
  - W3C and web standards
  - Browser differences and compatibility
  - Progressive enhancement

### **19**: Responsive web design
  - Mobile vs desktop web
  - Viewport and media queries
  - Touch vs mouse interaction

### **20**: Web accessibility
  - What is web accessibility?
  - Screen readers and assistive technology
  - WCAG guidelines basics

### **21**: Review and hands-on
  - Create a simple HTML page
  - Test it in different browsers
  - Use accessibility tools

### Week 4: Security, Performance, and Modern Web
### **22**: Web security basics
  - HTTPS and SSL/TLS certificates
  - Common security vulnerabilities
  - Safe browsing practices

### **23**: Web performance
  - Why website speed matters
  - Browser caching and optimization
  - Image optimization and compression

### **24**: Modern web development
  - Single Page Applications (SPAs)
  - Progressive Web Apps (PWAs)
  - Mobile-first development

### **25**: Content Delivery Networks
  - What is a CDN?
  - How CDNs improve performance
  - Popular CDN services

### **26**: Monitoring and analytics
  - Website analytics basics
  - Performance monitoring tools
  - Error tracking and debugging

### **27**: Future of the web
  - Web3 and blockchain concepts
  - AI integration in web development
  - Emerging web technologies

### **28**: Final review and next steps
  - Review key concepts
  - Assess your learning
  - Plan your next learning phase

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
