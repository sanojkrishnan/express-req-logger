# loggerdet

A simple and flexible Express middleware that logs HTTP requests to the console and/or a file. Ideal for debugging, monitoring, and tracking incoming traffic in your Express.js apps.

---

## 📦 Installation

```bash
npm install loggerdet

## ✨ What This Module Provides

This package exports **two independent middleware functions** that you can use based on your logging needs:

### 1. `requestLogger(options)`

- Logs request details (method, URL, IP, timestamp) to the **console**
- Useful for quick development/debugging
- Example log:


### 2. `logLogger(options)`

- Logs the same request details into a **log file (`log.txt`)**
- Ideal for storing logs for audit or production
- File log output:


### Whats new!

### 2. `listener(options)`

- Listen port
- Give the port number you use and app object in express to activate
- Runs the port listening code for you



------------
You can use either one **or all together** in your Express app like this:

```js
const loggerdet = require("loggerdet");

app.use(loggerdet.requestLogger()); // for console
app.use(loggerdet.logLogger());     // for file logging
loggerdet.listener(app,3000);      // for port listening


## 🧑‍💻 Author

**SanojKrishnan M**

- 💼 MERN Stack Developer
- 🌐 [GitHub Profile](https://github.com/sanojkrishnan)
- 📧 Email: sanojkrishnan12@gmail.com