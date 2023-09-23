[Roadmap](https://github.com/orgs/jahoda-tech/projects/3)
[Documentation](https://jahoda-tech.github.io/)

   
# Rules of programming 👋


  1. make it correct (make it work)
  2. make it readable (refactor code for better orientation, easy to understand)
  3. make it small (reduce number of code lines)
  4. make it simple (change code to make it more beautiful, easier to read and understand) 
  5. make it fast (change algorithm, use benchmarks, make tests)

## General coding rules

https://dave.cheney.net/practical-go/presentations/qcon-china.html#_package_design

## Philosophy

1. Files should be maximal 1000 lines long, optimal below 500 lines.
2. Reduce communication with expensive things (like databases) to minimum.
3. Make code readable, it should read like an english book.
4. Comment are forbidden, use logging instead.
5. Always use main.go as a starting point for every software. Use default go coding conventions.
6. Handle errors first. Use switch instead of multiples if-else.
7. Every procedure, method or functions starts with logging message and ends with logging messages with result and
   elapsed
   time information.

## Naming

### Software naming

1. Software naming is lower case only with underscore.
2. First name is the name of the software.
3. Second name is the type.
4. _service is for software that does NOT have web
5. _webservice is for software that DOES have web
6. _communication is added for softwares that transfer data with another systems

**Examples:**
- zapsi_service
- state_service
- terminal_service
- display_webservice
- terminal_webservice
- lcd_webservice
- maplast_communication_service
- database
- ...

### File naming

1. File naming is lower case one name only.

**Examples:**
- config.go
- main.go
- log.go

2. If there are multiple files that bound together, use the same name.


- input_user.go
- input_user.html
- input_user.css
- input_user.js

### Variable naming

1. Variable naming is camelCase, reasonable name should be used.
2. Use reasonable and descriptive name

**Examples:**
runningDevices instead of rd, runDev, ...

## Github style of work

1. Only one branch is allowed.
2. Only one user can work on one software at a time.
3. All users have admin rights.
4. Every user is responsible for his or her work.

### New repository

1. First create repository on Github
2. Then pull repository to Goland and make changes

### Existing repository (only push and pull)

1. Send information about start working on specific software to messages
2. Always first pull (update) from github
3. Make changes
4. Update changelog.md
5. Commit and push changes
6. Send information about end working on specific software to messages

### Issues in Github Projects

1. All users are responsible for adding new issues for all repositories, when requested
2. All users are responsible for checking periodically all issues and assigning their work on those issues 
3. All users are responsible for managing issues states
4. All users are responsible for closing done issues

### Dashboard in Github Projects

1. All users are responsible for managing proper dashboard issues in project page

### Git commits in changelog.md

1. Commit after every change. Use these tags:

* ```Added``` for new features.
* ```Changed``` for changes in existing functionality.
* ```Deprecated``` for soon-to-be removed features.
* ```Removed``` for now removed features.
* ```Fixed``` for any bug fixes.
* ```Security``` in case of vulnerabilities.

## Technologies

- Main language: Go
- Additional languages: HTML, CSS., JavaScript
- ORM: GORM
- Http Router and Muxer: Gin
- Main Javascript Charting Library: Echarts
- Main database: PostgreSQL
- Runtime: Docker
- Git repository: Github
- Licence: MIT

## Versioning

Version contains year, quarter, month of the quarter and day of the month.

2019.2.1.24 is version from year 2019, second quarter, first month of second quarter, which is April, and from 24th of
April.

Every week build new "latest" and proper "2019.2.1.24" version

## DockerHub and Docker

1. Only petrjahoda is allowed to push new and updated dockerhub images
2. All dockerhub images are public




    
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
