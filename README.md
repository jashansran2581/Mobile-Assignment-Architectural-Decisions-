# Mobile-Assignment-Architectural-Decisions-
Hybrid App Architecture Decision Record (ADR)
1. Decision: Hybrid App (React Native)
Status: Accepted
2. Context: 
Sharing React Native code between iOS and Android devices cuts development time by a huge amount. Users are happier and more interested in the game because React Native works right. Perfect Active Directory integration makes sure that signup is safe, which increases the protection of data. Cross-platform push alerts let users know about important changes. 
3. Negative:
When you use frameworks like React Native for hybrid development, you need skilled developers and maintainers, and you might not be able to get all the advanced native features that are available in apps that are only native. It can be hard to work with mixed apps that run on multiple platforms and systems. To make sure they work well offline and sync your data, you should carefully set them up and try them many times.
4. Positive:
The fact that it works with apps on both iOS and Android devices makes it more appealing. This increases adoption and lowers the cost of creation. Users love how fast and useful it is compared to native apps. They stay interested because they get push notifications for changes. Having a single script makes it easier to add to and maintain designs. Adding Active Directory makes managing users and controlling access easier. Cutting down on data use and making apps run faster and better helps the user experience and device integration. 
5. Rationale: 
React Native efficiently fulfills university social networking needs with cross-platform compatibility for easy development. Integrating Active Directory ensures secure logins and widespread accessibility, making a mixed approach ideal for the college app project.



UI Framework Architecture Decision Record (ADR)
1. Decision: React Native
Status: Accepted
2. Context:
React Native is a strong system for cross-platform development that makes it easier to make and keep up-to-date apps for both iOS and Android, which saves time and makes sure everything is consistent. It gives users performance and functions that are similar to those of a native device, so they can use native device features that make their experience better. With a strong community and lots of tools, React Native makes it easier to solve problems and make things better. It lets you make user interfaces that are flexible, easy to use, and follow current UI/UX design principles. It also supports inclusive design with features like text-to-speech and high-contrast modes that make sure all users' needs are met.
3. Negative:
It's hard for new developers to get good at React Native because it has a steep learning curve and high proficiency standards. Also, it doesn't let you customize as much as fully native development does, so you have to find other ways to add advanced UI/UX features.
4. Positive:
React Native is great for cross-platform development because it only needs one script, which cuts costs and speeds up time-to-market. It has almost the same speed and user experience as native, so the UI/UX is the same on all devices and users are happier. React Native is always changing and getting better thanks to its detailed documentation and busy developer community. It makes it easier to make responsive, user-friendly designs and lets you make quick changes using rapid prototyping. React Native makes sure that everyone can use apps by making them easy for everyone to use and giving everyone a sense of belonging through accessible UI design.
5. Rationale:
The university social networking app's goals are met by React Native, which provides a native-like experience and works on multiple platforms. React Native is the best choice for the app's UI structure because it has a helpful community and features that make it easy for anyone to use. It also fits with the project's goal for wide usage, even though there are some problems from time to time.


Backend Language Architecture Decision Record (ADR)
1. Decision: Node.js
Status: Accepted
2. Context:
As a result of its great ability to handle asynchronous tasks, Node.js is perfect for making real-time, quick, and scalable changes to the university app. Its huge collection of packages and tools makes it easier to combine different services, which speeds up development and release. Node.js has a lightweight execution engine and allows horizontal scaling, so it works well even when it's busy. The active Node.js community keeps the framework up to date with the latest best practices by providing a lot of documentation and help. Node.js also works well with Active Directory, which makes sure that users are authenticated safely and that only authorized people can view private university data. 
3. Negative:
It might be hard for developers who are new to asynchronous programming to get started with Node.js because they need to learn how it works. Also, Node.js only has one thread, so it might have problems scaling when doing jobs that use a lot of CPU power.
4. Positive:
Node.js is great at handling asynchronous tasks, which makes sure that changes and synchronization happen smoothly in real-time. It has a huge npm library with a lot of plugins that speed up development and encourage new ideas. Node.js keeps running at its best even as the number of users increases because it supports horizontal scaling and has a light load. A big and active group of developers shares knowledge and makes tools that are useful and keep things better. Node.js also works well with Active Directory, which lets you securely authenticate users and limit their access. 
5. Rationale:
The university social networking app should use Node.js as its backend language because it is good at handling asynchronous processes and integrating smoothly with other systems to ensure strong real-time updates and user authentication. This outweighs any possible downsides and makes sure the app is safe and useful. 
Permissions Architecture Decision Record (ADR)


