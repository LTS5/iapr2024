# Image Analysis and Pattern Recognition

## General information
* Lecturer(s): [Jean-Philippe Thiran][jpt], [Behzad Bozorgtabar][bb]
* [EE-451 coursebook][coursebook]
* [Moodle][moodle]

[moodle]: https://moodle.epfl.ch/course/view.php?id=5091
[jpt]: https://people.epfl.ch/115534
[bb]: https://people.epfl.ch/behzad.bozorgtabar
[coursebook]: https://edu.epfl.ch/coursebook/en/image-analysis-and-pattern-recognition-EE-451

### Objective of this course
Learn the basic methods of digital image analysis and pattern recognition:
pre-processing, image segmentation, shape representation and classification.
These concepts will be illustrated by applications in computer vision and
medical image analysis.

### Objective of this repository
This repository contains the material for the labs and project associated with
the [EPFL] master course
[EE-451 Image Analysis and Pattern Recognition][edu].

[epfl]: https://www.epfl.ch/
[edu]: https://edu.epfl.ch/coursebook/en/image-analysis-and-pattern-recognition-EE-451

### Labs instructions

The lab assignments aim to impart practical implementation skills related to the topics covered in class and serve as preparation for the final project. The final project is a hands-on endeavor that consolidates the concepts covered throughout the course. The labs themselves are in the form of Jupyter Notebooks, and need to be solved in groups of **three students**. Please make your groups on Moodle before `March 8th`.

It is important to note that the labs will be **graded**. For each lab, each group is required to submit one Jupyter notebook on Moodle, following the naming convention `lab_x_SCIPER1_SCIPER2_SCIPER3.ipynb`, where 'x' indicates the lab number, and SCIPER1, SCIPER2, and SCIPER3 denote the SCIPER of each group member.

To ensure uniformity and minimize code conflicts, we strongly advise following the provided `Installation Instructions` below.

**Important Note:** Before submitting each notebook, please execute the command `Kernel > Restart & Run All` to run the entire notebook from scratch. This ensures that the code runs correctly. We will re-run each notebook during evaluation to verify the correctness of your code.

## Installation instructions

### Python and packages
We will be using [git], [Python], and packages from the
[Python scientific stack][scipy].
If you don't know how to install these on your platform, we recommend to
install [Anaconda] or [Miniconda], both are distributions of the [conda]
package and environment manager.
Please follow the below instructions to install it and create an environment
for the course:

1. Download the latest Python 3.x installer for Windows, macOS, or Linux from
   <https://www.anaconda.com/download> or <https://conda.io/miniconda.html>
   and install with default settings.
   Skip this step if you have conda already installed (from [Miniconda] or
   [Anaconda]).
   Linux users may prefer to use their package manager.
   * Windows: Double-click on the `.exe` file.
   * macOS: Double-click on the `.pkg` file.
   * Linux: Run `bash Anaconda3-latest-Linux-x86_64.sh` in your terminal.
1. Open a terminal. For Windows: open the Anaconda Prompt from the Start menu.
1. It is recommended to create an environment dedicated to this course with
   `conda create -n iapr python=3.9.18`.
1. Activate the environment:
   * Linux/macOS: `conda activate iapr`.
   * Windows: `activate iapr`.
1. Install the packages we will be using for this course:
   * `conda install notebook`
1. You can deactivate the environment whenever you are done with `deactivate`
1. Install git if not already installed with `conda install git`.
1. Follow git instructions in the `Github` section below.
   
[git]: https://git-scm.com
[python]: https://www.python.org
[scipy]: https://www.scipy.org
[anaconda]: https://anaconda.org
[miniconda]: https://conda.io/miniconda.html
[conda]: https://conda.io

### Github

Git serves as a valuable tool for collaborative teamwork. To seamlessly access the upcoming labs and projects we'll be releasing throughout the semester, and to facilitate collaboration using Git, we highly recommend following these steps:

1. Initiate the process by creating a private **empty** repository for your group, `<my_group_repo>`, on Github. Ensure that it **does not** include `README.md` and `.gitignore`.
1. Clone your group remote repository locally using the command: `git clone https://github.com/<my_group_repo>`.
1. Establish the course repository, iapr, as a remote repository by executing the command: `git remote add upstream https://github.com/LTS5/iapr2024.git` (or use the SSH variant if preferred).
1. Stay up-to-date by fetching and merging changes from the iapr repository into your local branch with: `git pull upstream main`.
1. Once you've collected the code, push it to your remote repository: `git push origin main`.

Throughout the semester, we will periodically update the `iapr` repository with new labs and the project. To sync with the latest data, execute `git pull upstream main`. Exercise caution for potential conflicts; it's advisable to rename your Juypter Notebooks to `lab_x_SCIPER1_SCIPER2_SCIPER3.ipynb` (See Lab instructions) to prevent accidental overwriting of your code during merges.

### Python editors

[Jupyter] is a very useful editor that run directly in a web browser.
You can have Python and Markdown cells, hence it is very useful for
 examples, tutorials and labs.
 We encourage to use it for the lab assignments.
 To launch a Jupyter Notebook:
 * Open a terminal (for Windows open the Anaconda Prompt)
 * Move to the git repository `/path/to/iapr`
 * Activate the environment with `source activate iapr` (For Windows:
 `activate iapr`)
 * Run the command: `jupyter notebook`.

[jupyter]: https://jupyter.org/
