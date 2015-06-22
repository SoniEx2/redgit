# redgit
reddit:// URL support for Git

## Why reddit?
Reddit has all a git hosting service would ever need, with some minor caveats:

Think of a subreddit as a collection of repos.

Think of each post as a repo. A collection of:
- Per-user branches. Which in turn are a collection of:
    - Commits. Which can have:
        - Tags.
        - Comments.
        - Mentions. (That is, you can mention users in commit messages.)
- Issues.
- Pull Requests.

Issues, pull requests and comments cannot be "watched".

### What does "per-user branches" mean?
Instead of having a user/repo/branch hierarchy, we have a repo/user/branch hierarchy.
Forking a repo is as simple as making a new reddit comment on the repo (main post) but under a different reddit username.

### How does cloning work?
To clone, you clone reddit://subreddit/post/user (which follows the subreddit/repo/user hierarchy, instead of the user/repo hierarchy you're used to.)
