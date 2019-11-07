# Week 14: Session 2

This session our tutor has provided two example repositories as guides for us in implementing login in our applications. At first there were a lot of issues cropping up for us who are windows users; mostly with react-scripts.
The command which fixed this issue was 'npm i -g react-scripts@latest' or for some of us 'npm i react-scripts --save'. 
This fix fixed the react scripts issue and allowed the two applications to run. One still had issues after this and this was caused by a line of code calling a location reload and an import which wasn't being used. Following commenting out these two code lines I now have both login applications working.
These two login applications I will be reverse engineering over the weekend, seeking to understand how they work so I can complete the account login on my Music application.