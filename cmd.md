cargo build

cargo test

cargo clippy --all-targets --all-features

git add .; git commit -m "init"; git push -u origin master


Explanation for X api application;

For the following app;

An X bot that posts updates to an X_account with information from GitHub API.

use the GitHub API to:

Detect when a new contributor makes their first commit to the master branch of the X_account's github repository.

Detect when a new release of the delta repository is published.
You will use the X API to:

Post a message to the X_account whenever a new contributor makes their first commit to the master branch of the X_account's repository.

Post a message to the X_account whenever a new release of the X_account repository is published.

We need (for now) two types of posts:
1. For new contributors:
X_account got a new contributor [Contributor Name]!

Details: [Commit message]  

Link: [Commit link]
2. For new releases:
New release ([Version Number]) of Application out! 🎉
  
Link to release notes: [Release link]
Implement these features in the bot, ensuring the messages are posted automatically whenever these events occur.