# Node Server Notes

### Heroku

#### Deployment Checklist

- Dynamic Port Binding
  - Listen to whatever port Heroku tells us to
  - Taken care of in `index.js` with `PORT` variable. Heroku injects a value to `process.env.PORT`.
- Specify Node Environment
  - Tell Heroku which version of Node we want
  - `"engines"` block in package.json
- Specify start script
  - Tell Heroku what to run to start the server
  - `"scripts"` block in package.json
- Ensure .gitignore exists
  - Heroku will include dependencies on its own
