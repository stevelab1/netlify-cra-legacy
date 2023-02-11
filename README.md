# Netlify-CRA-Legacy

## Description

A boilerplate for CI/CD with [Create React App (CRA)](https://github.com/facebook/create-react-app), Github Actions and Netlify using legacy versions of React. Useful if your project includes legacy dependencies.

## Usage

- fork repo
- import new repo into Netlify and deploy
- setup Github Actions and Netlify

  1. Generate a new personal access token in your Netlify account, labelling it `NETLIFY_AUTH_TOKEN`. At the time of writing this was done by navigating to:

     - User Settings > Applications > New Access Token

  2. Add the `NETLIFY_AUTH_TOKEN` to your _GitHub_ repo

     - Settings > Secrets
     - _Important_: You must name it `NETLIFY_AUTH_TOKEN`.

  3. Return to Netlify and navigate to your deployed site and copy its `Site ID`.
     - Settings > Site Information > App ID
  4. Add the App ID to GitHub with the name of `NETLIFY_SITE_ID`.

- modify `push.yml` to add `branches` or `jobs`
- `git push` to build, test, (stage, if applicable), deploy

### For local development:

- run `npm i` to install dependencies

- `npm start` runs the app in development mode.
  Open [http://localhost:3000](http://localhost:3000)

## Testing

`npm test` launches tests
