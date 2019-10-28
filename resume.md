Jamie Holland
===============
Email: jamesarthurholland@hotmail.com   
Mobile: 07854682887   
Github: <https://github.com/JamesArthurHolland>   
Linkedin: <https://www.linkedin.com/in/jamie-holland-9a3663181/>

A hard working developer with a varied skillset, seeking a new role within a challenging working environment.

Education
---------

*   Computer Science BSc 2:1 , University of Manchester, United Kingdom
*   Saint Malachy’s College, Belfast, Northern Ireland

Skills
---------------

*   **Paradigms**   
   - Strong OOP and functional skills.
   - Full understanding of GRASP principles and the importance of writing clean, maintainable code.
   - Comprehensive knowledge of why a certain language would or would not suit a particular use case, depending on the given non-functional requirements.   

*   **DevOps**   
   - Extensive DevOps experience in both previous and current roles, including the setup and maintenance of (but not limited to): K8s, Docker, Kafka, GCP (appengine, cloud scheduler, cloudtasks, dataflow, bigquery, spanner, buckets), AWS (ec2), Redis, Ansible, Chef, Vagrant/Virtualbox. Entrusted with DBA and sysadmin responsibilities on BPOR project.   
   - Docker use both in roles and learning in my spare time. Created a reusable skeleton for a highly scalable microservice application which uses the kafka messaging queue within a k8s cluster (to stream logs).
   - Experience with EMQTT and rabbitMQ, hence familiarity with the MQTT and AMQP protocols.

*   **Linux**   
   - Linux distros used almost exclusively for the last 6-7 years. Regularly asked for help by colleagues on other teams. Can set up and maintain users/ssh keys/systemd files/host file settings/ip tables/mysql dbs and other sysadmin tasks with ease.   
   - Avid command line user and will almost never be seen using a GUI if there is a commandline version.
   - Always writes scripts for repeated tasks to complement documentation, rather than just documentation.
   - Always creating and sharing aliases, to increase personal efficiency and that of others.

*   **Writing RESTful APIs and clients**   
Has written APIs in multiple frameworks, a firm understanding of inversion of control through dependency injection and is quick to learn new technologies. A strong awareness of the types of security vulnerabilities that are present when connecting clients to such APIs.

*   **Languages**
    - Java, Javascrjpt, Golang, Erlang, C, Python, Ruby and C++ to varying degrees throughout my career.
    - A keen interest in compilers and formal language theory. This has been realised through the creation of a transpiler called "Alfalfa" which allows developers to generate API endpoints extremely quickly, as well as the client libraries for those APIs.  
    
Employment
---------

*   **Consultant Analyst, PA Consulting, Belfast UK.** (November 2018 - present)

    *Lead Developer, Rentokil North America Enablement*
    
    - Created 2 POCs, to enable replication of data from an IBM as400 machine to a cloud based backend, to lay the foundation for the client to migrate to the cloud. One using apache beam (GCP dataflow), the other using cloud tasks.

    - Had serious input into the architecture of the decided upon approach. Currently retrieving data from the big query table it is backed up to, via a java appEngine app, to post to a GCP task queue (a suggestion for kafka was made), which then posts the task to a taskHandler which currently transforms the data to their old schema, but it is decoupled enough that we can switch that out whenever they have went fully cloud native.

    - Worked alongside an architect who was assigned to the project 2/5 days per week. Solely responsible for the coding of the POCs which got the new work order funding approved for 3 more months, as well as the implementation of the final solution.

    *Full Stack Developer, [www.bepartofresearch.ac.uk]*   
    
    - Developed a text classifier using text frequency inverse document frequency (TFIDF) and a logistic regression to train the model.
    
    - Migrated all the git repos from an internally firewalled gitlab, which was useless for provisioning to cloud, to bitbucket cloud.

    - Created a jenkins build server for all the NIHR projects at PA. Created pipelines for the BPOR project and also the HDF project. These pipelines reused the same ansible script that was used by vagrant/virtualbox to spin up a local development environment in an automated 1 script fashion.
   
    - The data coming into the site normally was live dynamic data. For test builds, created a SQL dump that was a subset of the live data, so that the data would be static, the response for certain requests would therefore be known, making automated testing possible. Postman’s test runner, newman, was utilised for these end to end tests. 
    
    - Introduced vueJS into the project, which meant for quicker development and better responsiveness on the page compared to writing error-prone vanilla js with jquery.

*   **Software Developer, American Dynamics, Belfast UK.** (February 2017 - October 2018)    
    
    - Tasked mostly with re-factoring legacy code and successfully decreasing the build time of the compilation from 40 minutes to 2 minutes for an incremental build. This was achieved by converting the entire build from GNU Make to CMake, not only did this vastly improve developer efficiency in terms of compilation time, but also sped up development time in the fact that it allowed for greater integration with CLion, the jetbrains IDE which a lot of the staff were using. 

    - Worked on a C++ test tool that was used to mimic a camera communicating with the network video recorder. This tool used the realtime streaming protocol over both TCP and UDP. Gstreamer was the library used for this.

*   **Graduate Software Developer, Fidessa, Belfast UK.** (October 2016 - January 2017)

    - Product owner of an internal documentation website. Given sole responsibility to rewrite an existing internal website.
    
    - The new web application exists as a single page web application, using PHP/MongoDB on the backend and AngularJS on the frontend.
    
    - Completion this project under minimal supervision, strengthening my existing ability to elicit requirements from non-technical stakeholders in a software development project, through easy to digest dialogue.

*   **Internship, rentalcars.com, Manchester UK.** (March 2015 - August 2015)

    - Worked as part of the backend payment team and also the mobile team on a massive car rental price comparison site.
    
    - Had worked with Android previously in my spare time and settled into the more formal setting with ease. Worked mostly on the new version of the RentalCars app (now live in the playstore).
    
    - Implemented custom widgets on the welcome screens and handled the client side login functionality. Implemented the side navigation drawer and all of the screens/functionality that can be accessed from the drawer.

*   **Summer Internship, channelgrabber.com, Manchester UK.** (June 2014 October 2014)

    - Worked as part of an agile development team on a stock management program for eBay and Amazon.
    
    - Implemented API end points as well as front end UI for the browser.
    
    - Learnt how to make scalable 3 tier web applications and had some exposure to the security concerns of such applications, such as firewalling the API layer, using SSL keys etc.
    
    - Programmed MySQL wrapper classes that were safe from SQL injection.

Projects
------

*   **Alfalfa (Currently being refactored to use yml and java8)**
    - Alfalfa is an open source code generation language that is available on my github. Realised through a compiler I wrote from scratch. The idea for this tool arose out of my desire to be more efficient while developing API endpoints.
    
    - Almost all of the system class patterns that one uses in a web application have a common implementation structure, the only things that change are the variables. Alfalfa allows for the creation of templates for recurring software patterns to allow for the auto generation of e.g object (POJO in java), service, mapper and database wrapper classes for given variables.
    
    - Written in Java but accepts templates written in any language (mixed with Alfalfa directives).
    
*   **GPingS - Android and Swift**
    - GPingS is a conceptual app to demonstrate programming ability in native mobile languages.
    
    - Allows the user to stream their GPS location to a friend (within the app). It uses MQTT messaging for realtime updates and websockets to stream the location to a ruby backend. GPingS has an Android version and an iOS version written in swift.


