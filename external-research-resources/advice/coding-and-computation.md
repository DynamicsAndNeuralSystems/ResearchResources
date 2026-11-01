---
metaLinks:
  alternates:
    - /broken/spaces/mzd6xx2kCQ8dn7PxnBoD/pages/ksi312Hj54EtO4Pw9nvM
---

# 🖥️ Coding and Computation

### Writing code using version control

You must use version control when you code :relaxed:

**Graphical Interface**

Version control is much easier with a graphical interface than in the command-line. This is the place to start—you can do everything you need, and visually see the whole history of your code base.

* I recommend [GitKraken](https://www.gitkraken.com/), which is free for students.
  * Students get GitKraken Pro free through the [GitHub Student Developer Pack](https://education.github.com/pack); see [GitKraken's student page](https://www.gitkraken.com/student-resources).
* The free (for everyone) [SourceTree](https://www.sourcetreeapp.com) is also really good.
* An alternative is [Github Desktop](https://desktop.github.com).

**Command-line git**

On a server, such as for a compute cluster, you must run git in the command-line.

* Here is a quick [introduction article](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668) to version control using Git.
* Some nice tutorials for this have been written by [Atlassian](https://www.atlassian.com/git/).

#### Basics

* Commit regularly
* Focus on text files, like code, where changes can be stored efficiently. Avoid binary files (datasets, image files, etc.) that will bloat your repository. (Use the `.gitignore` file).

#### GitHub

If you're up and using git locally, GitHub is a free (for education) service that allows you to host your code. Then you can share what you've done so others can help you develop it through collaboration, or can exactly reproduce the steps of your analysis as outlined in your code.

1. Make an [educational account](https://education.github.com/benefits) on GitHub, which provides you with unlimited public and private repositories.
2. The first time you set up git, you should generate an ssh key to bypass having to type your username and password with every push to GitHub. Instructions are [here](https://help.github.com/articles/generating-an-ssh-key/). This means that you should use the ssh (not http) version of the Github repository reference: `git clone git@github.com:benfulcher/TestGitRepository.git`

* It's also very useful to set up git integration with your text editor. I recommend [VS Code](https://code.visualstudio.com/).

**Workflow**

Whenever you start a project that involves coding, be sure to first initialize a repository on Github, clone it to your local machine (as the `ssh` not `https` version), and then regularly commit snapshots of your code.

Whenever you produce an output figure or statistic, you should have a clear way to map back to the state of your code when you produced this (which can be done by committing the code at that point).

Code to reproduce every analysis and figure in your paper should be easy for others to access and use. A good way to do this is to describe all your analyses in a markdown file, like the online-rendered `README.md` file, where you work through the exact steps to reproduce every analysis in your paper, and embed the outputs.

When you're happy with your code, you should version it with a DOI to keep a preserved snapshot that cannot be modified/deleted. It's actually really easy to do this, by linking Zenodo to your Github (and you get a nice DOI logo on your repo!): [instructions here](https://guides.github.com/activities/citable-code/).

If you're really into it, building a Docker container for your project allows full reproduction into the future, regardless of changes to operating systems or software packages. See [Aria's notes](https://docs.google.com/document/d/1Um6sVef3JXVXYfmC5dYaHtGLc5Oi9W7sWSTv6fd8hzc/) and this [Simple Rules paper](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008316).

### Coding better

* Some helpful coding tips (mostly Matlab) are on this [medium blog](https://medium.com/@neuraljojo).
* And >20h of tutorials, including version control by Jeremy Howard, on [YouTube](https://www.youtube.com/playlist?list=PLfYUBJiXbdtSLBPJ1GMx-sQWf6iNhb8mM).
* [**VS Code**](https://code.visualstudio.com) is a full featured and efficient integrated text editor for coding. You should use the [jupyter support](https://code.visualstudio.com/docs/python/jupyter-support-py).

#### Terminals

* On Mac, [iTerm2](https://iterm2.com/) is free and far superior to the in-built terminal app.
* :fire: If you are fancy, you can change to using the [fish shell](https://fishshell.com/), which has lots of cool features.
* :fire: If you want to set up your Mac with lots of cool terminal superpowers, [look no further](https://github.com/ghaiklor/iterm-fish-fisher-osx).

### Working with a cluster

* You should have a nice interactive way of getting data/outputs to/from the server. The best is [Transmit](https://panic.com/transmit/); free alternatives are [Cyberduck](https://cyberduck.io/), or [FileZilla](https://filezilla-project.org/).
* You should set up an [ssh key](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2) for each server you use regularly, to avoid typing in your password every time you connect. If you use git on the server, also add a GitHub ssh key there, as described in the GitHub section above.
* To avoid typing in the full username and servername every time you connect to your server, you set up an [ssh config file](https://nerderati.com/2011/03/17/simplify-your-life-with-an-ssh-config-file/).
* There are also fancy ways of running code (like in Julia) on the cluster via VS Code. E.g., if you set up a VSCode server on a compute node, then you can use the `remote-dev-over-tunnel` to connect from a local VSCode instance, or from the browser. Brendan Harris has kindly written up details [here](https://github.com/brendanjohnharris/physics-cluster/tree/main/code-physics).

