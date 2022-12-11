..
   - Format for README.rst:
      1. Three Empty Lines between (sub)sections and (sub)sections. (Clear to view and edit)
      2. Zero Empty Lines between (subsections) and content right below it.






"""""""""""""""""
Development Guidance
"""""""""""""""""



...........
UTM021 IT Development Team
...........
.. contents:: Overview
   :depth: 3
   
   
   
===================
Quick Start
===================



----------------------
SetUp
----------------------
.. code:: sh
  
   cd /you/github  # your directory
   git clone https://github.com/24ERIC/official_website.git # clone code into the directory



----------------------
Run in Local
----------------------
.. code:: sh

   cd /official_website  # step into folder
   python3 manage.py runserver  # Note: "python3" may depends. # start local server, default IP: http://127.0.0.1:8000/



----------------------
Development Plan
----------------------
Plan is in Github "Project" option.



----------------------
Ask for necessary prvilege from IT Administrator.
----------------------
Prvilege includes:

• Access to Github Repository
• Access to Github Development Plan "Projects"



===================
Deployment
===================
We deploy the website on https://vercel.com for free.

NOTE: Please be aware that many settings in project are mandatory to deploy website on vercel successfully!



===================
Agile Develop Process
===================


----------------------
1 - Define Requirements
----------------------
In this project, we have two parts:

First: UTM021 Official Website

Second: UTM021 IT Department Back Yard



----------------------
2 - IU Design
----------------------
We need to design interface during each iteration.



----------------------
3 - Development
----------------------
We have the design, and the plan, now we start develop the application.



3.1 - SOLID Priniple
--------------------------
Priciples all developers should follow to make clean code, and easy add/ edit/ extend project in future.

• Single responsibility principle
   • Every class should have a single responsibility.
   • Every class should have one reason to change.
   
• Open/closed principle
   • Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification.
   • Add new features not by modifying the original class, but rather by extending it.
   
• Liskov substitution principle
   • If S is a subtype of (i.e. inherited or derived from) T, then objects of type S may be substituted for objects of type T without altering any of the desired properties of the program.
   • For example, if S is a child class of T, then we should be able to substitute T for S wherever it appears without breaking the code.
   
• Interface segregation principle
   • The use of the word interface here means all of the public methods associated with a class. Every instance of the class must have a valid implementation of these public methods, as clients of the class may depend on them. 
   • But no one should be forced to implement irrelevant methods in an interface!
   • It is therefore better to have lots of small, specific interfaces than a few larger ones; this makes the software easier to extend and modify.

• Dependency inversion principle
   • Reduce chains of dependence between classes so that you can change an individual piece without having to change anything more than the individual piece.
   • There are two aspects to the dependency inversion principle: High-level modules should not depend on low-level modules. Both should depend on abstractions.
   • Abstractions should not depend upon concrete details. Details should depend upon abstractions.



3.2 - CRC Modeling - (Class-Responsibility-Collaborator)
--------------------------
Online CRC Model Drawing: https://app.diagrams.net/


3.3 - UML - (Unified Modeling Language)
--------------------------
Online UML Drawing: https://app.diagrams.net/



3.4 - Design Pattern
--------------------------
Resource websites:
   • https://refactoring.guru/design-patterns
   • https://www.javatpoint.com/design-patterns-in-java#:~:text=Java Design Patterns,Builder Pattern Object Pool Pattern           
   • https://sourcemaking.com/design_patterns
   • https://www.tutorialspoint.com/design_pattern/index.htm





----------------------
4 - QA
----------------------
Test application

• Create Test Plan
• Write Test, and Check + Fix Bugs



----------------------
5 - UAT (user acceptance testing)
----------------------
Are we building the right product? Is our Customer satisfied?

• Ask Customer.
• Ask Ourself.

