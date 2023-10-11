# University Social Network ADR
# Date: October 11, 2023

## Summary
### Status
Proposed

### In the Context of Use Case: 
Our team has been tasked with the development of a social networking mobile app tailored for a university setting. This platform will serve as a hub for students to connect, share academic resources, keep abreast of events and club activities, and manage their academic schedules. Additionally, it will act as a portal for professors to disseminate announcements, assignments, and academic grades.
### Facing: 
The challenge lies in catering to a diverse user base that includes students and professors with varying levels of technological proficiency and device capabilities. The application must be universally accessible, secure, and provide consistent performance across different mobile platforms while ensuring data privacy and efficient offline access.
### Context:
The burgeoning need for a centralized platform in the academic arena has been evident. Universities require a cohesive system that bridges the communication gap between professors and students, fosters academic collaboration, and streamlines academic processes. Given the nature of a university environment, where students and professors are often on the move, an offline mode becomes paramount. Moreover, considering the wide variety of mobile devices used within a university, cross-platform compatibility is essential.
### We Decided For:
Application Type: Hybrid Application for both iOS and Android to maximize reach and ensure uniformity across platforms.
Framework: A cross-platform framework, potentially React Native or Flutter, for efficient development across both iOS and Android.
Offline Capabilities: Implementing local data caching and smart synchronization to ensure offline access and seamless data updates when online.
Performance Optimization: Adopting best practices for mobile development to ensure the app runs smoothly on both high-end and older devices.
Authentication: Integration with the university's Active Directory system to streamline the login process and ensure role-based access.
Notifications: A robust push notification system, compatible with both iOS and Android, to keep users updated about academic developments.
Security and Privacy: Implementing end-to-end encryption, secure APIs, and adhering to GDPR or other local data protection standards.
Accessibility: Ensuring the app is usable by everyone, including people with disabilities, by incorporating text-to-speech, high contrast modes, and other accessibility features.
### To achieve: 
Seamless integration with the university's existing systems, robust security, and a user-friendly experience that fosters collaboration and academic excellence.
### Accepting: 
Potential resistance to change from some university staff, initial learning curves for certain users, and the continuous need for updates and improvements based on user feedback.
## Discussion:
The academic landscape has evolved rapidly in the past decade. With advancements in technology and the increasing reliance on digital platforms, universities are under pressure to modernize and provide students and staff with tools that facilitate smoother interactions and efficient academic processes. The idea of a social networking app tailored for a university setting isn't new, but the requirements and expectations have changed. Besides, the application is designed to help students track their assignments' and exams' deadlines at their most convenience, keep their schedules up-to-date, store important information as well as financial documents, and utilize the application without internet connection.
### Issue Motivating the Decision:
There's a noticeable gap in communication and collaboration within universities. Traditional methods, such as emails and bulletin boards, are no longer sufficient. Students demand real-time updates, easy access to resources, and platforms that foster collaboration. Professors, on the other hand, require a platform where they can efficiently manage their courses, post assignments, and interact with students.
### Forces at Play:
Technical: The diverse range of devices and OS versions used within a university setting makes it challenging to develop an app that works seamlessly for everyone.
Political: Universities have established systems and protocols. Integrating with systems like Active Directory means navigating the existing political and administrative structures.
Social: The app needs to cater to a diverse user base with varied technological proficiency. It needs to be intuitive for both tech-savvy students and professors who might be more accustomed to traditional teaching methods.
Project: Timelines and resources are always a concern. The app development needs to be efficient, and the chosen technology stack should support rapid iterations and updates.
### The Problem We Aim to Resolve:
Our primary goal is to bridge the communication gap within the university. We aim to provide a platform that's not just a digital tool but an integral part of the university experience. It should facilitate academic processes, foster collaboration, and create a sense of community among students and staff.
## Decision:
### These are the decisions that we decided:
Application Type: We've opted for a hybrid application to provide a consistent experience across both major mobile platforms: iOS and Android. The hybrid application will ensure that users can access the internet; the device can access the app.
Framework: To streamline development and maintenance, our team chose a cross-platform framework. React Native and Flutter emerged as leading contenders given their wide adoption and support. With React Native, we ensure that this application is capable of compatibility enhancement and future maintenance purposes. With this modern framework, this application will always be up to date to catch up with UX/UI design trend and users’ behaviour.
Offline Capabilities: We decided to integrate local data caching mechanisms, ensuring users can access essential features even without internet connectivity. In order to ensure that users can access the app without the internet access, we will use SQLite to store data as SQLite is a one of the open-source database system encourage a full featured relational database.
Performance Optimization: Prioritizing performance optimization, we're committed to adopting best practices and tools that ensure a smooth app experience across a variety of devices. Java and Swift will be used to build the application as those programming languages’ popularity and large community supports.
Authentication: We'll integrate with the university's existing Active Directory system to leverage its secure authentication and role-based access mechanisms. Permission from school is required to access students' and faculties' credential information. As this application will allow students and faculties to log in the application by using their accounts, and programs and courses' content will be displayed on individual account.
Notifications: Recognizing the importance of timely academic updates, we've decided to integrate a comprehensive push notification system compatible with both iOS and Android platforms. As notification is one of the most important features of an application, notification feature will be enhanced with different functions and options which allow students to use it as their convenience. Necessary and important information will be designed to display to not disturbing students' lecture time or exam period.
Security: Beyond just adhering to data protection standards, our team is dedicated to implementing advanced encryption methods and secure transmission protocols to safeguard user data. Secure back-end language and data storage or cloud spaces are a sensitive case to keep an eye on since students' and faculties' account access to many credentials’ information. To ensure those requirements are met, code encryption is the area should be optimized and updated.
Accessibility: Inclusivity being a core value, we're ensuring the app design and features adhere to accessibility standards, catering to all users, including those with disabilities. UX/UI design should be optimized and up to date to make sure that people in different ages and with disabilities will be able to utilize the application conveniently.
## Consequences:
Hybrid Application Development: Opting for a hybrid application ensures a consistent user experience across both iOS and Android platforms. However, it might present challenges in accessing platform-specific features or optimizations.
Cross-platform Framework Choice: Using frameworks like React Native or Flutter facilitates efficient development across platforms, but there might be learning curves or platform-specific quirks to address.
Offline Capabilities: Supporting offline access enhances user experience, especially in areas with spotty internet. This requires robust data synchronization mechanisms which might increase the app's complexity.
Performance Optimization: Ensuring smooth performance on diverse devices is beneficial for user satisfaction. However, continuous testing on different devices and OS versions is crucial.
Active Directory Integration: Streamlined login processes and role-based access provide a secure and user-friendly environment. Nevertheless, any changes or updates in the Active Directory system might require app updates.
Push Notifications: Keeping users updated enhances engagement but requires a delicate balance to avoid notification fatigue. It's essential to ensure notifications are relevant and not overly frequent.
Security and Privacy: Implementing powerful security measures builds user trust. Compliance with data protection regulations is non-negotiable but demands continuous monitoring and potential updates as regulations evolve.
Accessibility Features: Incorporating accessibility ensures the app caters to all users, enhancing its reputation and user base. Continuous feedback from users with disabilities will be crucial to refine these features.
