# Week 9: Session 2

This session is about setting up restful api's through express. And oh my there is a lot to take in. It is intended as a continuation of last session where this time 
we are setting up our server and creating http requests which is then tested through a program called 'Postman'. The first thing to look at is what is a restful API?

From what I understand, a restful API is a the use of the applications programming interface to send and receive data through http requests and responses, and change the state of this data. AS part of todays code we used GET and POST quite a bit. This was here we either put out a request for certain data from our backend, i.e. database (GET) or sent data to it (SEND).

Below is an example of Get and Send from code used in class. In this a request is being sent to get the employee list or post data on a new employee depending on the decision of the user. If there is an error in the request the default option will show us that there was an error.

    if (urlEmployee.pathname == '/api/employees') {
        switch(req.method) {
            case 'GET':
                employeesList(req, res)
                break;
            case 'POST':
                addEmployee(req, res)
                break;
            default:
                errorRequest(req, res)
                break;
        }
    }

At the end of the session I dont feel that I completely understand what to do but as I continue to look into over the weekend I am hoping that this will change.
I think the problem is just the sheer volume of code that needs to be learned. As I mentioned in an earlier entry that I am slow to learn code but proficient 
when in it when I do and this is no exception. I believe I am going to have to sink quite a few hours into restful api's to understand them enough to use in my projects.


As a side note. I have just learned of a file type called .md which will enable me to format the text in my entries. This I will be doing to all past entries, creating 
headers, unordered lists, etc.