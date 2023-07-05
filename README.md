# URL Shortener
Organization: Code 4 Commmunity 

Developer: Ananya Radhakrishnan

## Project Overview
This is a `React` web application that shortens long URLs into more manageable and shareable links. Users will be able to input any URL they would like, and the app will produce a shorter URL that redirects to the original URL. The back-end for this web application is through `Express` using REST routing and `SQLite` for persistent data storage. Front end and back end components were combined using the `axios` library. `Chakra UI` was used as the library for styling the front end user interface. 

## Structure
- `client`: React app providing the user interface. Contains the components used throughout the application, as well as styling and main pages with features. 
- `client2e`: Cypress project for end-to-end testing. 
- `server`: Provides the backend code for the application.

![c4cap drawio](https://github.com/ananyar807/c4c_application/assets/76761180/b3453006-cbfb-4c5e-812e-6d91e97b59c9)


## Testing 
The express routes were initally tested using `Postman`, while the front end was tested using `Cypress`, an E2E testing framework. React components were also tested using `Jest` and the `React Testing Library`. Finally, the API was thoroughly tested using `supertest`, emulating HTTP requests to the Express router.

## Further Improvements
1. **Further abstraction of components**: Although right now there is only one page with components, later when generating many pages, it's important to break down repetitive features into components, and possibly organize them better, even by putting them in a components directory. 
2. **Further testing**: Using many testing libraries is great, but within each testing realm, there can always be more comprehensive testing, especially for each component in the front end, and each route in the back end. Later, when adding errors, we can also test for those as well.
3. **Error handling**: As this is an MVP, this wasn't added yet, but adding error handling and being able to render success/fail messsags in the front-end is important to test if the product is doing what we want it to be doing in all cases. This could also include input validation/output sanitization.
- I attempted input validation by using the `validator` package in node (Source: https://www.npmjs.com/package/validator )
- I also attemped output sanitization using `xss` package in node (Source: https://www.npmjs.com/package/xss) 
5. **Organization of File Heirarchy**: within each directory itself, such as client/src, the more components and files that get added, the more organized it should be. Directories should be made, such as components, styling, pages, etc. for better organization and usage for other programmers. This is also an enhancement, but adding comments is always helpful for documentation later on.
6. **Better Persistent Storage** : SQLLite was used as the persistent storage choice temporarily, and I would choose to use a different persistent storage. Depending on further features that will be implemented, I would choose MySQL or MongoDB. I've used MySQL when dealing with many entities and relationships as it organizes the data well, but MongoDB is helpful for large amounts of data. Depending on which would be helpful for URL Shortener, I would choose and reimplement the back-end. 
