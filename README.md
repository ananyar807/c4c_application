# URL Shortener
Organization: Code 4 Commmunity 

Developer: Ananya Radhakrishnan

## Project Overview
This is a `React` web application that shortens long URLs into more manageable and shareable links. Users will be able to input any URL they would like, and the app will produce a shorter URL that redirects to the original URL. The back-end for this web application is through `Express` using REST routing and `SQLite` for persistent data storage. Front end and back end components were combined using the `axios` library. `Chakra UI` was used as the library for styling the front end user interface. 

## Structure
- `client`: React app providing the user interface. Contains the components used throughout the application, as well as styling and main pages with features. 
- `client2e`: Cypress project for end-to-end testing. 
- `server`: Provides the backend code for the application.

## Testing 
The express routes were initally tested using `Postman`, while the front end was tested using `Cypress`, an E2E testing framework. React components were also tested using `Jest` and the `React Testing Library`. Finally, the API was thoroughly tested using `supertest`, emulating HTTP requests to the Express router.

## Further Improvements
1. **Further abstraction of components**: Although right now there is only one page with components, later when generating many pages, it's important to break down repetitive features into components, and possibly organize them better, even by putting them in a components directory. 
2. **Further testing**: Using many testing libraries is great, but within each testing realm, there can always be more comprehensive testing, especially for each component in the front end, and each route in the back end. Later, when adding errors, we can also test for those as well. 
3. **Organization of File Heirarchy**: within each directory itself, such as client/src, the more components and files that get added, the more organized it should be. Directories should be made, such as components, styling, pages, etc. for better organization and usage for other programmers. This is also an enhancement, but adding comments is always helpful for documentation later on. 
4. **Error handling**: As this is an MVP, this wasn't added yet, but adding error handling and being able to render success/fail messsags in the front-end is important to test if the product is doing what we want it to be doing in all cases. 
