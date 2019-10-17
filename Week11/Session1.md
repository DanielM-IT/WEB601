# Week 11: Session 1

With the milestone 2 due date being so near the class focus is solely on assessment work. But it is being done in the best way; peer coding. This is where a person will help another to code but completely hands off. The aid is only through advice. This I consider to be one of the best learnign methods as it is one thing to be able to do something myself but to guide someone else requires a new level of understanding. Peer coding is one way of rapidly boosting ones rate of learning.
My time in class consisted of two things. The first is helping Milton with his project through peer coding and the second was in between helping Milton, working to complete my own project. 
At the beginning of class I have a working POST and GET request but have been unable to get DELETE working as of yet. It me some time but I have managed ot pin down where my issue with DELETE is. I had set up my front end properly and even my request but my middle wear had an issue. The below code now passes the id through 'SongId'. However, before I simply had 'id' which was my issue. Having the wrong name for passing my id completely prevented any communication between my front and back end.

function checkID(req, res, next) {
    const SongId = +req.params.SongId

    if (Number.isInteger(SongId)) {
        next() 
    } else {
        return res.status(400).json('ID must be an integer'); 
    }
}

module.exports = {
    checkID
}


I had one other error appearing in my console when inspecting a page. 

Uncaught TypeError: Cannot use 'in' operator to search for 'default' in undefined
    at react-router-dom.min.js:1
    at react-router-dom.min.js:1
    at react-router-dom.min.js:1

The above error I eventually discovered was caused by havoing this script in my 'index.html' head.

<script src="https://unpkg.com/react-router-dom/umd/react-router-dom.min.js"></script>

This is not needed due to already having installed it as an npm package.