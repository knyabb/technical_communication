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

    1. Open **Command Prompt** 
    2. Enter command below to check if jekyll is installed, if not, please follow download and install instruction above
        * jekyll -v
    3. Open documents folder by entering the command below
        * cd document
    4. Create your static website inside document folder by entering the command below
        * jekyll new demo-site
    5. Move into the folder that contains your static website by entering the command below
        * cd demo-site
    6. Launch the static website by entering the command below
        * bundle exec jekyll serve
    7. View static website by entering `localhost 4000` on your web browser 

2. **To format and host resume on a static website**
    
    1. Open **VSCode**
    2. Click on **File** on the menu tab
    3. Click on **open folder** on the File menu
    4. Select **demo-site** folder to open the static site folder on VS Code
    5. Create a markdown file **resume.md** inside **demo-site** folder
    6. Copy and paste your existing resume content into **resume.md**
    7. Format resume as shown on [U of M's Career Services Resume Workbook](https://umanitoba.ca/student/careerservices/media/Resume.pdf)
    8. Add the Front Matter below to the top of **resume.md** page to display resume as a page on the static website
        ```
        ---
        layout: page
        ---
        ```

### Instructions on how to host and format resume on a Github pages


### More Resources
* link to resume theme


### FAQs

### Licence

* git bash is the source control mangt system on windows, allows the user to type/run git commands that allows user to access remote repositoty on github

# DELETE LATER
Your README has two goals:
1. Describe the practical steps of how to host and format a resume using the software stack
you used for this assignment. The most common one is Markdown, VS Code, GitHub
Pages, and Jekyll.

2. Relate the practical steps described above to the general principles of current Technical
Writing, as explained in Andrew Etter's book Modern Technical Writing
Each README must contain these topics/components:

1. Title
2. Purpose: describe the README's purpose (see above)
3. Prerequisites: This should include a resume formatted in Markdown
Include a link to a good Markdown tutorial under "More Resources." You do not need
to explain how to use Markdown.
4. Instructions, including animated gif
Use headings and numbered lists
Remember to use each step to explain
both how to follow the tools and model Etter
recommends and how to host a resume in GitHub Pages or Codeberg Pages. It's up to
you whether you 1) begin with Etter's general process and then demonstrate the
process with a practical step involving your resume, or 2) begin with the practical
steps for hosting a resume and relate each practical step to a concept in Etter's book.
Add an animated gif: Include a demo using an animated gif in your README. The gif
should feature your own resume (showing your own name).
More Resources - include:
1. a Markdown tutorial
2. a link to Etter's book
3. at least one other resource
5. Authors and Acknowledgments: credit template authors and group members
6. FAQs - add (and answer) two FAQs, as described below:
1. A question about the overall process, such as "Why is Markdown better than a word
processor?"
2. A question about the practical details, such as "Why is my resume not showing up?"
You may use the example FAQs, or come up with your own.