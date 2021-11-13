# Pipeline

Circle CI is the tool used for CI of this project.

A .circleCi folder contains a yml config file to handle the steps in order to depoy the app.

A push on main github branch will trigger the continuous integration in this way:

1. Commit and push on branch `main`
2. Circle CI starts `building` phase with its steps
3. Circle CI stays in `hold` until integration of the code is approved for delivery
4. After approval, `aws-cli` and `eb` are set up
5. Then the `deploy` scripts is run to deliver the updated builded code to aws services