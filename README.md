# PSAP Assignments

This repository contains assignments for the PSAP (Programming Skills and Practices) course.

## How to Download

### Downloading Using ZIP

1. Navigate to the [PSAP Assignments](https://github.com/vinitshirbhate/PSAP_assignments.git) repository on GitHub.
2. Click on the green **Code** button located near the top-right corner of the repository.
3. Select **Download ZIP** from the dropdown menu.
4. Once the ZIP file is downloaded, extract its contents to your desired location on your computer.
5. Unzip the Folder open the Folder.
6. Right Click open in terminal and paste the Rename the PDF's commands.

### Cloning the Repository Using Git

To clone the repository using Git, you'll need to have Git installed on your computer. If you don't have Git installed, you can download and install it from [here](https://git-scm.com/downloads).

Open a terminal or command prompt and run the following command:

1. Clone the repository:

   ```bash
   git clone https://github.com/vinitshirbhate/PSAP_assignments.git

   cd PSAP_assignments
   ```

2. Rename The PDF's

   **For Windows**

   ```bash
   Get-ChildItem -Filter "assignment_*.pdf" | Rename-Item -NewName { $_.name -replace "assignment_", "Div<div>_<rollno>_" }

   ```

   **For Linux & MAC**

   ```bash
    find . -name "assignment_*.pdf" -exec bash -c 'mv "$1" "${1/assignment_/Div<div>_<Roll_number>_}"' _ {} \;

   ```
