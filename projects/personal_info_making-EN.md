# Video-based Personal Information De-identification Service

# Summary

<img src="images/Screenshot%202025-04-08%20170910.png" width=800></br>

- Trained a deep learning based model on a custom dataset to recognize personal information (e.g., faces, license plates) in videos using Python and C++.
- Dockerized the inference process for portability and scalability.
- Built an API server leveraging AWS ECS/Batch for efficient processing.
- Developed a web-based user interface using PHP for ease of access.

# Project Details

## Overall Process

<img src="images/Screenshot%202025-04-08%20171152.png" width=800></br>

1.  User uploads a video via the web interface, which is then stored in an S3 bucket.
2.  A Lambda function is triggered to extract video metadata and record it in the database.
3.  When the user requests video processing, an AWS Batch task is initiated with the relevant video information.
4.  The Docker image containing the inference process runs within AWS ECS.
5.  Upon completion, the processed video is saved back to S3, and the user is notified.