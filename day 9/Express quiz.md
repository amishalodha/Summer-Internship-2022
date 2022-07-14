# EXPRESS QUIZ

 Q 1  What is NodeJS?

 * Node.js is a cross-platform environment and library for running JavaScript applications which is used to create networking and server-side applications.

 Q 2 What is V8 Engine?
 * V8 is the JavaScript engine i.e. it parses and executes JavaScript code. The DOM, and the other Web Platform APIs (they all makeup runtime environment) are provided by the browser.

 Q 3 What is Event Loop in NodeJS.
 * An event loop is something that pulls stuff out of the queue and places it onto the function execution stack whenever the function stack becomes empty.

 Q 4 What is the use of tsconfig.json file?
 *  The tsconfig.json file specifies the root files and the compiler options required to compile the project.
 * By invoking tsc with no input files, in which case the compiler searches for the tsconfig.json file starting in the current directory and continuing up the parent directory chain.

 * By invoking tsc with no input files and a --project (or just -p) command line option that specifies the path of a directory containing a tsconfig.json file, or a path to a valid .json file containing the configurations.

 Q 5 What are the methods provided by `fs` module to manipulate files?
  * Node.js includes fs module to access physical file system. The fs module is responsible for all the asynchronous or synchronous file I/O operations.

    * fs.readFile(fileName [,options], callback)	Reads existing file.
    * fs.writeFile(filename, data[, options],      callback)	Writes to the file. If file exists then overwrite the content otherwise creates new file.
     * fs.open(path, flags[, mode], callback)	Opens file for reading or writing.
     * fs.rename(oldPath, newPath, callback)	Renames an existing file.
     * fs.chown(path, uid, gid, callback)	Asynchronous chown.
     * fs.stat(path, callback)	Returns fs.stat object which includes important file statistics.

Q 6 What is API?
*  API means a software code that can be accessed or executed. API is defined as a code that helps two different software’s to communicate and exchange data with each other.

Q7 What is JSON format?
* JSON stands for JavaScript Object Notation. JSON is often used when data is sent from a server to a web page.
```javascript
{
"employees":[
    {"firstName":"Anuj", "lastName":"jain"},
    {"firstName":"Aman", "lastName":"singh"},
    {"firstName":"Amar", "lastName":"joshi"}
]
}
```

Q 8 Why we use JSON format for API?
*  It reduces both the number of requests and the amount of data transmitted between clients and servers.

* JSON API inspects entity type and bundle to provide URLs to access each one of them using the standard HTTP methods, GET, POST, PATCH, and DELETE (we will discuss more on HTTP methods while talking about Document Structure).

Q 9 What is a Framework?
* Frameworks are typically associated with a specific programming language and are suited to different types of tasks.
   Other advantages include:

    * More secure code
     * Simpler testing and debugging
     * Avoiding duplicate code
    *  Clean and easily adaptable code

Q10 .How an HTTP Communication works.
* It is the protocol that allows web servers and browsers to exchange data over the web.
* It is a request response protocol.
 * It uses the reliable TCP connections by default on TCP port 80.
* It is stateless means each request is considered as the new request.

Q 10 What is Middleware in ExpressJS.
* Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next.

Middleware functions can perform the following tasks:

  * Execute any code.
   * Make changes to the request and the response objects.
  * End the request-response cycle.
   *  the next middleware function in the stack.