# env-cmd - React integration

<li>npx create-react-app app-name
<li>npm i env-cmd
<li>Create a .env-cmdrc file - define the environment specific config. For example, BASE_URL that changes based on env - QA,Prod,Dev.
<li>In React, prefix all env variables with 'REACT_APP_'
<li>Access the env variables using - process.env.REACT_APP_. For example, access 'REACT_APP_BASE_URL' using 'process.env.REACT_APP_BASE_URL'.
<br/>
<br/>
To select the env, modify the package.json scripts.
<br/>For example, 
<br/>
<br/>
 "scripts": {<br/>
    "start": "env-cmd -e dev react-scripts start",<br/>
    "build": "env-cmd -e dev react-scripts build",
    <br/>
    "start:prod": "env-cmd -e prod react-scripts start",<br/>
    "build:prod": "env-cmd -e prod react-scripts build",<br/>
    "start:qa": "env-cmd -e qa react-scripts start",<br/>
    "build:qa": "env-cmd -e qa react-scripts build",<br/>
    "test": "react-scripts test",
    "eject": "react-scripts eject"<br/>
  },

  To start react app with prod config, <br/>
  `npm run start:prod`