1. Decision: Permissions for Location Tracking, Camera, and Storage
Status: Accepted
2. Context:
Giving the app access to track your location lets it use GPS for features that depend on your location and to make personalized suggestions. Giving the app access to your camera lets you read QR codes and make safe transactions inside the app. The file permission lets the app save settings in the user's files, which makes sure the user experience is smooth.
3. Negative:
People may not use an app if it asks for private permissions because they worry about their privacy and trust. Adding these permissions also needs code that is special to the platform, which makes the development process more difficult.
4. Positive:
Giving users access to rights makes apps more useful and encourages them to keep using them. Permissions for cameras and files make things safer and lower the chance of data breaches. Location tracking and camera access make the experience more tailored to each user, which makes them happier.
5. Rationale:
To enhance usefulness, security, and user experience, the app requires permissions for accessing the camera, tracking location, and storing data, enabling valuable features and interactions despite potential privacy concerns. Responsible and transparent use of permissions fosters personalized experiences, secure transactions, and seamless data storage, bolstering user trust and satisfaction.


Data Storage Architecture Decision Record (ADR)
1. Decision: NoSQL (MongoDB)
Status: Accepted
2. Context:
The flexible schema of MongoDB lets you use a lot of different data types, which makes it more adaptable. Its horizontal scalability makes sure that it is fast and quick, which makes it easier for applications to grow. Real-time data synchronization lets users see changing material right away, which makes the experience better.
3. Negative:
Understanding NoSQL ideas and mastering MongoDB's query language are both part of the learning curve for MongoDB, which could make development take longer. MongoDB also puts availability and split tolerance at the top of its list of priorities. This could lead to problems with consistency in the future, which means that application logic needs to be carefully designed to ensure data is always in sync. 
4. Positive:
The distributed design and horizontal scaling of MongoDB ensures high performance and scalability. This makes the best use of resources and cuts costs even as the amount of data and user traffic grows. NoSQL's schema-less method also makes its data modeling very flexible, so it can quickly adapt to changing user needs and application requirements without any downtime or complicated migrations. 
5. Rationale:
Using MongoDB, for the university's social networking mobile app gives it flexibility, scalability, and real-time data synchronization, which lets content be managed dynamically and user experiences be tailored to their needs. MongoDB's document-oriented design makes it easy to handle different types of data, ensuring responsive interactions, smooth data sync, and strong scalability to support future growth and changing user needs.


Additional Frameworks/Technology Stacks Architecture Decision Record (ADR)
1. Decision: Firebase for Real-Time Updates and Push Notifications
Status: Accepted
2. Context:
Firebase's real-time database makes it easy to sync content across devices, which makes it easier for students, teachers, and university staff to work together, especially when it comes to quickly updating events and plans. Firebase Cloud Messaging (FCM) also sends push alerts to app users, making sure that important updates and reminders are sent out on time. 
3. Negative:
Using Firebase could lock you into one seller, making it hard to switch to other backend solutions or cloud providers in the future. This means you'll need to plan carefully and handle any problems that come up.  
4. Positive:
Firebase's cloud-based technology ensures scalability and reliability, keeping speed and availability constant even when the network is busy or there are a lot of users. This makes it easier for apps to grow and meet messaging needs well. By hiding the details of infrastructure management, this cuts down on development costs and speeds up time-to-market.
5. Rationale:
Adding Firebase for real-time updates and push notifications to the university's social networking mobile app simplifies sharing and interacting, boosting cooperation and increasing user experience. Firebase's scalable and stable infrastructure, simple integration, and fast development process give students and teachers rapid updates. This lets the system evolve, helping developers work more effectively and communicate. 
