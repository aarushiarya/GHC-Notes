# Are You Happy? Data Driven Assessment of User Satisfaction in Voice Assistants
Chelsea Miller, Data Analyst, Cisco Systems Inc.; Maryam Tabatabaeian, Data Scientist, Cisco Systems Inc.

Voice interaction could be the medium of the future in a post-COVID, touch-free world. We offer a framework to evaluate the happiness of users as they interact with voice assistants. Using real data from Cisco Webex Assistant, we'll discuss what a conversation is and how we capture something as subjective as feelings. Join us to hear how we built & validated a data-driven user satisfaction system.

### Notes

* Cisco webex assistant
    * First commercial voice assistant
* Why is evaluating voice assistants so hard?
    * Measure satisfaction with AI
        * AI is probabilistic - not determinstic
        * Input is variable - Natural language is variable
        * Satisfaction is subjective
    * Previous research
    * Accuracy based- if system performs with accuracy equal to satisfaction
        * Problem - based on single occurrence rather than whole conversation
    * User studies- artificial lab setting, not scalable, no real time analysis
    * How we analyze interactions? 
    * New approach - automatic, conversational, scalable, real time
        * Analyze - previous data
        * Classify - how conversations end
        * Assign - classify data
        * What is a conversation? 
            * Initiated interaction
            * Single or multi-turn
            * One conversational goal
        * Capture a conversation 
            * Make a call - trigger
                * Who should I call
            * John
                * Okay calling John
        * Track the whole conversation with an id
        * Conversation end state
            * Fulfilled - goal achieved
            * Exited - user exit the conversation
            * Error - assistant failed to fulfill the goal
            * Modified - goal is same, but modified who to call
        * User satisfaction label
            * Happy - fulfilled
            * Sad - end in error or exit
            * Friction - has a lot of nuance, a lot of friction happening
                * User wants to call room
                * But company doesn’t allow calling rooms
        * 3000 user interaction conversation - labelled data
            * Track satisfaction of each feature
        * Find areas where user is not satisfied
            * Where is it happening?
                * Countries with non native speakers
                * Webex can’t understand
                * Identify and investigate issues
* What do humans think?
    * Human re-evaluate this data
    * Gave sample of interaction and asked to label conversations - happy, sad or friction
    * Compare output of algorithm with human label output
