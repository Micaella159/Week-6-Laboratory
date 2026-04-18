# Week-6-Laboratory

## Checklist - Did You Complete?

- [/] index.html created with all elements
- [/] style.css created with styling
- [/] script.js has fetchUsers() function
- [/] Click button loads and displays users
- [/] Loading message shows while fetching
- [/] Error message shows if something fails
- [/] Button re-enables after loading

## Reflection 

1. What does `await` do? Why do we need it?
In this activity, I learned how asynchronous JavaScript works and how it helps us manage tasks like fetching data from an API. One of the most important concepts is the use of await. The await keyword is used inside an async function to pause the execution of code until a Promise is resolved. In my program, it is used when calling fetchUsers. This is necessary because fetching data from an API takes time, and without await, the code would continue running before the data is ready. This could lead to errors or empty results being displayed.
2. What happens if the API is down? How does our code handle that?
 Another important part of the program is handling what happens when the API fails or is unavailable. If the API is down, the fetch request will fail and throw an error. My code handles this situation using a try catch block. The try section contains the code that attempts to fetch and display the users. If something goes wrong during this process, the control is passed to the catch block. In the catch block, an error message is displayed to the user, informing them that the data could not be loaded, and the error is also logged in the console for debugging purposes. This ensures that the application does not crash and instead fails gracefully.
3. What's the difference between `try` and `catch`?
The difference between try and catch is that try is used to run code that might potentially cause an error, while catch is used to handle that error if it occurs. The try block is essentially an attempt to execute a set of instructions, and the catch block is the response when something goes wrong. Together, they make the application more stable and user-friendly by preventing unexpected crashes and providing proper error handling.
