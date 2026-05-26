# How to Contribute to EmulatorEggs

[TOC]

## How to Contribute to EmulatorEggs 

GitHub Repository: [https://github.com/emulatoreggs/emulatoreggs](https://github.com/emulatoreggs/emulatoreggs)

### Option 1: Opening an Issue or Discussion

You will need to create a GitHub account to open an issue. To sign up for GitHub, see [https://github.com/signup](https://github.com/signup).

Once you have created an account, open the following page, [https://github.com/emulatoreggs/emulatoreggs/issues](https://github.com/emulatoreggs/emulatoreggs/issues), and submit an issue. 

Alternatively open a discussion post, [https://github.com/emulatoreggs/emulatoreggs/discussions](https://github.com/emulatoreggs/emulatoreggs/discussions)

### Option 2: Editing the Markdown files 

#### How to Contribute Using GitHub's Web Editor

Select a page to edit and follow one of the below options:

* **Method 1**
    1. On the respective wiki page, click the pencil icon in the top right and make your changes. 
    2. Once you are finished making your changes, click the `Commit changes...` button in the bottom left. 
    3. You will be prompted to create a Pull Request. 
    4. Add a little bit of detail about what you added and why.
    5. Submit your Pull Request.
    6. Once your Pull Request is reviewed, it will be merged and any of your changes will automatically be deployed to the website.
* **Method 2**
    1. Select a document to edit in the `docs` folder: [https://github.com/emulatoreggs/emulatoreggs/tree/main/docs](https://github.com/emulatoreggs/emulatoreggs/tree/main/docs).
    2. On the page you would like to edit, click the `Edit` button in the top right
    3. Click `Edit single file` and make your changes. 
    4. Once you are finished making your changes, click the `Commit changes...` button in the bottom left. 
    5. You will be prompted to create a Pull Request. 
    6 Add a little bit of detail about what you added and why.
    7. Submit your Pull Request.
    8. Once your Pull Request is reviewed, it will be merged and any of your changes will automatically be deployed to the website.

#### How to Contribute Using a Cloned Repository

##### Recommended Software

This is not a definitive list of software, but instead a tailored list for those new to contributing to GitHub repositories.

* [GitHub Desktop](https://desktop.github.com/)
* [Visual Studio Code](https://code.visualstudio.com/)

##### Cloning

Clone the EmulatorEggs repository, using one of the below methods:

* Command line
    * `git clone https://github.com/emulatoreggs/emulatoreggs.git`
* [GitHub Desktop](https://desktop.github.com/)
* [Clone and use a GitHub repository in Visual Studio Code](https://code.visualstudio.com/docs/sourcecontrol/github)
* Through your preferred software not listed above


##### Python

The EmulatorEggs wiki uses python for MkDocs, MkDocs-Material (the theme), and many of its extensions.

If you are on Windows, you can download Python from the website at [https://www.python.org/](https://www.python.org/). If you are on Linux, you can install Python from the various package managers.

##### Virtual Environments and Pull Requests

In your newly cloned repo, set up a virtual environment to localize your Python install to the work you do on the EmulatorEggs wiki.

Follow the instructions on Python's documentation, [https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) to learn how to create a virtual environment. The `.venv` folder is ignored when you commit to the GitHub repository.

After you have set up your virtual environment, install the various software with the following line:

`python3 -m pip install -r requirements.txt`

Generally, when you are starting work on the EmulatorEggs wiki, the flow will look like the following:

* (**If first time or if EmulatorEggs folder is deleted**):
    * Clone the EmulatorEggs repository to a folder of your choice:
        * git clone https://github.com/emulatoreggs/emulatoreggs.git 
* Open a terminal and `cd` to the EmulatorEggs cloned repository.
    * `cd /PATH/TO/EMULATOREGGS`
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
    * Use the `GitHub Pull Requests and Issues` in Visual Studio Code, [hhttps://code.visualstudio.com/docs/sourcecontrol/github](https://code.visualstudio.com/docs/sourcecontrol/github)

***

**Thank you for contributing!**
