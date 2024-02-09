# Review Questions

### What is the terminal? What are some synonyms for it?

* The terminal is a command-line-based method of navigating your computer's files and executing certain actions. Most users stick with the GUI (graphical user interface) when modifying files on their computer,
  but using a terminal can allow for more options and capabilities. There are multiple terminals, including PowerShell, Git Bash, and PuTTY. They each have their separate commands that allow for more
  system-specific modifications.
* The terminal that we use is **Git Bash**. It consists of two tools, "Git" and "Bash".
  * **Bash** is the terminal portion of Git Bash. This is where we navigate the computer's files and enter commands to work with our repositories.
    * Some basic commands include: `pwd` (lists your current directory), `cd` (takes you into a directory), and `ls` (lists all contents in a directory).
  * **Git** is the program where Bash is located, referred to as a "version control system" or VCS.
    * Git allows us to make and save changes to commit them onto the GitHub repository.

### What is the prompt?
* When using a terminal, the prompt is where the user can enter commands. When opening your computer's terminal or a program like Git Bash, the prompt will be what shows up.

### What is a directory?
* A directory is where files are kept (essentially another word for folder). You can access and navigate these directories in several ways, including your operating system's file explorer and a terminal.

### What is `cd`?
* `cd` is one of the commands used in the Bash terminal. It stands for "change directory" and allows the user to change their current directory.
  * This command relies on the argument provided. After the initial command, writing a folder name will tell the terminal which folder to enter. ".." returns to the parent directory.

### What is `npm`? What does it stand for? What is it used for?
* "npm" stands for "Node Package Manager". `npm` comes with Node, and installs Node modules that help you write and save code. `npm install` will install modules off the npm package registry, and `npm run dev` opens a
local server where you can see a live preview of your work.

### What file must be present for `npm` to work? (Manifest file)
* `npm` requires a `package.json` file. Sometimes there is also a `package-lock.json` that can interfere with running `npm`.

### How do we add a script to `package.json`?
* We can add scripts by adding another line under the "scripts" portion of `package.json`. The script name is contained in quotes followed by a colon, after which you add the command that is tied to that script. In the video's
  example, this is done as `"kick": "echo 'Hello, Vite!'"`. Once a script is added, you can run them using `npm run`.

### How do we install a package? Why would we want to do this?
* Packages can be installed through the NPMJS website, normally by googling the package you're looking for. Adding extra packages to `package.json` can make your web development experience much more convenient. For example,
  using `modern-normalize` normalizes browser defaults for CSS projects.

### What is Vite?
* Vite helps us with front-end tooling. They have many features, including:
  * Instant Server Start: This opens a realistic web server that gives you a live preview while you're working on your projects.
  * Lightning-Fast HMR: This updates the preview as soon as you make changes in your code.

# Reflections

* Before this class, my experience with terminals and other CLI-based programs was with PowerShell (CIS-178 Administrative Scripting) and Windows's Command Prompt. Using Git Bash to make changes to my programs has definitely
  been a new experience for me, considering my previous classes only required a Blackboard/Brightspace submission and therefore I didn't need to post my work to sites like GitHub.
  
* When using Git Bash, it took me some time to learn some of the Git-specific commands and how to utilize them. It probably wasn't until Week 2 or 3 that I felt I had a good understanding of the commands that we've discussed so far.
  I've enjoyed using `npm install` and `npm run dev` when testing websites as that is **way** more convenient than having to refresh a webpage each time I wanted to view my progress. The only issue that I've experienced with
  using `npm` commands is errors with the `package.json` file. For example, this repository contains my reflections in MarkDown that I've made since the class started. However, I haven't been able to work on these using Git Bash and
  Visual Studio Code because this repository does not have a `package.json` file. I don't know if copying one from another repository would fix the issue, but I'm thinking about giving it a shot after writing this.
  
* I think Vite is a nice tool to have when doing web development, and I'm looking forward to using it for future GitHub projects. It's nice being able to clone repositories and work on them locally before pushing them back to the
  origin without all the extra steps that usually come with it.
  
* This isn't related to the questions, but I like the idea of using the Office Hours idea for class content. My only issue is that when the Screenshare gets desynced it becomes hard to follow what's happening in the video.
