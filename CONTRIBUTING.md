<!---
title: Contributing
intro: Read [ IBM's Code of Conduct](https://github.com/IBM/anz-developer-advocacy-code-of-conduct) to keep our community approachable and respectable.
permissions: '{% data reusables.enterprise-accounts.emu-permission-fork %}'
topics:
  - Pull requests
  - Forks
  - GitHub
  - Open Source
--->

![hero](https://user-images.githubusercontent.com/3901764/57545698-ce5f2380-7320-11e9-8682-903df232d7b0.png)

# Contribuiting 

🎉 First off, thanks for taking the time to contribute! 🎉

In this guide you will get an overview of the contribution workflow from opening an issue, creating a PR, reviewing, and merging the PR. Read [ IBM's Code of Conduct](https://github.com/IBM/anz-developer-advocacy-code-of-conduct) to keep our community approachable and respectable.



_Optional_: [How to Contribute to an Open Source Project on GitHub](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)

## Forking a repository

This tutorial uses [the Spoon-Knife project](https://github.com/octocat/Spoon-Knife), a test repository that's hosted on GitHub.com that lets you test the fork and pull request workflow.

1. Navigate to the `Spoon-Knife` project at https://github.com/octocat/Spoon-Knife.
2. Click **Fork**.
![Fork button](https://raw.githubusercontent.com/github/docs/main/assets/images/help/repository/fork_button.png)
3. Select an owner for the forked repository.
   ![Create a new fork page with owner dropdown emphasized](https://github.com/github/docs/blob/main/assets/images/help/repository/fork-choose-owner.png?raw=true)
4. By default, forks are named the same as their parent repositories. You can change the name of the fork to distinguish it further. 
   ![Create a new fork page with repository name field emphasized](https://github.com/github/docs/blob/main/assets/images/help/repository/fork-choose-repo-name.png?raw=true)
5. Optionally, add a description of your fork.
   ![Create a new fork page with description field emphasized](https://github.com/github/docs/blob/main/assets/images/help/repository/fork-description.png?raw=true)
6. Choose whether to copy only the default branch or all branches to the new fork. For many forking scenarios, such as contributing to open-source projects, you only need to copy the default branch. By default, only the default branch is copied.
   ![Option to copy only the default branch](https://github.com/github/docs/blob/main/assets/images/help/repository/copy-default-branch-only.png?raw=true)
7. Click **Create fork**.
   ![Emphasized create fork button](https://github.com/github/docs/blob/main/assets/images/help/repository/fork-create-button.png?raw=true)

## Cloning a fork

You've successfully forked the Spoon-Knife repository, but so far, it only exists on GitHub. To be able to work on the project, you will need to clone it to your computer.

You can clone your fork with the command line, GitHub CLI, or GitHub Desktop.

1. On GitHub, navigate to your fork of the Spoon-Knife repository.

2. Click **Code**.

    ![Emphasized create fork button]( https://github.com/github/docs/blob/main/assets/images/help/repository/code-button.png?raw=true)

3. To clone the repository using HTTPS, under "HTTPS", click on the copy button.
   ![Emphasized code button]( https://docs.github.com/assets/cb-33207/images/help/repository/https-url-clone-cli.png)

4. Open Git bash.

    ![terminal]( https://1v5ymx3zt3y73fq5gy23rtnc-wpengine.netdna-ssl.com/wp-content/uploads/2021/07/git-bash-open-screen.png)
5. Type `git clone`, and then paste the URL you copied earlier. It will look like this, with your username instead of `YOUR-USERNAME`:
  ```shell
  $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
  ```

6. Press **Enter**. Your local clone will be created.
  ```shell
  $ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
  > remote: Counting objects: 10, done.
  > remote: Compressing objects: 100% (8/8), done.
  > remove: Total 10 (delta 1), reused 10 (delta 1)
  > Unpacking objects: 100% (10/10), done.
  ```

To create a clone of your fork, use the `--clone` flag.

```shell
gh repo fork <em>repository</em> --clone=true
```

## Making and pushing changes

Go ahead and make a few changes to the project using your favorite text editor, like [Visual Studio Code](https://code.visualstudio.com). You could, for example, change the text in `index.html` to add your GitHub username.

When you're ready to submit your changes, stage and commit your changes. `git add .` tells Git that you want to include all of your changes in the next commit. `git commit` takes a snapshot of those changes.


```shell
git add .
git commit -m "a short description of the change"
```

```shell
git add .
git commit -m "a short description of the change"
```

When you stage and commit files, you essentially tell Git, "Okay, take a snapshot of my changes!" You can continue to make more changes, and take more commit snapshots.

Right now, your changes only exist locally. When you're ready to push your changes up to GitHub, push your changes to the remote.

## Making a pull request

At last, you're ready to propose changes into the main project! This is the final step in producing a fork of someone else's project, and arguably the most important. If you've made a change that you feel would benefit the community as a whole, you should definitely consider contributing back.

To do so, head on over to the repository on where your project lives. For this example, it would be at `https://www.github.com/<your_username>/Spoon-Knife`. You'll see a banner indicating that your branch is one commit ahead of `octocat:main`. Click **Contribute** and then **Open a pull request**. will bring you to a page that shows the differences between your fork and the `octocat/Spoon-Knife` repository. Click **Create pull request**.

GitHub will bring you to a page where you can enter a title and a description of your changes. It's important to provide as much useful information and a rationale for why you're making this pull request in the first place. The project owner needs to be able to determine whether your change is as useful to everyone as you think it is. Finally, click **Create pull request**.

## Managing feedback

Pull Requests are an area for discussion. In this case, the Octocat is very busy, and probably won't merge your changes. For other projects, don't be offended if the project owner rejects your pull request, or asks for more information on why it's been made. It may even be that the project owner chooses not to merge your pull request, and that's totally okay. Your copy will exist in infamy on the Internet. And who knows--maybe someone you've never met will find your changes much more valuable than the original project.

###### tags: `GitHub`, `Basics`

