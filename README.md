## **Technical Communication Project**


### **Purpose**

* To describe practical steps on how to host and format a resume using VS Code, Git/Gitbash/GitHub, Github Pages, and Jekyll.
* To relate each practical step to principles of technical writing as explained in Andrew Etter's [book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).  


### **Prerequisite**
* [elukanle_resume](https://github.com/knyabb/technical_communication/blob/main/resume.md)

### **How Practical Steps Implemented Relates to Andrew Etter's Principle of Technical Writing**
```
Practical steps implemented in this project relates to principle to technical writing described in Andrew Etter's book in such a way that my resume was originally editted and formatted in a markdown file on VS Code; then i use Git Bash to check out a repository on Github, apply a customised theme to the markdown file and host on Github pages via command line integration; a static website is produced. This ensures a more dynamic and versatile approach to produce scannable and searchable technical content and easy access for contribution.
```

#### **Instruction on how to download and install software applications on windows**
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
    * Create an account on [github](https://docs.github.com/en/get-started/onboarding/getting-started-with-your-github-account) using 1. 


#### **Instructions on how to host and format resume on a static website**

1. **To create a static website**

    1. Open **Command Prompt**.
    2. Enter command below to check if jekyll is installed, if not, please follow download and install instruction 1 above.
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
    7. View static website by entering address below on your web browser.
        ```
        localhost:4000
        ```

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

#### **Instructions on how to host and format resume on a Github pages**
1. **Select a markdown flavoured resume theme and template**

    1. Use a **theme** powered by Jekyll and Github [modern-resume-theme](https://rubygems.org/gems/modern-resume-theme).
    2. Download [resume-template-folder](https://github.com/sproogen/modern-resume-theme#step-3---download-resume-template) to access config file.

2. **On your Github account, create a public repository**
    1. Follow 1 to create [github repository](https://pages.github.com/) to host resume template and README file.

3. **Use VS Code to edit markdown and yml files**
    1. Open **VSCode**
    2. Click on **File** on the menu tab
    3. Click on **Open Folder** on the File menu
    4. Select downloaded **resume-template-folder** to open on VS Code.
    5. Edit the **_config.yml** file to reflect content of your **resume**
    6. Edit the **README.md** file to show practical steps taken to implement the project

4. **Use Git Bash to send resume-template-folder to remote server**
    1. Open **Git Bash**.
    2. Move to the folder that contains the downloaded **resume-template** by entering the command below.
        ```
        cd documents
        ```
    3. Move to the **resume-template-folder** by entering the command below
        ```
        cd resume-template-
        ```
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
        ```
        cd documents
        ```
    3. Move to the **resume-template-folder** by entering the command below
        ```
        cd resume-template-folder
        ```
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

### **FAQs**
* Why is Markdown better than Word Processor?
```
Markdown has a simple and faster formating syntax. Also documents written in Markdown can be exported into any format you want, Word Doc, PDF, HTML. Markdown document ensures life span as they are kept in version control.
```
* Why did my github pages did not build successfully?
```
To host on github pages, i used a resume template and theme supported by github pages. This theme has a default layout which makes modifying config file limited. Make sure you edit your config.yml file such that it does not distort the default layout.
```


### **More Resources**
* [Markdown Tutorial](https://www.youtube.com/watch?v=HUBNt18RFbo)
* [Andrew Etter's Book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
* [Modern Resume Theme](https://github.com/sproogen/modern-resume-theme)

### **Author and Acknowledgement**
    * Author - Kehinde Elukanle
    * Group Members
        * Robert Loader
        * Chang Geng
        * Michael Akpan

### **Licence**
* The resume theme is available under the terms of the [MIT License](https://opensource.org/license/mit/).

* The resume image is available under the terms of the [Adobe Stock License](https://stock.adobe.com/ca/license-terms).


### **Animated Resume**

![Animated Resume GIF Demo](img/animated-resume.gif)
