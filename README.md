# Git Operations in Google Colab

This repository contains a Jupyter Notebook (`Git.ipynb`) that demonstrates common Git operations within a Google Colab environment.

## Notebook Contents

The `Git.ipynb` notebook is structured into several cells, each performing a specific action:

1.  **Mount Google Drive**:
    *   Connects and mounts your Google Drive to the Colab environment, allowing access to files stored there.
    *   Code:
        ```python
        from google.colab import drive
        drive.mount('/content/drive')
        ```

2.  **Check Current Directory**:
    *   Displays the current working directory within the Colab environment.
    *   Code:
        ```bash
        %pwd
        ```

3.  **Clone a Private Repository**:
    *   Clones a Git repository from GitHub.
    *   **Important**: You will need to replace `https://daquarti:Activos86@github.com/daquarti/privado.git` with your own repository URL and credentials (or use a token).
    *   Code:
        ```bash
        !git clone https://daquarti:Activos86@github.com/daquarti/privado.git
        ```
    *   The example shows cloning an empty repository named 'privado'.

4.  **List Directory Contents**:
    *   Lists the files and directories in the current working directory.
    *   Code:
        ```bash
        %ls
        ```

## How to Use

1.  **Open in Google Colab**:
    *   Click on the "Open In Colab" badge at the top of the `Git.ipynb` notebook, or upload it directly to your Google Colab environment.
2.  **Run Cells**:
    *   Execute the cells sequentially.
3.  **Modify for Your Use**:
    *   Particularly for the `git clone` command, ensure you update the repository URL and authentication details to match your own private repository. If you are cloning a public repository, you can remove the username and password/token from the URL.

This notebook serves as a basic guide and template for integrating Git version control into your Google Colab workflows.
