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
