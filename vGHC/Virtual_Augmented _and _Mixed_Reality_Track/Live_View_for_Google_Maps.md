# Developing Live View for Google Maps: A Lesson in Working With Emerging Technologies
Rachel Inman, Staff UX Design Lead Google;
Wenli Zhao, Software Engineer Google;

### Notes
* Problem - users find it difficult to navigate while walking with a dot on 2d map
    * Which direction are you facing and which way you should move?
* Gps signal off by couple of blocks in urban surroundings
* Gps in phones impaired where tall building can block or reflect signal
* To calculate orientation of device - compass in phone - skewed by surrounding magnetic fields
* Human like approach 
    * Human navigating on foot
* Technology - Global localization = VPS + Street view + ML
    * Localization - identify position + orientation
        * Eg. Blue dot help you localize
    * Visual positioning surface + Machine Learning
        * Determines location of a device by imaginary rather than gps signals
        * VPS creates a map with images with known locations
            * Analyze for key visual features such as outline of buildings / bridges
            * VPS compares the map with images in the index
            * Matches visual features - high accuracy for devices’s location and orientation 
    * High quality data set of images with known locations from all over the world
        * Google street view
        * 170 billion images from 87 countries
* AR + Global localization gave users useful tech
* UX Design Challenges
    * Cities across the world are laid out differently - navigation is different
    * Eg New York City is orthogonal vs Tokyo is multidimensional; eg. Restaurant is at 8th floor of a building accessed by hidden elevator
    * Which way is my next turn? Which way should I start walking?
        * User research 
            * Different cities walked 100 miles with participants
            * Different age, tech familiarity, navigational skills
        * Many people struggled with map abstraction - hard to understand 2d map in context to what they see
        * AR place things in real world
        * Why not put blue line in real world, like on the maps?
            * People felt compelled to exactly walk on the blue line
            * Doesn’t fit well with localization quality
        * 120 prototype 
            * 3d particle to guide users
                * People hated it in user testing, want specificities, motion was distracting
            * Little bit 2d map with AR to give familiarity
                * Technical challenges bringing prototype to reality
                    * Prototype was stand alone apps - fast build times
                    * 3d development infrastructure 
                    * Add live view to google maps - 2 platform - android / IOS
                    * Develop 3 times
                        * Stand alone prototype
                        * Android 
                        * IOS
                    * Different challenges faced for each platform - different solution
                        * Difficult to stay consistent
                        * If new change proposed, difficult to make change
                        * Need to work closely with other platform team and UX team
    * Chicken or egg problem
        * Egg - Whether to wait for technology to evolve 
            * Slow and needs 10 sec to find location
            * UX design needs to account for those 10 sec of processing
        * Chicken - develop UX for user needs
            * Start developing for user needs
    * Solution 
        * Chicken + egg
        * Egg - revealed challenges, shaped foundation, improved tech
        * Chicken - early feedback, vision
    * How to incubate egg to become a chicken?
        * Prioritize recent times
        * Travel and navigation slowed down
        * More important to give new timing and opening hours of businesses 
    * Tap on blue dot
        * Click on live view - get high accuracy
        * If friend sharing location on pixel - live view points to them
        * Look at live view for the current location
