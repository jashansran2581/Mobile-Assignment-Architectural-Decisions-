# Mobile-Assignment-Architectural-Decisions-Hybrid App Architecture Decision Record (ADR)
1. Decision: Hybrid App (React Native)
Status: Accepted
2. Context: 
React Native helps in cutting down the time of writing code for two different platforms by using the same code on iOS and Android devices. The result of using the same code improves the cost-effectiveness of an app. Perfect Active Directory integration increases the protection of data by making sure that signup data is safe. Moreover, cross-platform push alerts let the users know about the important changes made in the app.
3. Negative:
While using React Native for hybrid app development, skilled developers and maintainers are needed which are difficult to find. Also, it's hard to work with an app that runs on multiple platforms and systems. Along with this, both platforms have different security checks and requirements which make it hard to made. Developers must carefully set up the code to work well offline and sync your data and they must test them multiple times on both platforms. 
4. Positive:
The fact that the app works on both iOS and Android, targets a huge audience. Having a single code base makes it easier to maintain and add new features because they don’t have to write two different codes for the same features. Besides this, users love how fast these apps are as compared to native apps. As discussed earlier, hybrid apps decrease the cost of creation and increase adoption. Adding Active Directory allows users to manage and control their apps easily. Cutting down on data use and making apps run faster and better helps the user experience and device integration. They stay interested because they get push notifications for changes.
5. Rationale: 
React Native efficiently fulfills university social networking needs with cross-platform compatibility. Integrating Active Directory ensures secure logins and widespread accessibility, which protect their data. A mixed approach  makes it ideal for the college app project.


UI Framework Architecture Decision Record (ADR)
1. Decision: React Native
Status: Accepted
2. Context:
React Native is a strong system for cross-platform development that makes it easier to make and keep up-to-date apps for both iOS and Android, which saves time and makes sure everything is consistent. It gives users performance and functions that are like those of a native device, so they can use native device features that make their experience better. React Native has a huge community and because of that, they have lots of tools, which makes it easier to solve problems and make things better. Moreover, it provides flexibility to users by adjusting UI/UX according to their preferences.  
3. Negative:
It's hard for new developers to get good at React Native because it has a steep learning curve and high proficiency standards. Also, it is not as flexible as a fully native-developed app, so users/developers must find other ways to customize and add advanced UI/UX features.
4. Positive:
React Native builds the app once, and runs it everywhere! This cuts costs and gets the app in everyone's hands faster. Plus, it feels just as smooth and familiar as a native app, keeping users happy. React Native is constantly improving with a helpful community and clear instructions. This translates to beautiful, responsive designs and the ability to test changes quickly. It's all about making the app accessible and inclusive for everyone on campus!
5. Rationale:
The university social networking app's goals are met by React Native, which provides a native-like experience and works on multiple platforms. React Native is the best choice for the app's UI structure because it has a helpful community and features that make it easy for anyone to use. It also fits with the project's goal for wide usage, even though there are some problems from time to time.


Backend Language Architecture Decision Record (ADR)
1. Decision: Node.js
Status: Accepted
2. Context:
As a result of its great ability to handle asynchronous tasks, Node.js is perfect for making real-time, quick, and scalable changes to the university app. Its huge collection of packages and tools makes it easier to combine different services, which speeds up development and release. Node.js has a lightweight execution engine and allows horizontal scaling, so it works well even when it's busy. The active Node.js community keeps the framework up to date with the latest best practices by providing a lot of documentation and help. Node.js also works well with Active Directory, which makes sure that users are authenticated safely and that only authorized people can view private university data. 
3. Negative:
Node.js might be trickier for beginner programmers because it handles things differently than usual. Also, it can struggle with super intense tasks that require a lot of processing power.
4. Positive:
Node.js rocks for the app! It handles real-time updates and user logins smoothly, even with tons of users. Plus, it has a massive toolbox of plugins and a supportive community to keep things running great. And, it works well with your existing security system for safe access.
5. Rationale:
Node.js is a great choice for the university app's backend! It excels at handling things happening at different times (asynchronous processes) and connecting seamlessly with other systems. This translates to smooth real-time updates, like seeing new posts right away, and secure user logins. While there might be some other options, Node.js offers a reliable and secure foundation for a user-friendly app.


