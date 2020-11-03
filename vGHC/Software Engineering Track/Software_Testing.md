# Software Testing - Emerging Challenges in Industry
Emily Kowalczyk, Software Engineer, Apple; Sahana Gururaj, Engineering Manager, Apple

Modern software development is placing increasingly high demands on software testing. Not only is the software under test more complex (distributed and ML components), but the demand for instantaneous releases requires processes to be extremely efficient. In this talk, we outline new challenges faced by our team at Apple and provide a deep dive into the innovative techniques used to address them.


### Notes

* Only test what we changed; because that is where new errors can creep in; use static analysis to find what line are edited and then what tests need to be run
* Reduce test flakiness;
    * In distributed architecture, tests pass sometimes and fail sometimes without any code/test change
    * Take the test out or change the test to reduce flakiness; so that fail gives a strong indicator of actionable step that can be taken
* Test ML models; automate test and use oracle; test results seen in ‘defect space’; better than looking at coverage because never show what path test took
