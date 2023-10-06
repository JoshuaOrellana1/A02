# A02
Git and GitHub:

Imagine you're working on a text document in a text editor. You type "Hello World" and save the file. This saved state is like a "milestone" on your computer because you can reopen it later. If you make changes and save again, you overwrite the previous milestone. Git operates similarly but allows you to save these milestones, or versions, of your files over time.

When you type git commit -am "By typing this command I am saving a collection of saved files," you're essentially saving a snapshot of your work in Git. This is great because it lets you go back to older versions of your files without starting from scratch, which is known as "source control."

Now, what if you could save these milestones not just on your computer but in the cloud? This is where GitHub comes in. GitHub is like a cloud-based Git system with social networking features around code. You can push your local Git repository to GitHub using git push origin master, making it available to others and preserving the complete history of your project.

To set up a project on GitHub:

Create a new repository on GitHub (don't check "Initialize this project with a README" if you already have one).
Determine the SSH clone URL, typically something like git@github.com:USERNAME/PROJECT.git.
Add this remote repository to your local Git using git remote add origin {{the link you copied}}.
If you want to clone an existing repository:

Determine the SSH clone URL.
Use git clone {{the link you copied}} to clone the repository and add a remote named "origin."

With a Git repository set up, remember these principles:

Never commit directly to master or develop. Instead, create feature branches from develop for specific tasks.
Make changes, stage them with git add, and commit with git commit -am "Your commit message".
Merge your feature branches back into develop with git checkout develop and git merge --no-ff my-feature-branch.
When releasing a new version, update your master branch, create a tag (e.g., v1.0.0), and push it to GitHub.
These practices help maintain a clean and organized version history for your project.

Glossary

Branch: A separate line of development in Git, allowing multiple features or changes to be worked on simultaneously.

Clone: To make a copy of a remote repository on your local machine for development or collaboration.

Commit: A record of a change in Git, capturing a snapshot of the repository at a specific point in time.

Fetch: To retrieve changes from a remote repository without merging them into your local branch.

Git: A distributed version control system used for tracking changes in source code during software development.

GitHub: A web-based platform for version control and collaboration that uses Git.

Merge: To combine changes from one branch into another, typically used to incorporate new features or bug fixes.

Merge Conflict: Occurs when Git cannot automatically merge changes from different branches, requiring manual resolution.

Push: To upload your local Git commits to a remote repository, making them available to others.

Pull: To retrieve changes from a remote repository and merge them into your local branch.

Remote: A reference to a Git repository on a server, often used for collaborative development.

Repository: A collection of files and version history managed by Git, typically hosted on a platform like GitHub.

References:

GitHub. (n.d.). GitHub: Where the world builds software. GitHub.
JetBrains. (n.d.). WebStorm: The smartest JavaScript IDE. WebStorm.
Pro Git Book. (n.d.). Git Glossary. Git Glossary.
