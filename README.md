# Site
repository: knyabb/technical_communication
favicon: images/favicon.ico

# Content configuration version
version: 2

# Personal info
name: Kehinde Elukanle
title: Business Systems Analyst
email: kehindelukanle@gmail.com
website: www.github.com/knyabb/technical_communication

# Dark Mode (true/false/never)
darkmode: false

# Social links
twitter_username: KElukanle
github_username:  knyabb
# stackoverflow_username: "00000001"
# dribbble_username: jekyll
# facebook_username: jekyll
# flickr_username: jekyll
#instagram_username: jameswgrant
linkedin_username: kehinde elukanle
# xing_username: jekyll
# pinterest_username: jekyll
#youtube_username: globalmtb
# googleplus_username: +jekyll
# orcid_username: 0000-0000-0000-0000

# Additional icon links
additional_links:
- title: itsgoingto.be
  icon: fas fa-globe
  url: https://www.itsgoingto.be
# - title: another link
#   icon: font awesome brand icon name (eg. fab fa-twitter) (https://fontawesome.com/icons?d=gallery&m=free)
#   url: Link url (eg. https://google.com)

# Google Analytics and Tag Manager
# Using more than one of these may cause issues with reporting
# gtm: "GTM-0000000"
# gtag: "UA-00000000-0"
# google_analytics: "UA-00000000-0"

# About Section
# about_title: About Me
#about_title: Professional Summary
about_profile_image: images/black_girl.jpg
about_content: | # this will include new lines to allow paragraphs
  Technically sound Final Year Computer Science Student and Certified Project Manager with good knowledge of the software development lifecycle, unified modeling language, programming languages including Java, Python with a wide range of e-commerce applications and technology skills. Known for excellent troubleshooting skills, able to analyze code and engineer well-researched, cost-effective, responsive solutions. Solid understanding of project management processes, and currently seeking a full time position within a technology-driven organization

  this is interesting
  ok what is going on

content:
  - title: Education # Title for the section
    layout: list # Type of content section (list/text)
    content: | 
      - layout: left
        title: University of Manitoba
        caption: 2018 - Present
        sub_title: BSc Computer Science
        description: |
          this is great great 
        # description: | # this will include new lines to allow paragraphs
        #   - Experienced in object-oriented programming; developing, testing and debugging code; designing interfaces; and administering systems and networks.
        #   - Solid, persuasive and genuine communication (verbal and non-verbal), facilitation and relationship-building skills.
        #   - Quick learner and ready to master new technologies; successful at working in both team and self-directed settings.
        #   - Proficient in Java, Python, Ansible, Git, GitHub, Linux, Windows, MS Office Suite.

  - title: Work Experience # Title for the section
    layout: list # Type of content section (list/text)
    content:
      - layout: left
        title: Royal Bank Canada
        link: rbcroyalbank.com
        # link_text: boringcompany.com
        sub_title: Business Analyst Intern
        caption: May 2021 - August 2022
        # description: | 
        #   - Developed compliance logical rules to audit running configuration of over 1000 production devices using Ansible Automation and Prime-infrastructure tool, resulting in accurate compliance visibility foe all stakeholders.
        #   - Increased compliance percentage by 78% by creating remediation workflow for non-compliant production devices thus standardizing their running configuration as per Cisco and RBC standard.
        #   - Reviewed existing solution to create an automated solution for Bell Shared Internet and compliance projects, eliminating code repetition and reducing time spent on scheduling change requests by 90%.
        #   - Collaborated with senior team members and engineers to implement compliance fix jobs, debug code error messages without impacting production workflow.
        #   - Maintained detailed code base and source control processes in GitHub to improve collaboration, visibility, accuracy, and efficiency.
      # - layout: left
      #   title: Hunter Douglas Inc, Dubai, UAE
      #   link: hunterdouglas.com
      #   # link_text: boringcompany.com
      #   sub_title: Project Coordinator
      #   caption: January 2017 – June 2017
      #    description: | 
      #      - Developed project requirements with the design team by selecting the best materials based on project specification using cost-benefit analysis, resulting in the most profitable project for the company
      #      - Led the project team to implement improvements based on technology advancement by evaluating the effectiveness of current processes, thereby eliminating huge risk impact for all possible project delays.

  - title: Volunteer Experience # Title for the section
    layout: list # Type of content section (list/text)
    content:
      - layout: left
        title: Living Interiors & Furniture Contracting, Abu Dhabi, UAE
        link: livinginteriors.com
        # link_text: boringcompany.com
        sub_title: Project Administrator
        caption: April 2015 – August 2016
        # description: | 
        #   - Developed an automated project sales spreadsheet to eliminate huge sales discrepancies and provide accurate sales information for all stakeholders.
        #   - Developed a questionnaire to collect qualitative data from all suppliers, built relationships with all suppliers to gain their confidence, ensure expedited means of delivery for all supplies, resulting in an increased client base by 15%. 

      # - layout: left
      #   title: Franke Care System Middle East, Doha, Qatar
      #   link: frankecare.com
      #   # link_text: boringcompany.com
      #   sub_title: Project Planner
      #   caption: January 2013 – April 2015
      #    description: | 
      #      - Worked with a team of 4 professionals to create a project baseline program by translating project requirements into qualitative and quantitative data, resulting in project progress reports for management review.
      #      - Implemented mitigation plans on possible contractor delays to complete project deliverables on time, resulting in zero contractual penalties.

   - title: Training and Certification # Title for the section
    layout: text # Type of content section (list/text)
    content: | 
      Project Management Professional (PMP) - Project Management Institute 2013
     
  - title: A Little More About Me
    layout: text
    content: | # this will include new lines to allow paragraphs
      Alongside my interests in networks and software engineering some of my other interests and hobbies are:
      - Rock climbing
      - Gaming
      - Knitting
      - [Becoming a ninja](https://www.youtube.com/watch?v=vtg4o__aRMg)

      Look at this cool image  
      ![Trees](/modern-resume-theme/images/landscape-trees.jpg "Trees")

# Footer
footer_show_references: true
# references_title: References on request (Override references text)

# Build settings
remote_theme: sproogen/resume-theme

sass:
  sass_dir: _sass
  style: compressed

plugins:
 - jekyll-seo-tag
