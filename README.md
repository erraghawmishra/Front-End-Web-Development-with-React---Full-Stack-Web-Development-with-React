# Full-Stack-Web-Development-with-React---Front-End-Web-Development-with-React
Full-Stack Web Development with React:- Front-End Web Development with React

<h2>Peer-graded Assignment: React Components</h2>

InstructionsMy submissionDiscussions
In this assignment you will add a new component to the React application to show the details of a selected dish. You will use the Card component and the Bootstrap unstyled list component to prepare the view for this new component.

Step-By-Step Assignment Instructions
less 
Objectives and Outcomes

In this assignment, you will continue to work with the React application that you have been developing in the exercises. You will add a new component named DishdetailComponent that will display the details of a selected dish. You will then design the view for the component using the card component. At the end of this assignment, you should have completed the following tasks:

Created a new DishdetailComponent and added it to your React application. 
Updated the view of the DishdetailComponent to display the details of the selected dish using an reactstrap card component.
Updated the view of the DishdetailComponent to display the list of comments about the dish using the Bootstrap unstyled list component.
Assignment Requirements

This assignment requires you to complete the following tasks. Detailed instructions for each task are given below. The picture of the completed web page included below indicates the location within the web page that will be updated by the three tasks.

Task 1

In this task you will be adding a new DishdetailComponent  to your React application and include the component into the menu component's view so that the details of a specific dish are displayed there:

Replace the card showing the selected dish in MenuComponent's view with the DishdetailComponent, and make sure to pass the selected dish information as props to the DishdetailComponent.
Create a new DishDetail class in a file named DishdetailComponent.js in the components folder
Export the DishDetail class from this file so that it can be imported in MenuComponent.js and used to construct the view of the selected dish.
Return a <div> from the render() function. This <div> should use the Bootstrap row class to position the content within the <div>. This div will display both the details of the dish in a Card and the list of comments side-by-side for medium to extra large screens, but will stack them for xs and sm screens.
The card should be enclosed inside a <div> appropriate Bootstrap column classes so that it occupies the entire 12 columns for the xs and sm screen sizes, and 5 columns for md screens and above. Also apply a class of m-1 to this div.
The comments should be enclosed in a <div> to which you apply appropriate column classes so that it occupies the entire 12 columns for the xs and sm screen sizes, and 5 columns for md screens and above. Also apply a class of m-1 to this div.
If the dish is null then you should return an empty <div>
Task 2

In this task you will be adding a card component to the DishdetailComponent view to display the details of the dish given above:

Implement a function named renderDish() that takes the dish as a parameter and returns the JSX code for laying out the details of the dish in a reactstrap Card. You have already seen this as part of the MenuComponent class in the exercise earlier.
Display the name of the dish as the Card title, and the description as the Card text.
Task 3

In this task you will use the comments that are included in the dish object above to display a list of the comments for the dish. Please use your JavaScript knowledge to recall how you would access an inner property in a JavaScript object that itself points to an array of JavaScript objects (comments). This task involves the following steps:

Implement a function named renderComments() that takes the comments array as a parameter and lays out each comment as shown in the image below. You should use the Bootstrap list-unstyled class on the list.
Each comment should be displayed on two lines, the first one showing the comment, and the second line showing the comment author's name and the date.
The comments should contain a <h4> header with the word "Comments".
Remember to enclose the header and comments inside a <div> before returning the JSX code. Otherwise React will not do the layout correctly.
If the comments are null, then you should return an empty <div>.


Review criteria
less 
Upon completion of the assignment, your submission will be reviewed based on the following criteria:

Task 1:

A new DishdetailComponent  has been added to your React application.
Included the DishDetail into your MenuComponent's view to show the selected dish.
Passing the selected dish as props to the DishDetail Component.
Used the appropriate Bootstrap classes to the card so that it occupies the entire row for xs and sm screen sizes, and 5 columns for md screens and above.
Used the appropriate Bootstrap classes to the div containing the list of comments so that it occupies the entire row for xs and sm screen sizes, and 5 columns for md screens and above.
Task 2:

Used the Card component to display the details of the dish.
Task 3:

Included a list of comments about the dish into the dishdetail view.
  
  <h2>Peer-graded Assignment: React Router and Single Page Applications</h2>
  
  In this assignment you will continue working with the React application by adding a new component named AboutComponent to serve up the details of the corporate leaders, and you will then integrate the AboutComponent into the single page application.

Step-By-Step Assignment Instructions
less 
Assignment Resources

AboutComponent.js
Objectives and Outcomes

At the end of this assignment, you should have completed the following tasks:

Integrated the AboutComponent given above into the single page application.
Added a new functional component named <RenderLeader> through the RenderLeader() function to AboutComponent.js that renders the details of a given leader using the reactstrap <Media> component.
Construct and render the list of leaders in the About Us page using the <RenderLeader> component implemented above.
Assignment Requirements

This assignment requires you to complete the following tasks. Detailed instructions for each task are given below. The picture of the completed web page included below indicates the location within the web page that will be updated by the three tasks.

Task 1

In this task you will be integrating the AboutComponent into the single page application:

First, download the AboutComponent.js given above and move it to the components folder, and
Update the MainComponent.js file to integrate the AboutComponent into the single page application. You should be able to navigate to the AboutComponent by clicking the links in the navigation bar and the footer.
Task 2

In this task you will implement a new functional component named <RenderLeader> through the RenderLeader() function:

