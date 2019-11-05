# HTTP Server - Exercise #2

- Copy your server js file from the previous exercise over to this directory

- We now want to manage books data within our server
    - Create an array with at least three book objects
    - Each book object has an unique ID and a title
    - Create the array BEFORE the server is created

- Create a route /api/books
    - Serve the array of books on this route
    - Remember: The res.write and res.end methods only can send strings (and binary data), but not objects. You remember the JSON.stringify method, don't you?
    - Specify the right type of this content for the browser so it can interpret it correctly. The content type should be: application/json 

- Update the catch-all route
    - Sent back the status code 404
    - Test it in the browser 
        - Open the developer tools and select the tab "Network"
        - Open the route /test
        - You should see a red entry with the code 404

- Update the route /books
- This route should create and display an HTML list of all our book titles below our heading
- Loop through all books in the array and generate the corresponding HTML tags
