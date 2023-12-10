**STUDY GUIDE – cpsc349 – Fall 2023** 

**You should be able to answer any of the questions from these**  

- Quiz: Intro to NodeJS 
- Quiz on chs. 16/17/18 – ES6, Babel, and chattrbox 

**Chapters covered** 

The first part of the final exam will be based on the following chapters from our Front-end Web Programming textbook.  

- Chapter 15 (Introduction to Node.js) 
- Chapter 16 (Real Time Communication with WebSockets) 
- Chapter 17 (Using ES6 with Babel) 
- Chapter 18 (ES6, The Adventure Continues)  

**Chattrbox\_ project** 

You should thoroughly understand the code in the Chattrbox project, and be able to make modifications or extensions to it. 

**Example questions** 

Be able to answer any of the following questions… 

- Using Node you can create anything… 
    From command line tools to web servers

- With Node, the Javascript engine can communicate to… 
    WebSockets

- Know the difference between node start and node run dev 
    npm run dev runs a specific script it also requires run because it's a custom script which would be npm start

- Knowing how npm installs locally and globally, and what the default behavior is 


- Know how to import files into Node.js using import and require, and how to export them. 
    require loads in the the path to the file we want
    var extract = require('./extract');



    exports function called extractFilePath
    module.exports = extractFilePath;

- Know how Node can handle errors. 

    look at index.js at line 8-10, and 19-22 for the answer

- Know how to test and run the chat server using wscat 

    Run two terminal windows, one should do npm run dev and the other should run wscat -c ws://localhost:3001

    In the second terminal window, enter some text at the prompt. Each time you type some text and press the Return key, your text will be repeated by the WebSockets server


- Understand how the simple chat server runs when receiving and broadcasting messages, and how to launch it and connect to it. 



- Understand how Java objects are created, stringified, and parsed. 



- Be familiar with the features of ES6** that are supported by Chrome, Firefox, Safari, and Edge.

The self update without the need to manually do it,

- Know how to create and handle promises. 
- Know how babel handles errors it finds, and what it displays if there are none. 
- Understand how local storage and session storage work. 
- Know when React renders, and the states in the React life cycle. 
- Understand the different package managers available or Node.js 
- Understand how to use props and state in React, and which is preferrable. 
- What is the advantage of using React? Why is it so popular? Who created it? 
- What is the architecture of the Chattrbox application?  
- What are the modules and what are their purposes?  
- Could you modify them if needed to add functionality? 

**CODING QUESTIONS:** 

You will have to be able to code ONE of the following questions (from the challenge questions in our textbook) 

**CHOICE A:** In the ws-client module, add another function called registerCloseHandler. It should take a callback that is invoked when the close event is triggered on the socket. 

In main.js, use registerCloseHandler to alert the user that the connection is closed. Then, test it to make sure it works. 

How can you test it? Obviously, you cannot close the browser window. You will need to close the other end of the connection. 

For an added bonus, write a function that attempts to reconnect. You can either use a setTimeout or you can prompt the user for confirmation (search the MDN for details). 

OR 

**CHOICE B**: If you are in the middle of a chat and need to reload the browser, all of your messages disappear. It is nice that your UserStore remembers your username – but it would be better if you also had a similar mechanism for caching chat messages. 

Create a MessageStore that subclasses Store. It should store messages as they come in, making sure not to store the same message more than once. 

When the page loads, Chattrbox should get any cached messages from MessageStore. Decide if you would like messages to persist even if the browser tab is closed and re-opened. (If so, what alternative to sessionStorage would you use?) 
*Study guide – cpsc349 – Fall 2023*  2 ![](Aspose.Words.a927465c-dc03-4c78-8ce5-12a1c49c9c41.001.png)
