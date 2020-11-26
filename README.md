# env-cmd - React integration

<li>npx create-react-app app-name
<li>npm i env-cmd
<li>Create a .env-cmdrc file - define the environment specific config. For example, BASE_URL that changes based on env - QA,Prod,Dev.
<li>In React, prefix all env variables with 'REACT_APP_'
<li>Access the env variables using - process.env.REACT_APP_. For example, access 'REACT_APP_BASE_URL' using 'process.env.REACT_APP_BASE_URL'.
