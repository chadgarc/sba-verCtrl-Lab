The steps I followed to create and manage branches were the following.
First, I created my workspace and initialized my local repository using:

git init

Then, on my GitHub account, I created a new remote repository. Once I had the URL, I connected my local repo to GitHub using:

git remote add origin [repository-url]

Since I already had the main branch, I created the feature/header and feature/footer branches using:

git switch -c [branch-name]

From there, I worked on each branch separately. Whenever I needed to switch between feature/header, feature/footer, or main, I used:

git switch [branch]

Before switching branches, I always made sure to save my work by running:

git add .

git commit -m "message"

I intentionally made changes to the same lines in both the header and footer sections to create merge conflicts. When merging those branches into main, Git detected the conflicts. I resolved them manually by editing the files, removing the parts I didn’t need, and keeping the correct version.
VS Code helped by showing the conflict markers, and I chose which lines to keep. After resolving the conflicts, I used:

git add .
git commit

To finalize the merge, and then pushed the changes to GitHub.

Even though we were told that Part 4 was optional, I still practiced creating Pull Requests on my own repository. From what I understand, Pull Requests are used to collaborate on code changes. The owner or authorized collaborators of the repository can review, approve, or reject the changes. This process helps maintain control, code quality, and ensures that no one modifies the main codebase without proper review or permission.
