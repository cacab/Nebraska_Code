# Nebraska.Code() 2023 Keynote Speech 

<img width="1147" alt="Screenshot 2023-07-23 at 12 04 41 PM" src="https://github.com/cacab/Nebraska_Code/assets/46205451/3b5caba7-6de2-4278-b85b-92b21f4e9aa4">

On 07/20/2023 I had the honor of kicking off Nebraska.code() as the first keynote speaker of the week. Below is a synopsis of my talk and my slides can be found [here](https://github.com/cacab/Nebraska_Code/blob/main/Nebraska_Code.pdf). 

## Description / Abstract:
Attendees will leave with a complete understanding of how open-source works and how to maintain and contribute to open-source projects. This talk is of value to open-source maintainers and contributors or anyone interested in contributing to an open-source project.

This talk will use a real-life example of a contribution I made to osquery.

### Details:
Why is open-source important?
Open-source projects encourage innovation through collaboration. As we know, when multiple developers from different backgrounds work together, we are more likely to see robust and reliable results. Open-source projects allow us to build on ideas and projects we wouldn’t otherwise have access to. They also allow us to collaborate with others who we wouldn’t normally cross paths with. These aspects of open-source have the potential to create a strong, organized community. These aspects also have the potential to create a disorganized and weak community as well.

#### Why is contributing to open-source important?
The open-source movement aims to use and iterate on reliable frameworks and software. Essentially, we want to provide high-value tools for other developers to iterate on and use. Therefore, open-source communities need to put themselves in a position to support those interested in using and contributing to their projects.

#### What makes for a good open-source community?
Collaboration and culture
Strong and active open-source projects have one thing in common: their communities. More specifically, these projects rely on maintaining existing relationships with developers and recruiting new developers to use and contribute to their projects.

The importance of having a positive community culture associated with these projects cannot be understated. Slack and discord channels are great places to garner feedback and spark discussion among project maintainers and contributors. However, if these forums are not positive, it becomes more arduous to recruit new contributors and can alienate existing contributors. The value of the project itself has a strong impact on the community it serves, as well as the culture of the members who make up the community.

##### Collaboration and culture 
This is the "people" element and how the community of the project itself maintains relationships with existing developers, and also recruits and mentors other developers. A code of conduct is important in this context because it's vital to promote a positive culture with a set standard for developer interactions. In addtion setting this standard is a huge part of recruiting and retention. 

##### Technology and innovation
High-value projects provide innovative solutions to a given problem. High value projects also tend to use languages with a larger user base. Low-value projects not iterated upon frequently will present many challenges when it comes to recruiting as well as generating processes and documentation. On the other hand, high-value projects that are frequently used are naturally more collaborative, as they will often have larger communities and more members willing to contribute and answer questions.

##### Processes and vision
Having a core team, or group of maintainers to direct future initiatives and features is important. Issues organized within a given version control system need to be accessible and easy to self-assign. Documentation around workflows, testing, tooling and releases should be through and straightforward. Communities and decision-making processes should be outlined and readily available as well.

### My contribution success story
After being in my current position for over a year, I decided to make a contribution to osquery, which is an open-source framework upon which Kolide’s launcher agent runs on.

### What is osquery?
Created by engineers at facebook, osquery is an open-source framework that allows you to query endpoint devices. This framework provides insight into devices of all operating systems by allowing a user to write SQL queries to find information about a given system.

osquery is an operating system instrumentation framework for Windows, OS X (macOS), and Linux. The tools make low-level operating system analytics and monitoring both performant and intuitive. osquery exposes an operating system as a high-performance relational database. This allows you to write SQL queries to explore operating system data. With osquery, SQL tables represent abstract concepts such as running processes, loaded kernel modules, open network connections, browser plugins, hardware events or file hashes.

osquery has a core team, slack channel, extensive documentation and clear guidelines for creating and submitting pull requests.

### My contribution
After spending a brief amount of time scrolling through the open issues in the osquery repository, I settled upon one that had a request for making an addition to an existing table, the ‘video_info’ table associated with macOS. However, after some initial research into how this would be done, I decided it would be more straightforward to create a new table with the information requested in the Github issue at hand. This particular use-case would need to render information associated with any display associated with a given endpoint. Specifically, the user who filed the issue was looking for serial numbers and display ages.

I was able to follow the setup guide for osquery and set up my development environment quickly. Then I read over their guide for creating a new table, decided on a table name, and got to work. Not having much experience with objective C++, I was able to find numerous resources written by maintainers and members of the osquery community. One of which was this blog post.

I named my table ‘connected_displays’, and began fleshing out the data. After I felt confident with the new table I’d written and tested, I was again able to follow the documentation and format my code properly. I did run into some snags with getting my build to run once I added my tests, but after asking some questions in the osquery slack channel I received a nudge in the right direction and was back on my way.

When submitting my pull request, I again had numerous resources to fall back on, and I was able to search the slack channel to find a fix for some formatting errors that ended up getting flagged by the CI/CD pipeline. This is another good aspect of a strong and high-value open-source project, a contribution process with a happy path! Here is a screenshot of the end result.

## Conclusion
By having clear documentation in place and fostering a sense of ownership and positive culture within your open-source community, you are empowering maintainers and contributors alike. From this process I was not only able to learn how to write functions in objective C++, i was also able to make a contribution to the largest open-source cybersecurity project on Github.

It is because of these positive aspects associated with this particular project that I, along with many other contributors, are able to contribute efficiently and in a meaningful way.
