# Software Development Methodologies

- SDM = SDLC ( Software Development Lifecycle ) = Waterfall, Iterative , Agile ( Scrum )
- DevOps - Dev + Ops
    - Linux
    - SCM ( Software code manager )
    - Build tools
    - Deployment tools 
    - CI / CD

## Software Engineering

### Introduction

- **Software**
    - Software is more than just a program code.
    - A program is an executable code, which serves some computational purpose.    
    - Software is considered to be collection of executable programming code, associated libraries ( dependencies ) and documentations.
    - Software, when made for specific requirement is called software product.
- **Engineering**
    - All about developing products using well defined principles, methods and procedures.
    - Native Development
        - code 
            - Computational Logic (Executable + Dependencies )
    - Web Development 
        - Documentation
        - Dependencies
            - Resources
                - Images
                - Audios
                - Videos
            - Runtime (Optional)
            - Libraries
            - Frameworks
### What is Software Engineering ?
- Software Engineering is an engineering branch associated with the development of software product using well defined scientific principles, methods and procedures.
- The application of systematic, disciplined, quantifiable approach to the development, operation and maintenance of software.
- Establishment and use of sound engineering principles in order to obtain software that is reliable and work efficiently on real machines.
- The process of developing software product using software engineering principles and methods.

### Software Types 
- System software : Device Drivers
- Application software : Photoshop and calculator
- Engineering/Scientific Software : Auto-Cad, Catia
- Embedded Software : VLSI
- AI Software : ChatGPT, Gemini, Cloude
- Legacy Software : old application -> office suite 
- Web/Mobile Software : Websites and Mobile Applications

### Why Software engineering is important ?
- Helps to build complex systems in estimation or timely manner.
- Ensures high quality of software
- Imposes discipline to work
- Minimizes software cost.
- Decreases time

### Characteristics of good software
- A software product can be judged by what it offers (features) and how well it can be used (quality).
- Well-engineered and crafted software is expected to have the following characteristics : 
    - Operational
    - Transactional
    - Maintenance

#### Operational 
- This tells us how well software works in operations.
- Can be measured on :
    - **Budget** : Software should be developed within the budget.
    - **Usability** : Software should be usable by end user.
    - **Efficiently** : Software should efficiently use the storage and space.
    - **Correctness** : Software should provide all the functionalities correctly without having any bug/issues.
    - **Functionality** : Software should meet all the requirements of the user.
    - **Dependability** : Software should contain all the dependencies in its package.
    - **Security** : Software should keep the data safe from any external threat.
    - **Safety** : Software should not be hazardous or harmful to the environment.

- **Security**
    - Confidential : Confidential data must be confidential i.e should not be accessible i.e encrypted.
    - Integrity : Once data is stored in app, the original data can be retrieved by valid users of  system.
    - Availability : Application will always be available through scalability using horizontal scaling.
    - Authentication : Check if user is valid.
    - Authorization : Check if the authenticated user has enough permission using token.
#### Transactional
- This aspect is important when the software is moved from one platform to another.
- Can be measured on :
    - **Portability** : If the software is able to perform the same operations on different environments and platforms, that shows it Portability.
    - **Interoperability** : It is the ability of software to use information transparently.
    - **Reusability** : If on doing slight modification to the code of software, we can use it for different purpose, then it is reusable.
    - **Adaptability** : It is the ability to adapt the new changes in the environment.
        - Development environment
        - Staging environment     
        - Production environment

#### Maintenance
- Briefs about how well a software has the capabilities to maintain itself in the ever-changing environment.
- Can be measured on : 
    - **Maintainability** : The software should be easy to maintain by the any user.
    - **Flexibility** : The software should be flexible to any changes made to it.
    - **Extensibility** : There should not be any problem with the software on increasing the the number of functions performed by it.
    - **Testability** : It should be easy to test the software.
    - **Modularity** : A software is of high modularity if it can be divided into separate independent parts and can be modified and tested separately.
    - **Scalability** : The software should be easy to upgrade.
- Where, modularity means
    - functions
    - classes
    - modules - Collections of functions and classes.
- Scaling are of two types : 
    - Vertical Scaling 
        - Single point of failure
        - limit on resource
        - downtime is required
    - Horizontal Scaling 
        - No single point of failure
        - No limit on resources
        - No downtime
