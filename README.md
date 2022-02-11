# THE WIZZARD CHALLENGE

Recreate the basic, simplified functionality of a feature we developed for our CreativeEngine site called the "Wizard".
The Wizard fetches data about a video template - a <ins>template JSON object</ins>, collects project information from the user and builds a <ins>project JSON object</json>, which will later be used to customize and render the project.

## GOAL

The goal is to create a single page application (SPA) using Vue.js (https://vuejs.org/) and Axios (https://axios-http.com/). Both libraries are already being loaded into the index.html. Just open the.index html file in a browser.
Get the template information from an axios call to https://hoazygo0r9.execute-api.us-west-2.amazonaws.com/default/wizard-test and guide the user through steps to:

- first step
  - enter a project name
  - select a file format from the available outputOptions
  - enter display width and height
- second step
  - select one of the available color options
- third step:
  - fill out x number of text fields according to the numberOfTextFields value of the template JSON,
- Then submit and log out the result in a <ins>project JSON object</ins> with the following keys:

```
{
  "projectName": "MyProject",
  "templateId": <number>,
  "displayWidth": <number>,
  "displayHeight": <number>,
  "textFields": ["MyText1", "MyText2",...],
  "colors": "My Color Option",
  "output": "MyFileFormat"
}

```

To avoid confusion: do not manipulate the template JSON object but create a completely new JSON object that contains the project name, the template id and the project information collected in the form you built.

Assume that the template data will always have the same properties. But the number of text fields, color options and output options can change.

Use a similar design to the wizard-example-step1/2/3.png files and a stepwise entry of data. You can see design and functionality on the live site:

- go to https://ce.prismview.com/
- navigate to the library
- select one of the 2 free templates
- click customize to see the Wizard

You do not need to build everything you see on the site (no progress bar, social media file sizes etc.) only what's described here.
You can use the design as a basic layout idea, your view does not have to match the site. Feel free to be creative.

Make sure we can see your solution by just opening the html file in a browser or if you use a local development server, let us know how to start the project.

## DIRECTIONS

Feel free to change the file structur, create new files or add additional Javascript or CSS libraries. But build the components with Vue.js and make API calls with Axios.

Do not spend more than 4 hours on this. If you haven't finished, just submit what you have. If you have time left, think about improvements you could make to the UI or make it a properly set up node project (with package.json, git repo, gitignore file etc.)

You can either upload the solution to Github and share the link or zip the files and send them back via email.

Let us know if you have any questions.
