# twitter_to_s3_firehose
node_js code to run firehose process on EC2 to get tweets and send them to an s3 bucket.
# Social Media Macroscope - ingest twitter data and store on s3

Javascript code run in NODE js to get twitter sample stream and use Kiniesis Firehose to write data to an s3 bucket.

## Getting Started

The code for this app was from the blog post by Assaf Mentzer at: https://aws.amazon.com/blogs/big-data/building-a-near-real-time-discovery-platform-with-aws/  
The above, well written, blog post explains how to use this node js app, indicates where to get Assaf Mentzer's code, and put this app into context with the overall twitter to elastic search pipeline.

### Command to start process on EC2 as a nohup job running in the background

Added to the code set is a bash script, run_twitter_stream_producer_app_w_nohup.sh, to start the node js app running in the background on an EC2 server.

```
cd ~/applications/twitter_stream_producer_app
sh run_twitter_stream_producer_app_w_nohup.sh
```

## Acknowledgments

* Purple Booth for a nice readme.md template (https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)

:e-mail: email me: _jmtroy2@illinois.edu_
