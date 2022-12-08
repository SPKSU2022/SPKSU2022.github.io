---
layout: page
title: Backend
permalink: ./backend
---

## Backend

Amazon Web Services’ provided modules have an integral ability to work congruently with each other, granted implementation is successful. This meant ensuring that with the proper calls, users could easily undergo changes to the RDS without having to switch between contexts within the Dart app. With the AWS properly integrated, CompChores development team were able to mitigate the number of listeners, both active and passive, that were present. Fortunately, the development team was successful in supporting each service into the program after recognizing how each component could effectively be integrated. What this allowed us to achieve was an ability to essentially create an intricate highway to and from the RDS without compromising the users experience.
Login especially saw significant amelioration with the Amplify API allowing all the general abilities of conventional login modules to be inserted all from a single package. Function calls were sent through the AWS API Gateway, and the application was able to use Lambda to efficiently communicate database calls. Future prospects to the project were the use of S3 Bucket to provide further media enhancement support for the application. This sort of plug and play approach to CompChores meant that backend operations could be rapidly deployed and updated as fast as a programmer could come to understand how and where to utilize this. CompChores thus enhanced it’s scalability potential, as the tier system with AWS could be adaptive to the demands of fluctuating number of users. Should the RDS demand more, CompChores could update a tier and without any time sacrifice be just as operational ready as before. These autonomous modules also had their own development cycles internally, meaning as the modules themselves were enhanced, so too could the capabilities of CompChores. Granted, this would require a keen monitoring of development schedules and efficient management of utilized modules, with the ever present risk of syntax modification and their dependencies.


[back](index.markdown)
