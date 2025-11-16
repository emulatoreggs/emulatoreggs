# How to Contribute to Emuguinpedia

[TOC]

## How to Contribute to Emuguinpedia 

GitLab Repository: [https://gitlab.com/emuguinpedia/emuguinpedia](https://gitlab.com/emuguinpedia/emuguinpedia)

### Option 1: A quick shout-out

Send a quick message on Emuguinpedia's Discord stating what needs to be edited or added.

[Emuguinpedia Discord Link](https://discord.gg/d8rdpamJqj)

### Option 2: Opening an Issue

You will need to create a GitLab account to open an issue. To sign up for GitLab, see [https://gitlab.com/users/sign_up](https://gitlab.com/users/sign_up).

Once you have created an account, open the following page, [https://gitlab.com/emuguinpedia/emuguinpedia/-/issues](https://gitlab.com/emuguinpedia/emuguinpedia/-/issues), and submit an issue. 

### Option 3: Editing the Markdown files 

#### How to Contribute Using GitLab's Web Editor

Select a page to edit and follow one of the below options:

* **Method 1**
    1. On the respective wiki page, click the pencil icon in the top right and make your changes. 
    2. Once you are finished making your changes, click the `Commit changes...` button in the bottom left. 
    3. You will be prompted to create a Pull Request. 
    4. Add a little bit of detail about what you added and why.
    5. Submit your Pull Request.
    6. Once your Pull Request is reviewed, it will be merged and any of your changes will automatically be deployed to the website.
* **Method 2**
    1. Select a document to edit in the `docs` folder: [https://gitlab.com/emuguinpedia/emuguinpedia/-/tree/master/docs](https://gitlab.com/emuguinpedia/emuguinpedia/-/tree/master/docs).
    2. On the page you would like to edit, click the `Edit` button in the top right
    3. Click `Edit single file` and make your changes. 
    4. Once you are finished making your changes, click the `Commit changes...` button in the bottom left. 
    5. You will be prompted to create a Pull Request. 
    6 Add a little bit of detail about what you added and why.
    7. Submit your Pull Request.
    8. Once your Pull Request is reviewed, it will be merged and any of your changes will automatically be deployed to the website.

#### How to Contribute Using a Cloned Repository

##### Recommended Software

This is not a definitive list of software, but instead a tailored list for those new to contributing to GitLab repositories.

* [GitHub Desktop](https://desktop.github.com/)
* [Visual Studio Code](https://code.visualstudio.com/)

##### Cloning

Clone the Emuguinpedia repository, using one of the below methods:

* Command line
    * `git clone https://gitlab.com/emuguinpedia/emuguinpedia.git`
* [GitHub Desktop](https://desktop.github.com/)
* [Clone and use a GitLab repository in Visual Studio Code](https://docs.gitlab.com/ee/user/project/repository/#clone-and-open-in-visual-studio-code)
* Through your preferred software not listed above


##### Python

The Emuguinpedia wiki uses python for MkDocs, MkDocs-Material (the theme), and many of its extensions.

If you are on Windows, you can download Python from the website at [https://www.python.org/](https://www.python.org/). If you are on Linux, you can install Python from the various package managers.

##### Virtual Environments and Pull Requests

In your newly cloned repo, set up a virtual environment to localize your Python install to the work you do on the Emuguinpedia wiki.

Follow the instructions on Python's documentation, [https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) to learn how to create a virtual environment. The `.venv` folder is ignored when you commit to the GitLab repository.

After you have set up your virtual environment, install the various software with the following line:

`python3 -m pip install -r docs/requirements.txt`

Generally, when you are starting work on the Emuguinpedia wiki, the flow will look like the following:

* (**If first time or if Emuguinpedia folder is deleted**):
    * Clone the Emuguinpedia repository to a folder of your choice:
        * git clone https://gitlab.com/emuguinpedia/emuguinpedia.git
* Open a terminal and `cd` to the Emuguinpedia cloned repository.
    * `cd /PATH/TO/EMUGUINPEDIA`
* **(If first time or if .venv folder is deleted)**
    * Linux: `python3 -m venv .venv`
    * Windows: `py -m venv .venv`
* In the same folder as the cloned repository and the `.venv` folder:
    * Linux: `source .venv/bin/activate`
    * Windows: `.venv\Scripts\activate`
* `mkdocs serve`
    * This line will provide you with a URL in which you can see your edits in real time.
* Make your changes to the documents while testing the changes in a web browser of your choice.
* When you are finished, save your changes and create a `Pull Request` 
    * [Creating an issue or pull request from GitHub Desktop](https://docs.github.com/en/desktop/working-with-your-remote-repository-on-github-or-github-enterprise/creating-an-issue-or-pull-request-from-github-desktop)
    * Use the `GitLab Workflow Extension` in Visual Studio Code, [https://about.gitlab.com/blog/2020/07/31/use-gitlab-with-vscode/](https://about.gitlab.com/blog/2020/07/31/use-gitlab-with-vscode/)

***

**Thank you for contributing!**