## Software Development Lifecycle - SDLC

### Overview 
- Also called as software development process.
- Is a well defined, structured sequence of stages in software engineering to develop the intended software product.
- Is a framework defining tasks at each step in the software development process.
- Aims to provide a high-quality software that :
    - meets or exceeds customer expectations
    - reaches completion within times and cost estimates.
- Consists of detailed plan (stages) of describing how to develop, test, deploy and maintain the software product.
    - Planning
    - Defining - Using SRS -> Software requirement specifications
    - Designing - Using DDS -> Design Document Specification
    - Building - Not well tested product
    - Testing - well tested product
    - Deployment - deployed app - end users
#### Planning and Requirement Analysis
- The most important and fundamental stage in SDLC.
- It is performed by the senior members of the team with inputs from the customer, the sales department, market surveys and domain experts in the industry.
- The information is then used to plan the basic project approach and to conduct product feasibility study in the operational, and technical areas.
- Planning for the quality assurance requirements and identification of risk associated with the project also done in the planning stage.
- The outcome of the technical feasibility study is to define the various technical approaches that can be followed to implement the project successfully with minimum risks.
#### Defining Requirements
- Once the requirement analysis is done the next step is to clearly define and document the product requirements and get them approved from the customer or the market analysts.
- This is done through an **SRS(Software requirements specification)** document which consists of all the product requirements to be designed and developed during the project lifecycle.
- SRS - Developers and Tester for test planning.

#### Designing the Product Architecture
- SRS is the reference of product architects to come out with the best architecture for the products to be developed.
- Based on the requirements specified in SRS, usually more than one design approach for the product architecture is proposed and documented in a DDS - Design Document Specification.
- This DDS is reviewed by all the important stakeholders ( stakeholders are those people who gets affected by application users, client and VC ) and based on various parameters as risk assessment, product robustness, design modularity, budget and time constraints, the best design approach is selected for the product.
- A design approach clearly defines all the architectural modules of the product along with its communication and data flow representation with the external and third party modules (if any).
- The internal design of all the modules of the proposed architecture should be clearly defined with the minutest details in the DDS.

- Architecture -> monolithic , microservices , peer-to-peer
- Designing -> Screen, Screen flow, database, UI/UX, architecture

#### Building or Developing the product - Not Well Tested Software
- In this stage of SDLC the actual development starts and the product is built.
- The programming code is generated as per the DDS during this stage.
- If the designed is performed in a detailed and organized manner, code generation can be accomplished without hassle.
- Developers must follow the coding guidelines defined by their organizations and programming tools like compilers, interpreters, debuggers etc are used to generate the code.
- Different programming languages such as C,C++, Java, PHP etc are used for coding.
- The programming language is chosen with respect the software being developed.

#### Testing the Product - Well tested Product
- This stage is usually the sub-set of all stages as in SDLC models.
- The testing activities are mostly involved in all stages of SDLC.
- However, the stage refers to the testing only stage of the product where products defects are reported, tracked, fixed and retested. Until the product reaches the quality standards defined in SRS.
- Testing
    - Types
        - Manual
        - Automation
    - Methods
        - Black Box
        - White Box
        - Gray Box
    - Levels 
        - Functional
        - Non-Functional
#### Deployment in Market and Maintenance - deployed app - end user
- Once the product is tested and ready to be deployed it is released formally in the appropriate market.
- Sometimes product deployment happens in stages as per the business strategy of that organization.
- The product may first be released in a limited segment and tested in the real business environment (UAT - User acceptance testing)
- Then based on the feedback, the product may be released as it is or with suggested enhancements in the targeting market segment.
- After the product is released in the market , its maintenance is done for the existing customer base.

## SDLC Models 
- There are various software development lifecycle models defined and designed which are followed during the software development process.
- Also referred as Software Development Process Models.
- Models 
    - Waterfall Model
    - Iterative Model
    - Spiral Model
    - V-Model
    - Big Bang Model
    - Agile Model -> DevOps 

### Waterfall Model
- Requirement Specification (Planning and Defining)
    - System Design (Designing)
        - Design Implementation (Building)
            - Verification & Testing (Testing)
                - System Deployment (Deployment)
                    - Software Maintenance (Deployment)
