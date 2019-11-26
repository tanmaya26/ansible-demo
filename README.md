# HW5-510


### Instructions to run.

1. git clone https://github.ncsu.edu/tnanda/HW5-510.git
2. cd HW5-510/ansible
3. baker bake
4. baker ssh

Once inside VM, run the following commands
1. cd /ansible
2. ansible-playbook roles.yml
3. ansible-playbook tasks.yml

NOTE: All the assignment tasks including setup are in tasks.yml file. 

### Demo Link

[click me](https://photos.app.goo.gl/RyCQxv8PHaBbTyBt6)


### Concepts (20 points):

1. Explain continuous integration. How is it used on a project?<br>
Continuous Integration (CI) is a software development practice where developers write and integrate code into a shared repository, usually several times a day. Each check-in is then verified by an automated build, allowing developers to detect problems at an early stage. It can also be looked at as a practice of automating the integration of code changes from multiple contributors into a single project. This version control is also supplemented with checks such as code quality (complexity) tests, syntax review and others during the integration.By integrating regularly, you can detect errors quickly, and locate them more easily.
In a project, CI is used using version control systems (Eg git, bitbucket). After the code is merged, a test suite is run. This test suite consists of unit, integration tests and other necessary tests. Generally, when a developer pushes code using the version control system an event will trigger the full test suite to run automatically. In the CI pipeline, the entire event of merge and test automation is stored as "Builds". Each build describes a new version and whether the build passed or not. After the builds, the developer can either manually trigger the deployment to different environment or the pipeline can be configured to automate deployment after build success. 

2. Why should developers use configuration management tools to manage their software programs? What can go wrong if they don't?<br>
CM is essential to systematically manage the software and control the changes during the entire development cycle. 
CM tools help to make sure any changes whether changes in versioning, packages, or code changes must be applied to the software such that it doesn't break the existing product. It maintains the current state of software as well as lets developers add new features and versions. Other reasons include:
    - Software is deployed to remote servers and runs on cloud or VMs. CM is necessary to automate running the application on remote application without local intervention
    - Changes are made fequently to the software with growing changes in requirements and version updates. CM tools help to take care of these concurrent changes without breaking the components.
    - CM tools help to gracefully handle installation and deployment even when scripts fail. 
    - Softwares today runs on various platforms or Operating systems with the help of CM tools. 
    - Most softwares today rely heavily on open source packages and tools and CM helps to take care of handling version updates of external dependencies. 
    - Developers are distributed geographically over the world and make concurrent changes and updates to the software. CM helps manage the updates to code, handles merges, builds and deployment efficiently. 
  
    If CM is not used, many things could go wrong: 
  
    - It will become tedious and redundant to manage concurrent changes to software and integrate each change one by one as in today's time developers merge code almost many times a day.
    - There could be product incompatibility on different platforms or version conflict. Without CM, these problems will be detected at later stage in Production
    - Build failure will result in breakdown of the product and often manual intervention to fix the components.  
    - Out-of-date software packages with catastrophic results. Without CM, teams can easily miss out on maintaining latest software versions or patches. 
    - Manual fixing of recurrent software issues is costly and inefficient. 


