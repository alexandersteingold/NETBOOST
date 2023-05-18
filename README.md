# NETBOOST

Abour Section

WITH THIS TOOL YOU CAN EXTRACT INSIDE URLS FROM ANY WEBSITE (MAXIMUM 100 URLS)
Technology Scope: NodeJS, Angular, MongoDB
Tool will accept only TOP Level Domain name for scrapping. Any URL from search box will be converted to this format by the default.

MongoDB Section
------------------------------------------------------------------------------------------------------------------------
1. MongoDB Database on remote MongoDB Atlas Server.
use it as is with available credentials settings provided by the default in the code

2. DB Contains 2 Tables/Documents:

WEBSITES - store top level domain from the search bar

ULRS - store extracted urls for requested domain with foreign key to WEBSITES

Server Side Section
-----------------------------------------------------------------------------------------------------------------------
1. API / CRAWLER build with NodeJS
2. Open NETBOOST/API directory with PowerShell/Command Prompt
3. Run npm install for node_modules dependencies installation
4. Run npm run dev command to start server
5. Expected response: Server started on port 3000. MongoDB Connected
6. API / CRAWLER Server works on http://localhost:3000/
7. All requests secured with passport.authenticate and with API-Key Header => API_KEY
8. As default crawler limited to the maximum 100 URLs from any domain
9. Available configuration settings in .env file
                            
PORT=3000
MONGODB_URI="mongodb+srv://admin:Y1SMDReqXGeGAbhT@netboost.2bczhys.mongodb.net/test?retryWrites=true&w=majority"
API_KEY="a5464fb5-0a77-4920-b135-50a078c05254"
MAX_URLS=100

Client Side Section
----------------------------------------------------------------------------------------------------------------------
1. Client interface build with Angular
2. Open NETBOOST/CLIENT directory with PowerShell/Command Prompt
3. Run npm install for node_modules dependencies installation
4. Run ng serve command to start server
5. Expected response: ** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ **
6. API / CRAWLER Server works on http://localhost:4200/
7. All requests secured with API-Key Header => apiKey
8. Available configuration settings in enviroments/enviroments.ts file
                            
apiKey: 'a5464fb5-0a77-4920-b135-50a078c05254'
                  
