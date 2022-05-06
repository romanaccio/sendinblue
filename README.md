# Sendinblue hook

A basic server to handle events coming from the Sendinblue hook.
We expect sending blue to POST events at route/hook on port 3000,
where route is the url where were listening.

We are using ngrok to forward a real url to the localhost.

## how to

Initiate the repo once: yarn
in a terminal, run the server: yarn start
in another terminal, run ngrok: yarn tunnel
Copy the https route provided by ngrok and paste it in the hook config in Sendinblue pannel as:
route/hook, and save.
The server terminal will start displaying events as they are sent by Sendinblue.
