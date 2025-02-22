---
layout: default
title: CS-499 ePortfolio Stephanie S. McClurkin
---

<h2 style="text-align: center;">Professional Self-Assessment</h2>

   My name is Stephanie McClurkin, and I have spent the last few years studying for my Bachelor of Science in Computer Science at Southern New Hampshire University. Unlike many in the field, I didn’t start with a programming background. My professional experience has been in healthcare, where I’ve worked as a CNA and currently work in dietary services. Despite always having an interest in technology, I was initially discouraged from pursuing it as a career. However, after years of working in retail and healthcare, my employer provided me with the opportunity to earn a degree, and I took the chance to study something I was truly interested in.

   I originally enrolled in Information Technology but quickly realized I was drawn to programming. My first coding course, IT-140 Intro to Scripting, was a big turning point. It reminded me of how much I enjoyed building small websites and interactive projects as a kid, and I knew I had found the right path. I switched to Computer Science and embraced the challenge of learning something completely new, in love with the creative potential of programming. During my coursework, I’ve explored software engineering, data structures, databases, and cybersecurity, gaining hands-on experience and discovering my strengths. While I didn’t take a traditional path into this field, I feel confident in my adaptability and problem-solving abilities - and my technical skills continue to grow each day. This capstone project and ePortfolio have helped me reflect on my progress and reinforced my professional goals.

   My ePortfolio shows how I’ve developed as a programmer through three major enhancements to my original CS-360 Mobile Architecture & Programming project, which started as a simple weight-tracking app. The first enhancement focused on software design and engineering, where I converted the project from Java to Kotlin to align with modern Android development standards. This improved code efficiency, readability, maintainability, and demonstrated my ability to work with multiple programming languages. The second enhancement focused on algorithms and data structures, where I developed a predictive weight trend algorithm that analyzed user data and estimated future trends. While I originally planned to visually display both recorded and predicted weight trends, technical constraints led me to prioritize refining the algorithm’s accuracy, leaving graph visualization for a future update. The third enhancement centered on databases and security, integrating Firebase authentication and Firestore, allowing users to securely log in and store weight data in the cloud. This improved the app by making it more compatible with multiple devices while strengthening security through authentication safeguards and Firestore security rules.

   Each of these enhancements pushed me outside my comfort zone, and I’m proud of how I researched, adapted, and implemented solutions independently. Looking at my work now, I see how much I’ve grown and know I can continue learning and tackling more complex challenges. The transition from Java to Kotlin is likely my strongest enhancement, but I am most excited about the Firebase integration because it was my first experience with cloud computing, and it significantly improved the functionality of the app for the user.

   Throughout this course, I’ve demonstrated my knowledge of several important learning outcomes in computer science. Collaboration is important, even when working alone, and it’s necessary to make sure code is well-documented and readable. I reviewed my work frequently, focusing on writing informative but concise comments to help future developers understand my approach. Communication is another key skill, and I worked to ensure my code review video and documentation were clear, professional, and easy to follow. I did my best to break my project down into simple explanations to make my process more accessible. Soft skills like communication are often understated in computer science, but I recognize their importance and will continue to refine them in my career.

  The predictive weight trend algorithm in my second enhancement tested my ability to design and evaluate complex computing solutions. This required handling fluctuating weight data, determining the best formula for estimating trends, and troubleshooting inconsistencies. A big challenge was trying to incorporate the predicted weight trend into the graph while maintaining data accuracy; despite my best efforts, the graph would never correctly display the predicted trend. After numerous attempts, I chose to focus on improving the algorithm itself, realizing that effective problem-solving sometimes means reassessing priorities. Security was also a major focus in my database enhancement. Implementing Firebase authentication and Firestore security rules ensured that only authorized users could access their weight history, reinforcing industry best practices for authentication and data protection.

   As I move forward, my primary career goal is to secure an entry-level role in software development or database management where I can continue learning and gaining hands-on experience. While I am open to different roles, I am particularly interested in software development, database management, and web or mobile development. I don’t expect to immediately land a high-level job, but I am focused on getting my foot in the door, gaining experience, and continuously improving my skills. My next steps include continued self-study, working on personal projects, and preparing for technical interviews through coding challenges and algorithm practice. This program has taught me that a career in computer science is a continuous learning process, and I look forward to growing in this field.

   Completing this capstone and developing my ePortfolio has been one of the most challenging and rewarding experiences of my academic journey. I started with little experience in computer science, but now I have a strong foundation in software development, algorithms, and databases. I’m proud of my growth and confident that the skills I’ve developed will help me succeed in the industry. While I still have much to learn, this project has shown me that I am capable of tackling challenges, problem-solving, and continuously improving as a developer. I am excited to apply everything I’ve learned as I take the next steps in my career.

