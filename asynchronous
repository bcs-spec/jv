const fs = require("fs");
// 1. Create (write) a file asynchronously
fs.writeFile("demo.txt", "Hello from Node.js\n", (err) => {
 if (err) return console.log("Error creating file:", err.message);
 console.log("File created and written successfully.");
 // 2. Append data
 fs.appendFile("demo.txt", "This line is appended.\n", (err) => {
 if (err) return console.log("Error appending:", err.message);
 console.log("Data appended successfully.");
 // 3. Read the file
 fs.readFile("demo.txt", "utf8", (err, data) => {
 if (err) return console.log("Error reading file:", err.message);
 console.log("File contents:\n" + data);
 // 4. Rename the file
 fs.rename("demo.txt", "renamed.txt", (err) => {
 if (err) return console.log("Error renaming:", err.message);
 console.log("File renamed to renamed.txt");
 // 5. Delete the file
 fs.unlink("renamed.txt", (err) => {
 if (err) return console.log("Error deleting:", err.message);
 console.log("File deleted successfully.");
 });
 });
 });
 });
});
console.log("This line prints first - the fs calls are asynchronous!");