The RenderLeader() function receives the details of a leader as its  parameter,
Implement RenderLeader() function to use the Leader information received as a parameter and render the leader information as shown in the screenshot below using the reactstrap <Media> component. Recall how we used the <Media> component in the first module to render the details of a dish in the MenuComponent.
This will make available the <RenderLeader> component for use within your AboutComponent.
Task 3

In this task you will use the <RenderLeader> component created in the previous task to render a list of leaders within your AboutComponent:

Update the leaders variable within the AboutComponent() function to make use of the <RenderLeader> component to render the list of leaders.

Review criteria
less 
Upon completion of the assignment, your submission will be reviewed based on the following criteria:

Task 1:

The AboutComponent.js file has been downloaded and integrated into our React application.
The React application has been appropriately updated to enable navigation to the About Us page of our application.
Task 2:

Implemented a new <RenderLeader> functional component in your application.
 Used the reactstrap <Media> component to render the details of a leader.
Task 3:

Updated the leaders variable within the AboutComponent() function to make use of the <RenderLeader> component to render the list of leaders.
  
  <h2>Peer-graded Assignment: React Forms and Redux</h2>
  
  In this assignment you will be updating the React application with a react-redux-form based local form and do the form validation in code.

Step-By-Step Assignment Instructions
less 
Assignment Overview

In this assignment you will update the DishdetailComponent.js to include a form and do the form validation in code. At the end of this assignment, you should have completed the following tasks to update the page:

Added a new class component named CommentForm to DishdetailComponent.js.
Provide a form to enable users to submit their comments
Validate the information entered by the users in the form
Assignment Requirements

Task 1

In this task you will add a new class component named CommentForm. You need to complete the following:

Add a new class component named CommentForm that will add a button to the view as shown in the image below.
When the button is clicked, it toggles a modal that will display the comment form.
The CommentForm component is used by the RenderComments function to display the button for toggling the modal.
Task 2

In this task you will construct the form for users to submit their comments as shown in the image below. You need to complete the following:

Set up the form as a local form using the react-redux-form with the three fields: author, rating and comment.
The rating field in the comment form is implemented using a select, the author is implemented using a text field, while the comment uses a textarea with six rows.
Task 3

In this task, you will enable form validation as shown in the images below. You need to complete the following:

The author field should at least be three characters long.
The author field should be less than or equal to 15 characters.
The user should be alerted by showing the invalid message displayed at the bottom of the field.


Review criteria
less 
Upon completion of the assignment, your submission will be reviewed based on the following criteria:

Task 1:

A CommentForm component is implemented that adds a button to the view, which when clicked will toggle a modal containing the form.
Task 2:

The form is set up with the three fields correctly.
A select is included in the form to enable users to submit the rating, a text field for author and a text area for the comment.
Task 3:

The author field is being properly validated. If incorrect, the user is alerted.
  
  <h2>Peer-graded Assignment: Redux, Client-Server Communication and Fetch</h2>
    
    In this assignment, you will update the web application to get data from the server to render the information corresponding to the leadership team of the company. In addition, you will handle the submission of the feedback form by posting the feedback to the server.

Step-By-Step Assignment Instructions
less 
Assignment Overview

At the end of this assignment, you should have completed the following:

Introduced new action types and action creators to support the fetching of the leaders information from the server and update the Redux store.
Updated the Home and the About component to render the information about the leaders using the downloaded data from the server
Add simple animations to the About component where the leaders information is displayed.
Enabled the users to submit feedback through the feedback form by creating a new feedback service that accepts the form data and uses Restangular to record their feedback on the server.
Assignment Requirements

Task 1

In this task, you will update the Redux actions and the Home and About components to use the data from the server for rendering the leader information:

Add new action types in ActionTypes.js to support the fetching of the leaders information from the server
Add new action creators in ActionCreators.js to enable the fetching of the leaders information from the server and update the Redux store
Update the code in leaders.js to respond to the dispatched Redux actions and update the Redux store and appropriately handle the loading and errors.
Update the code in MainComponent.js to fetch and use the leaders information.
Update HomeComponent.js to render the leader information.
Update AboutComponent.js to render the leaders information. You should handle the loading and error condition appropriately.
Task 2

In this task, you will enable the saving of the feedback data submitted using the feedback form in the Contact component. You will save the feedback form data submitted by the user to the server:

Implement a new action creator named postFeedback() that takes a Feedback object as a parameter and submits the feedback to the server using Fetch. Recall that the feedback data is accessible at http://localhost:3001/feedback on the json-server.
Update MainComponent.js to make the new dispatch method postFeedback() available to ContactComponent.
Update the ContactComponent.js to submit the form data using the postFeedback() method by passing the feedback form data.
Task 3

In this task you will use simple animation using react-animation-components to enable a staggered rendering of the list of leaders in AboutComponent:

Use the expand animation that we have already used earlier to judiciously apply animation to the various stages of the form submission.
Screenshots




Review criteria
less 
Your assignment will be assessed based on the following criteria:

Task 1

Appropriate action types and action creators have been added.
The Home component is correctly using the leader data, and handling any errors that might arise.
The About component is correctly using the leader data, and handling any errors that might arise.
Task 2

A new postFeedback() action creator is correctly implemented to post the feedback data to the server.
The Contact component has been correctly updated to use postFeedback() to post the form data to the server.
Task 3

Appropriate animation has been added to stagger the rendering of the leaders in the AboutComponent.