---

<h2 style="text-align: center;">Original Project: CS-360 Weight Tracking App</h2>

My original weight-tracking application was developed during CS-360: Mobile Architecture & Programming. It was designed as a simple mobile app where users could log their weight daily, set personal weight goals, and track progress over time. The app used an SQLite database to store weight entries and displayed them in a RecyclerView list. It featured basic UI elements and SMS notifications to alert the user of basic milestones. 

While functional, the original version of the app had several limitations, including the lack of predictive analytics, cloud storage, and modern Android development practices. These limitations became the focus of my three enhancements, where I worked on code modernization, algorithmic improvements, and database integration to make the improve the app. You can view my original code in the main branch located at the link below.

**Original CS-360 Project Code (Located in Main Branch):**  
**[View Original Project Code on GitHub](https://github.com/smcclurkin0312/CS499weighttrackingapp)**  

---

<h2 style="text-align: center;">Enhancement 1: Software Design & Engineering</h2>

The first major enhancement I made to my weight-tracking app was converting the entire codebase from Java to Kotlin. This transition was necessary because Kotlin has become the preferred language for Android development due to its improved efficiency, null safety, and more concise syntax. By making this change, I modernized the project to align with industry best practices, making the code more maintainable, reducing boilerplate, and improving security. The conversion also allowed me to take advantage of Kotlin's built-in features, such as automatic resource management and null safety, to eliminate potential crashes and memory leaks. These improvements made the app more stable, scalable, and easier for future developers to work with.

#### Course Outcome 1: Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.

Even though I worked on this project independently, I made sure the code is easy to understand and maintain for anyone who might work on it in the future. This is important because it supports building software in a collaborative setting. One way I did this was by improving documentation with clearer comments, especially in DatabaseHelper.kt, where I added comments to clarify where the database handles user weight records and optimized SQLite queries. Adding clear and straightforward comments makes it easier for future developers to expand or modify the app without running into confusion or potential data issues. This ensures that future developers can quickly understand its functionality. Well-documented code is important for effective collaboration, making the app easier to maintain and grow.

Next, I also focused on making the code itself easier to read and manage. A good example of this is the getLatestWeight() function. In the original Java version, I had to manually open and close the database and cursor objects, which made the code longer and increased the likelihood of errors. With Kotlin, I simplified the code using the use function, which automatically handles resource management. This minimized the lines of code, reduced the risk of memory leaks, and made the function easier to maintain. These updates show that I can write clean, well-documented code that is easy to understand and build upon, an important skill in any collaborative development environment.

#### Course Outcome 4: Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for implementing solutions that deliver value and accomplish industry-specific goals.

The transition from Java to Kotlin wasn’t just about switching languages; it was a way to modernize the project and follow industry standards, which directly supports the fourth course outcome. Since Kotlin is the preferred language for Android development, making this change ensures my app stays compatible with future updates and best practices. It also makes the code easier to maintain and expand over time, which is especially important since Google is prioritizing Kotlin in Android libraries (Mehra, n.d.). One of the biggest ways this enhancement aligns with the fourth course outcome is through improving efficiency with Kotlin’s modern features. A great example is the getLatestWeight() function. In the original Java version, I had to manually open and close the database and cursor objects, which meant extra lines of code and a higher risk of errors. In Kotlin, I was able to simplify it using the use function, which automatically handles resource management. This means I don’t have to worry about manually closing database connections, making the function cleaner, easier to read, and safer to use.

![Improved Resource Management](https://raw.githubusercontent.com/smcclurkin0312/smcclurkin0312.github.io/refs/heads/main/assets/images/Code%20Screenshot%20Enhancement1%20Course%20Outcome%204.png)

The screenshot above shows exactly how Kotlin helped streamline the getLatestWeight() function. Kotlin takes care of managing resources, making the code more efficient and reducing the chances of memory leaks. This supports the fourth course outcome because it demonstrates how modern programming techniques can lead to a more maintainable piece of software. Writing clean and efficient code ensures the app runs better and is easier to work with.

Beyond converting the language from Java to Kotlin, I also updated the app’s dependencies and compile SDK to API level 35, ensuring compatibility with the latest Android development standards. This is important because it allows the app to take advantage of newer features, such as security improvements, and improves overall performance. This enhancement supports the fourth course outcome because it shows my ability to keep up with industry trends and ensure my app is using the best tools available.

#### Course Outcome 5: Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.

Security is a critical aspect of software development, and I made several improvements to ensure my app follows best practices and reduces potential vulnerabilities. One of the biggest changes I made was improving how user authentication data is handled to prevent crashes and unexpected behavior, which supports the fifth course outcome. Before converting the app to Kotlin, there was a security risk related to how authentication data was handled in MainActivity. If user authentication data wasn’t properly initialized, the app could crash with a NullPointerException, which is both a hassle for users and a security concern. With Kotlin, I was able to take advantage of **null safety features** to prevent this type of problem before it ever happens. Preventing crashes helps reduce unexpected behaviors that could later be exploited as potential security vulnerabilities.

![Enhanced Security with Null Safety](https://raw.githubusercontent.com/smcclurkin0312/smcclurkin0312.github.io/refs/heads/main/assets/images/Code%20Screenshot%20Enhancement1%20Course%20Outcome%205.png)

The screenshot above shows how I improved the way user authentication data is handled. The original Java version required manual null checks, meaning that if I forgot to check for null, the app could crash. Kotlin, however, provides built-in null safety, allowing the app to check automatically. If authentication data is missing, Kotlin defaults to a safe value instead of crashing. This change improves both security and app stability by reducing the chances of unexpected failures.

Additionally, I updated the app to API level 35, which ensures that it follows Google’s latest security standards. This update includes stricter permission handling, stronger encryption policies, and better data protection. By implementing these enhancements, I demonstrated my ability to develop software with a security mindset, anticipate potential vulnerabilities, and design features that help protect user data, fully satisfying the fifth course outcome.

---

**Enhancement One Project Code (Located in the Enhancement 3 Branch):**  
[View Updated Code on GitHub](https://github.com/smcclurkin0312/CS499weighttrackingapp/tree/enhancement3)

---

<h2 style="text-align: center;">Enhancement 2: Algorithms & Data Structures</h2>

The second major enhancement I made to my weight-tracking app was implementing a predictive weight trend algorithm to analyze past weight entries and estimate future weight trends. The original version of the app only allowed users to log their weight manually, without providing any insight into their progress over time. To improve this, I created an algorithm that calculates weekly weight changes and predicts future weight trends based on the user’s recorded data. These predictions are displayed in a dropdown menu, where users can select a timeframe of 1-4 weeks to estimate future weight changes.  

Next, I integrated MPAndroidChart to create dynamic visualizations for the recorded weight data. Instead of just listing weight entries, the enhancement displays weight trends in a graph, helping users quickly recognize patterns in their weight fluctuations. Although I originally planned to display both recorded and predicted weight trends on the graph, technical constraints led me to keep only recorded data visualized, while predictions remain text-based in the dropdown menu.

![Empty Weight Tracking Page (New User)](https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/new%20user%20empty%20weight%20screen.png?raw=true)

The screenshot above shows the weight-tracking page before any entries are logged. The enhancement allows users to manually input past weight values, improving the accuracy of predictions.

#### Course Outcome 2: Design, develop, and deliver professional-quality communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.

For this enhancement, I wanted to make sure that my implementation was not only functional but also well-documented and easy to follow. One way I did this was by improving code readability with structured comments and documentation, ensuring that future developers (or even my future self) could easily understand how the predictive weight trend feature works. I included clear comments in key areas, such as explaining how the algorithm processes past weight changes to predict future trends, how MPAndroidChart is used to visualize recorded weight trends, and how stored weight entries are retrieved and structured. This demonstrates my ability to write technically sound, professional-quality documentation that is clear and informative.

Beyond ensuring my code, comments, and technical documentation were well-structured, I also focused on making sure the user-facing side of this enhancement was clear and intuitive. I improved multiple features to make the interface more intuitive for the user, such as the calendar you see in the screenshot below. Since the prediction results needed to be easy to interpret, I decided to integrate MPAndroidChart to visually display recorded weight trends instead of just listing numbers. The prediction results themselves are provided in the drop-down as text-based calculations. The graph dynamically plots weight data with a clear x-axis for time and y-axis for weight, allowing users to quickly recognize patterns in their weight trends. This enhancement improves the app’s usability by making weight trends and predictions easier to understand at a glance, aligning with best practices in professional software development.

![Date Selection Calendar](https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/select%20a%20date%20calendar%20screenshot.png?raw=true)

#### Course Outcome 3: Design and evaluate computing solutions that solve a given problem using algorithmic principles and data structures.

The predictive weight trend algorithm is the centerpiece of this enhancement and it demonstrates my ability to design and evaluate computing solutions using algorithmic principles and structured data. This algorithm takes a user’s past weight entries and estimates future trends based on their recorded data. The prediction is based on averaging weight changes over time, which helps account for short-term fluctuations and provides a realistic trend line instead of a simple projection. To make sure the algorithm was efficient and scalable, I used sorted lists and dynamic data structures so that new weight entries could be processed quickly, without extra recalculations. This makes sure that calculations are performed only when necessary, which helps to keep the app responsive. The prediction logic focuses on actual progress rather than static assumptions, making the results both accurate and useful for the user. This demonstrates my ability to apply structured data principles to build efficient, real-world computing solutions.

The screenshot below show how MPAndroidChart is used to visually display recorded weight history. The prediction results, however, are presented as text-based calculations in the dropdown menu, allowing users to estimate their future weight based on their recorded data.

![Algorithm Implementation - Part 1](https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/Code%20Screenshot%20Enhancement2%20Course%20Outcome%203%20P1.png?raw=true)

By structuring the algorithm this way, I helped make sure that users receive realistic, data-driven predictions that adjust dynamically as they log new weight entries. Once the algorithm was in place, I checked its accuracy by testing it against both steady and fluctuating weight trends to make sure the predictions made sense and weren’t too rigid or too extreme. This testing process demonstrates my ability to analyze and refine algorithmic solutions to ensure they provide reliable results.
I also focused on making sure users could easily interpret their recorded weight trends by integrating MPAndroidChart to visually display their historical weight data. Instead of relying on plain numbers, users can now see a clear, interactive graph that plots both their historical weight data. This helps them quickly recognize patterns and adjust their goals accordingly. The first screenshot below shows how users are provided with a text prediction of their anticipated weight loss. The second screenshot shows the results of this prediction at 1 week, and how MPAndroidChart is used to visually display recorded weight data. This graph-based visualization ensures that users can see trends at a glance, making this feature functional and user-friendly.

![Algorithm Implementation - Part 2](https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/Code%20Screenshot%20Enhancement2%20Course%20Outcome%203%20P2.png?raw=true)

<img src="https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/estimated%20weight%20prediction%20and%20current%20weight%20graph.png?raw=true" alt="Weight Prediction Dropdown & Graph" width="600">

#### Course Outcome 4: Demonstrate an ability to use innovative techniques, skills, and tools in computing practices to implement computing solutions that accomplish industry-specific goals.

One of the biggest improvements in this enhancement was integrating MPAndroidChart to create a dynamic weight trend visualization. Instead of just displaying numbers in a list, this enhancement applies modern data visualization techniques to show recorded weight entries as a visual graph, making it easier for users to track their past progress over time. MPAndroidChart is commonly used in mobile apps for analytics and trend tracking, so adding it to my project directly demonstrates my ability to integrate professional-grade tools that align with industry expectations for mobile applications handling user data.

Another way I demonstrated industry-relevant skills was by adding manual date selection for weight entries. Instead of restricting users to logging their weight for the current date, they can now enter past weights, ensuring that the prediction model is working with the most complete dataset possible. This feature improves the accuracy and reliability of the predictions by allowing the algorithm to analyze a broader, user-controlled data range. It also promotes better data integrity, since users can correct mistakes or fill in missing entries, which is an important part of maintaining clean, structured datasets in professional applications. You can see an example of the filled out weight entry page in the screenshot below. By implementing these enhancements, I showed that I can use modern computing tools and best practices to improve both functionality and usability in mobile app development.

![Filled-Out Weight Page (Recorded Data Visualization)](https://github.com/smcclurkin0312/smcclurkin0312.github.io/blob/main/assets/images/filledout%20weight%20page%20screenshot.png?raw=true)

---

**Enhancement Two Project Code (Located in the Enhancement 3 Branch):**  
[View Updated Code on GitHub](https://github.com/smcclurkin0312/CS499weighttrackingapp/tree/enhancement3)

---

## Project Code
**[View My CS-499 Weight Tracking App on GitHub](https://github.com/smcclurkin0312/CS499weighttrackingapp)**
