# Machine Learning in Finance II - labs dedicated to machine learning tools

# Table of contents
1. [Creation of virtual environments](#venv)
2. [Basic usage of git and GitHub](#git)
3. [Project setup in Kedro framework](#kedro)

## Creation of virtual environments <a name="venv"></a>
### Creating a Python Virtual Environment in a Specific Location

A virtual environment is a self-contained directory that contains its own Python interpreter and packages. This allows you to manage project dependencies separately. In this tutorial, we will learn how to create a Python virtual environment in a specific location using the `venv` module.

### Prerequisites

Before you begin, make sure you have Python installed on your system. If not, you can download and install Python from [python.org](https://www.python.org/downloads/).

#### Step 1: Open a Terminal or Command Prompt

Open your terminal or command prompt. The steps may vary depending on your operating system.

##### On Windows

- Press `Win + R`, type `cmd`, and press Enter.

##### On macOS

- Press `Cmd + Space`, type `Terminal`, and press Enter.

##### On Linux

- Use the keyboard shortcut to open the terminal (e.g., `Ctrl + Alt + T`).

#### Step 2: Navigate to the Desired Location

Use the `cd` command to navigate to the directory where you want to create your virtual environment.

```bash
cd /path/to/your/desired/location
```

Replace `/path/to/your/desired/location` with the actual path where you want to create the virtual environment.

#### Step 3: Create the Virtual Environment

Run the following command to create a virtual environment named `venv`:

```bash
python -m venv venv
```

If you're using Python 3.3 or newer, you can use the `python3` command:

```bash
python3 -m venv venv
```

This command creates a directory named `venv` containing the virtual environment.

#### Step 4: Activate the Virtual Environment

Activate the virtual environment. The activation command may differ based on your operating system.

##### On Windows

```bash
venv\Scripts\activate
```

##### On macOS and Linux

```bash
source venv/bin/activate
```

Once activated, you will see the virtual environment's name in your command prompt or terminal.

#### Step 5: Deactivate the Virtual Environment

When you're done working in the virtual environment, you can deactivate it:

```bash
deactivate
```

This returns you to the global Python environment.

Congratulations! You have successfully created and activated a Python virtual environment in a specific location.

--------------------------------------------------------
## Basic usage of git and GitHub <a name="git"></a>

In this tutorial, we will cover the fundamental concepts of version control using Git and how to collaborate with GitHub. These skills are essential for managing and tracking changes in your projects.

#### Step 1: Install Git

If you haven't installed Git on your machine, you can download and install it from [here](https://git-scm.com/).

#### Step 2: Set Up Git

Configure your Git username and email with the following commands (please use GitHub credentials). Replace "Your Name" and "your.email@example.com" with your actual name and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

#### Step 3: Create a GitHub Repository

1. Create and log in to your GitHub account.
2. Set up GitHub token - https://github.com/settings/tokens.
3. Click on the "+" sign in the top right corner and select "New repository."
4. Name your repository and provide a description.
5. Optionally, initialize this repository with a README file.
6. Click "Create repository."

#### Step 4: Clone the Repository

Copy the URL of the repository you just created on GitHub. Open the terminal, navigate to the directory where you want to clone the repository, and run:

```bash
git clone https://github.com/your-username/your-repository.git
```

Replace the URL with the one you copied.

#### Step 5: Navigate to the Project Directory

```bash
cd your-repository
```

#### Step 6: Make Commits

After making changes to your project, stage the changes and make a commit.

```bash
git add .
git commit -m "Your commit message here"
```

Repeat these steps whenever you make changes to your project.

#### Step 7: Create Branches

Create a new branch to work on features or fixes without affecting the main codebase.

```bash
git branch feature-branch
git checkout feature-branch
```

Alternatively, you can use a shortcut:

```bash
git checkout -b feature-branch
```

#### Step 8: Fetch Changes

Fetch changes from a remote repository (like GitHub) to update your local repository.

```bash
git fetch
```

#### Step 9: Pull Changes

Pull changes from a remote repository into your current branch.

```bash
git pull origin master
```

Replace "master" with the branch you want to pull changes from.

#### Step 10: Push Changes

Push your changes to a remote repository, such as GitHub.

```bash
git push origin feature-branch
```

Replace "feature-branch" with the name of your branch.

#### Step 11: Merge Branches

Merge changes from one branch into another.

```bash
git checkout master
git merge feature-branch
```

#### Step 12: Handling Merge Conflicts

If there are conflicts during a merge, resolve them manually, then commit the changes.

Congratulations! You've covered the basics of Git and GitHub. These commands will help you manage and collaborate on projects effectively.
Here you can find decent git tutorial which will cover all necessary commands and concepts: https://www.atlassian.com/git/tutorials.

## Project setup in Kedro framework <a name="kedro"></a>
Kedro is an open-source Python framework to create reproducible, maintainable, and modular data science code. It uses software engineering best practices to help you build production-ready data science pipelines.

Official project documentation: https://docs.kedro.org/en/stable/index.html

We will follow Kedro's brilliant documentation and tutorials:
1. Kedro concepts: https://docs.kedro.org/en/stable/get_started/kedro_concepts.html
2. Set up Kedro: https://docs.kedro.org/en/stable/get_started/install.html
3. Create new Kedro project: https://docs.kedro.org/en/stable/get_started/new_project.html
4. Tutorial: https://docs.kedro.org/en/stable/tutorial/spaceflights_tutorial.html
5. Kedro viz:
    5.1 introduction: https://docs.kedro.org/projects/kedro-viz/en/stable/kedro-viz_visualisation.html
    5.2 charts visualization: https://docs.kedro.org/projects/kedro-viz/en/stable/visualise_charts_with_plotly.html
    5.3 experiments tracking: https://docs.kedro.org/projects/kedro-viz/en/stable/experiment_tracking.html 
8. More details: https://docs.kedro.org/en/stable/starters/index.html and https://docs.kedro.org/en/stable/kedro_project_setup/index.html
9. More advanced stuff - kedro-mlflow: https://kedro-mlflow.readthedocs.io/en/stable/source/03_getting_started/01_example_project.html



