### Technical Communication Project


### Purpose

* To describe practical steps on how to host and format a resume using VS Code, Git/Gitbash/GitHub, Github Pages, and Jekyll.
* To relate each practical step to principles of technical writing as explained in Andrew Etter's [book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).  


### Prerequisite
* [elukanle_resume](https://github.com/knyabb/technical_communication/blob/main/resume.md)


### Instruction on how to download and install software applications on windows
1. **Jekyll**

    * Download [RubyInstaller](https://rubyinstaller.org/downloads/) for windows.
    * Install **Jekyll** by following the steps under [Installing Ruby and Jekyll](https://jekyllrb.com/docs/installation/windows/).

2. **VS Code**
    * Download [VSCode](https://code.visualstudio.com/download) for windows.
    * Install **VSCode** by following the steps on [How to Install VSCode](https://www.youtube.com/watch?v=MAuLRELi2YA).

3. **Git bash**
    * Download [Git Bash](https://git-scm.com/downloads) for windows.
    * Install **Git bash** by following the steps on [How to Install Git Bash](https://www.youtube.com/watch?v=7BOrUHFu44A).

4. **GitHub**
    * Create an account on [github](github.com). 


### Instructions on how to host and format resume on a static website
1. **To create a static website**

    1. Open **Command Prompt**.
    2. Enter command below to check if jekyll is installed, if not, please follow download and install instruction above.
        ```
        jekyll -v
        ```
    3. Open documents folder by entering the command below.
            ```
            cd document
            ```
    4. Create your static website inside document folder by entering the command below.
            ```
            jekyll new demo-site
            ```
    5. Move into the folder that contains your static website by entering the command below.
        ```
        cd demo-site
        ```
    6. Launch the static website by entering the command below.
        ```
        bundle exec jekyll serve
        ```
    7. View static website by entering **localhost4000** on your web browser.

2. **To format and host resume on a static website**
    
    1. Open **VSCode**.
    2. Click on **File** on the menu tab.
    3. Click on **Open Folder** on the File menu.
    4. Select **demo-site** folder to open the static site folder on VS Code.
    5. Create a markdown file **resume.md** inside **demo-site** folder.
    6. Copy and paste your existing resume content into **resume.md**.
    7. Format resume as shown on [U of M's Career Services Resume Workbook](https://umanitoba.ca/student/careerservices/media/Resume.pdf).
    8. Add the Front Matter below to the top of **resume.md** page to display resume as a page on the static website.
        ```
        ---
        layout: page
        ---
        ```

### Instructions on how to host and format resume on a Github pages
1. **Select resume theme and template**

    1. Use a **theme** powered by Jekyll and Github [modern-resume-theme](https://rubygems.org/gems/modern-resume-theme).
    2. Download [resume-template-folder](https://github.com/sproogen/modern-resume-theme#step-3---download-resume-template) to access config file.

2. **Use Github**
    1. Create a [techical_communication](https://github.com/sproogen/modern-resume-theme#step-3---download-resume-template) github repository to host resume template and README file.

3. **Use VS Code**
    1. Open **VSCode**
    2. Click on **File** on the menu tab
    3. Click on **Open Folder** on the File menu
    4. Select downloaded **resume-template-folder** to open on VS Code.
    5. Edit the **_config.yml** file to reflect content of your **resume**
    6. Edit the **README.md** file to show practical steps taken to implement the project

4. **Use Git Bash to send resume-template-folder to remote server**
    1. Open **Git Bash**.
    2. Move to the folder that contains the downloaded **resume-template** by entering the command below.
        * cd documents
    3. Move to the **resume-template-folder** by entering the command below
        * cd resume-template-folder
    4. Inside the **resume-template-folder** , follow the steps below push files on **VS Code** to **Github** via **Git Bash**
        * Initialize as a git folder
            ```
            git init
            ```
        * Connect to Github repository
            ```
            git remote add origin https://github.com/knyabb/technical_communication.git
            ```
        * Create a gh-pages branch on the remote server
            ```
            git checkout -b gh-pages
            ```
        * Stage files that will be push to the remote server
            ```
            git add .
            ```
        * Commit files with appropriate commit message
            ```
            git commit -m "initial commit"
            ```
        * Push files to appropriate branch on the remote server
            ```
            git push origin gh-pages
            ```
    5. **Use Git Bash to send README.md to remote server**
        1. Open **Git Bash**.
    2. Move to the folder that contains the downloaded **resume-template** by entering the command below.
        * cd documents
    3. Move to the **resume-template-folder** by entering the command below
        * cd resume-template-folder
    4. Inside the **resume-template-folder** , follow the steps below push files on **VS Code** to **Github** via **Git Bash** 
        * check branch
            ```
            git branch
            ```
        * if branch is on gh-pages, switch branch to main branch
            ```
            git checkout main
            ```
        * Stage files that will be push to the remote server
            ```
            git add .
            ```
        * Commit files with appropriate commit message
            ```
            git commit -m "update README file"
            ```
        * Push file to appropriate branch on the remote server
            ```
            git push origin main
            ```




### More Resources
* link to resume theme

### Etthers book analysis

### FAQs

### Author And Acknolegment

### Licence

### Images

<!--- ![Shallow Backup GIF Demo](img/shallow-backup-demo.gif) --->

* git bash is the source control mangt system on windows, allows the user to type/run git commands that allows user to access remote repositoty on github