# Using Open Source to Solve Customer Identity Authorization
Chandana Pavuluru, software manager, Intuit;
Snezana Sahter, Distinguished Software Architect, Intuit;

Authorization is a challenge in Identity & Access Management, for business or consumer use cases. Just debating attribute vs. role-based access will give you a headache and not to mention policy points: decision, enforcement, information. We will share how our globally distributed team decided to use an open source for AuthZ, while testing assumptions how open the open source communities are.

### Notes

* Problem
    * App - customer tries to do an operation - gets access or gets denied to resources
    * Resource can be sensitive information like SSN and documents like tax docs
    * Who is allowed to edit / who is allowed to view?
    * Authorization problem
        * User u wants to access resource R to perform action A, in context C in environment E
        * Grant access or not?
    * Where to enforce access decision?
        * Enable flexible policies
        * Never permit malicious user / never deny genuine user
        * Respond fast when decision is to permit
        * Attribute based access control
            * Application -> policy enforcement point -> policy decision point <->policy information point <-> attribute store
            * Create policy -> (store policy) Policy Repository  ->(Deploy policy) Policy decision point
            * Called XACML architecture

* Open Source - OPA
    * Generic policy engine
    * Flexibility to write complex policies
    * Treat policy as code to test integration with the code
* Integrate with OPA
    * Build negotiation on top of OPA
* Drive adoption
    * Start with training workshops
    * Collaborate with OPA
    * Deliver first use case within platform
* Spread goodness
    * Enhance self-service tools and processes
    * Standardize policy writing
    * Manage prioritized backlog of new ask