Permissions Architecture Decision Record (ADR)
1. Decision: Permissions for Location Tracking, Camera, and Storage
Status: Accepted
2. Context:
For a smoother user experience, the university app might request permission to access your location, camera, and files. Location access allows features like GPS-based suggestions and nearby events. Camera access enables QR code scanning and secure in-app transactions. Finally, file permissions let the app save user settings for a personalized experience.
3. Negative:
People may not use an app if it asks for private permissions because they worry about their privacy and trust. Adding these permissions also needs code that is special to the platform, which makes the development process more difficult.
4. Positive:
MongoDB offers the university's social networking app flexibility, scalability, and real-time data sync. Permissions for cameras and files can actually make things safer. They ensure the app only accesses what it needs, reducing the risk of data breaches. This allows for dynamic content management and personalized user experiences. Its document-oriented structure makes handling different data types a breeze and ensures responsive interactions. The horizontal scaling ensures the app stays fast as user needs and data grow.
5. Rationale:
The university app might ask for access to your camera, location, and data storage. using the app to find study buddies nearby, share photos of campus events, or save important class materials for later. Trust is important. The app will be designed to use these permissions responsibly and transparently. This means only using the information it absolutely needs, keeping it secure, and giving you control over what's shared. This responsible approach builds trust and keeps everyone happy!


Data Storage Architecture Decision Record (ADR)
1. Decision: NoSQL (MongoDB)
Status: Accepted
2. Context:
MongoDB lets you store all sorts of data – text, photos, videos, anything! This makes the app adaptable to future needs and keeps things interesting. Plus, MongoDB is built for speed. Its horizontal scaling means it can easily grow alongside the university. Everyone sees updates instantly. Real-time data sync keeps students, teachers, and staff on the same page.
3. Negative:
Learning MongoDB takes some effort. You'll need to wrap your head around NoSQL concepts and master its query language. This can add some time to development initially. Another thing to consider is that MongoDB prioritizes availability over strict consistency. While this keeps the app up and running smoothly, it might require careful application design to guarantee data always stays perfectly in sync across all parts of the system.
4. Positive:
It spreads data across multiple servers, so the app can handle tons of users and data without slowing down. This keeps everything running smoothly and saves money because you're only using the resources you need. Unlike other databases, it doesn't require a strict structure for your data. This flexibility lets the app easily adapt to new features and user needs without any shutdowns or complex upgrades.
5. Rationale:
MongoDB offers the university's social networking app flexibility and smooth scaling. This means the app can easily adapt to changing needs and user growth. Its real-time data sync keeps everyone on the same page, allowing for dynamic content management and personalized user experiences. MongoDB's unique document-oriented structure makes it a breeze to handle all sorts of data, ensuring responsive interactions and a foundation that can grow alongside the university community.


Additional Frameworks/Technology Stacks Architecture Decision Record (ADR)
1. Decision: Firebase for Real-Time Updates and Push Notifications
Status: Accepted
2. Context:
Firebase's real-time database acts like a shared online document that updates instantly for everyone using the app. This makes collaboration between students, teachers, and university staff a breeze. Imagine everyone seeing changes to events and plans happening simultaneously! This ensures that important updates and reminders reach everyone on time, keeping everyone in the loop. 
3. Negative:
Using Firebase might make it tricky to switch to different cloud storage or app-building services later on. This means you gotta think carefully before diving in, and be ready to tackle any bumps in the road if you ever want to switch providers.
4. Positive:
Imagine the university app as a bustling online hub for students, teachers, and staff. Now picture a giant, super-powered computer working tirelessly behind the scenes. That's Firebase in action! This amazing tech takes care of all the complicated nuts and bolts, keeping everything running smoothly no matter how many people are using the app at once. It's like having a personal tech wizard ensuring information flies back and forth without a hitch. But that's not all! Firebase also acts as a translator, hiding all the confusing tech jargon that developers usually have to wrestle with. This saves them tons of time and lets them focus on what truly matters: building the coolest features and functionalities for the app. In short, Firebase acts as a tireless behind-the-scenes partner, making sure the app runs like a dream and gets into your hands as fast as possible!
5. Rationale:
Imagine the app as a giant message board where everyone sees updates instantly! That's what Firebase does. It makes communication between students, teachers, and staff a breeze. No more waiting for info to refresh – everyone's on the same page, all the time. This makes working together and staying connected way easier!
