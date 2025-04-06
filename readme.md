##### AWS Resources Used in this Project
- S3
- Lambda
- Cloudwatch

Steps to execute:
- Extract the data from the Spotify playlist using the Spotify-API and python code.
- Create folders in S3 bucket to store the raw data and processed data.
- Create a Lambda function for "SPOTIFY_API_DATA_EXTRACT" and define the environmental variables under configuration tab to save client_id and client_secret of Spotify API.
- Create Lambda Layer for Spotipy package and add it to the lambda function.
- Create a Trigger of Cloudwatch event.

###### Now we have to transform this data using AWS Glue
- Frist we need to create a role in IAM under roles.
- Give permissions for S3FullAccess, AWSGlueServiceRole, AWSGlueServiceNotebookRole, AWSLambdaFullAccess.
- GIve name to the role and create the role.
- Create a New Notebook in Glue by selected the newly created IAM role.
- Wite the transformation code using Pyspark and run the notebook.
