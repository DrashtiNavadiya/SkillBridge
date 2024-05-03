# Project Report Web Application
- _Date Created_: 09 April 2024
- _Last Modification Date_: 10 April 2024
- _Netlify URL_: <https://cs5709-group11.netlify.app/>
 
## Authors
- [Drashti Navadiya (B00948838)](drashti.navadiya@dal.ca)

### Steps to authenticate application
1. Open the deployment link: <https://cs5709-group11.netlify.app/>
2. Click on Login or Create a new user.
3. Enter credentials and continue.

## Features

The following are the features of our application

- User Management
- Messaging
- Content Feed
- Discussion Forums
- Job board
- Payment Gateway
- Advanced Networking and Connection
- User Dashboard
- Mentorship Program

## Deployment
### Frontend 
To deploy the project environment, We have used Netlify[12]. The steps we followed for the deployment are as follows[19]:

1. Mirrored our code into a private GitHub repository from GitLab.
2. Accessed our Netlify account using GitHub credentials.
3. Chose the repository to be deployed.
4. Set up the site configurations, including naming the site, among other settings.
5. Initiated the site deployment by clicking on the "Deploy site" button. The site went live in just a few minutes. Links to both the source code and the live site are provided above. 


### Backend
To deploy the project environment, We have used Render[13]. The steps we followed for the deployment are as follows[19]:

1. Mirrored our code into a private GitHub repository from GitLab.
2. Accessed our Render account using GitHub credentials.
3. Chose the repository to be deployed.
4. Set up the ci/cd configurations, including naming the site, and automated build with main branch.
5. Initiated the site deployment by clicking on the "Deploy site" button. The site went live in just a few minutes. Links to both the source code and the live site are provided above. 
 
## Testing

In the context of my application, the end-to-end tests & coding style tests which I went through are described below[19]:

1. Testing Responsiveness

- Test: Resize the browser window to different screen sizes or use a responsive design testing tool to emulate various devices.

- Expectation: Verify that the website layout and components adapt appropriately to different screen sizes, ensuring readability and usability across devices. Elements should resize, reposition, or hide as necessary.

2. API integrations

- Test: Test for various requests with and without data. Test with invalid values. Test through postman[6] with different data.

- Expectation: Verify that the backend apis give the appropriate response or error

3. Stripe integration

- Test with various test cards[7] and amounts. Test with saved cards and new cards.

- Expectation: User should be shown the error messages sent by stripe. User should be able to pay with new or saved cards. 

4. Form validations

- Test form with invalid or blank information

- Expectation: User is shown the right error messages to fix issues.

## Frontend Folder structure (Vite build) [19]
- frontend/src/assets/ - used for storing images
- frontend/src/components/ - used for react components. Each component has a folder with tsx and scss(if needed since most stying through mui)
- frontend/src/models/ - used for typescript interfaces
- frontend/src/pages - used for react pages. Each folder has one of more related pages
- frontend/src/stores - used for various mobx store class
- frontend/src/utils - for .ts helper functions

## Backend Folder structure [19]
- backend/src/models/ - used for mongoose schemas
- backend/src/routes/ - used for individual route files
- backend/src/services/ - used for services to be used in the route files
- backend/src/utils/ - for .ts helper functions

## Local deployment
Below are the requirements and steps for both frontend and backend local deployment and testing. After cloning the repository, switch to either frontend or backend folder and follow the below instructions.

### Prerequisites

To have a local copy of this lab up and running on your local machine, you will first need to install the following software (environment).

```
Node.js version 18+
```

See the following section for detailed step-by-step instructions on how to install this software (environment).

### Installing

Download and Install Node.js for your Operating System from https://nodejs.org/en/download.

Test successful install by checking node version in Command Prompt/Terminal

```
node -v
```

Confirm if the version is the same as the one downloaded.

```
v20.11.0
```

### Deploying

Install the required dependencies

```
npm install
```

To run the development server use dev script

```
npm run dev
```
 
## References
 
[1] [Node.js](https://nodejs.org/en/download) - To provide the runtime environment and for Dependency Management. <br/>
[2] [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) - For installing and managing packages for the React app. <br/>
[3] [React](https://react.dev/learn/installation) - For building the user interface for the app. <br/>
[4] [Material-UI](https://mui.com/getting-started/installation/) - To improve the user interface (UI) of the application by using the UI components provided by   Material-UI. <br/>
[5] [Stripe](https://docs.stripe.com/) -  For quick and secure payment integration in the application <br/>
[6] [Stripe-testing](https://docs.stripe.com/testing) - For testing using test cards <br/>
[7] [FontAwesome](https://fontawesome.com/start) -  For various icons and images <br/>
[8] [Postman](https://www.postman.com/downloads/) - Testing was done by using Postman. <br/>
[9] [VisualStudio-code](https://code.visualstudio.com/docs) - lightweight but powerful source code editor. <br/>
[10] [StickPng](https://www.stickpng.com/img/icons-logos-emojis/iconic-brands/visa-logo) - Visa logo for payments and cards <br/>
[11] [MasterCard](https://brand.mastercard.com/debit/mastercard-brand-mark/downloads.html) - Downloadable logo for mastercard <br/>
[12] [Netlify](https://docs.netlify.com/) - Platform to deploy react application <br/>
[13] [Render](https://docs.render.com/) - Platform to deploy backend node application <br/>
[14] [MobX](https://mobx.js.org/README.html) - Simple, scalable state management. <br/>
[15] [PaginateMongo-Stackoverflow](https://stackoverflow.com/questions/5539955/how-to-paginate-with-mongoose-in-node-js) - ReferencedSolution for paginating data from mongo <br/>
[16] [StripeElement-Styling-LinkedIn](https://www.linkedin.com/pulse/stripe-custom-styled-card-elements-tanjir-antu/) - Referenced solution for styling stripe elements <br />
[17] [Combining-stores-DevCommunity](https://dev.to/cakasuma/using-mobx-hooks-with-multiple-stores-in-react-3dk4 ) - Referenced for combining various stores in mobx <br/>
[18] [Axios](https://axios-http.com/docs/api_intro) - Library used for making api calls to backend <br/>
