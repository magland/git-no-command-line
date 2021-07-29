# Log in to GitHub from within VSCode

GitHub authentication is now tightly integrated into VSCode. This is especially good news considering that very soon, [GitHub will no longer allow password authentication](https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/) for git operations. That means that the traditional method of interacting with a remote GitHub repo will be a thing of the past, and we will all need to migrate to a token-based system. Let's let VSCode can handle all those details for us!

![Log in screenshot](https://user-images.githubusercontent.com/3679296/127549378-ac072338-5039-428c-b40f-570989865882.png)

* Click the *Accounts* button in the lower-left part of the VSCode window and click to Sign in with GitHub (note that you must have the GitHub Pull Requests and Issues extension installed).

* You will be redirected to a `vscode-auth.github.com` site where you will be asked to continue with authorization.

* The browser will then ask you to click to run a command on your local machine which will open VSCode and give the following prompt:

![allow extension screenshot](https://user-images.githubusercontent.com/3679296/127549941-d405618b-6a59-4219-a7de-256fc55dcbb5.png)

* After clicking "Open" you should be all set. VSCode is now authorized to communicate with GitHub on your behalf.