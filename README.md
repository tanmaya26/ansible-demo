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

### Demo Link

https://photos.app.goo.gl/H3J8dFJybG6p7THF6


### Concepts (20 points):

1. Explain continuous integration. How is it used on a project?
Continuous Integration (CI) is a software development practice where developers write and integrate code into a shared repository, usually several times a day. Each check-in is then verified by an automated build, allowing developers to detect problems at an early stage. It can also be looked at as a practice of automating the integration of code changes from multiple contributors into a single project. This version control is also supplemented with checks such as code quality (complexity) tests, syntax review and others during the integration.By integrating regularly, you can detect errors quickly, and locate them more easily.
In a project, CI is implemented using version control systems (Eg git, bitbucket). After the code is merged, a test suite is run. This test suite consists of unit, integration tests and other necessary tests. Generally, when a developer pushes code using the version control system an event will trigger the full test suite to run automatically. In the CI pipeline, the entire event of merge and test automation is stored as "Builds". Each build describes a new version and whether the build passed or not. After the builds, the developer can either manually trigger the deployment to different environment or the pipeline can be configured to automate deployment after build success. 

2. Why should developers use configuration management tools to manage their software programs? What can go wrong if they don't?




