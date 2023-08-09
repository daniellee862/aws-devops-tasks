# AWS DevOps Tasks  🛠️🚀
![AWS Logo](images/aws.png)

## Technologies used:
![AWS Badge](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)

- Amazon Polly 🗣️
- Amazon Rekognition 👁️
- EC2 🖥️
- S3 ☁️
- IAM 🔒
- CloudWatch ☁️🕰️


## Task One: deploy a Node.js / Express.js server on AWS EC2

![Node.js Express](images/NODE-EXP.jpeg)

```node
const express = require("express");
const app = express();
const port = 3000;

app.get("/", (req, res) => {
  res.send("Hello Daniel!");
});

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`);
});
```

Steps for task completion;

- Used a `t2.micro` instance (the default).
- Used Amazon Linux operating system.
- Allow HTTP and SSH traffic.
- Enabled public IP address creation.
- Used `npm` to install the dependencies.
- Redirected requests from Port 80 to Port 3000 to allow the server to respond.

---

## Task Two: Build small applications that make use of AWS services by using the command line API

### Amazon POLLY 🦜

[Amazon Polly](https://aws.amazon.com/polly/) (text-to-speech software).

![](images/POLLY-LOGO.png)

Steps for task completion;

- Used Amazon Polly, a text-to-speech software, to generate audio files from text in different languages.
- Created multiple S3 buckets to store multi-language text files and audio files.
- Prompt Polly to read text files from an S3 bucket, generate converted audio files and save to a different S3 bucket
- configure Polly to use computer OS to use the sound files and 'read' them for the user.
- Used bucket policies to allow public downloads and streaming of audio

![](images/POLLY.png)

### Amazon Rekognition 👁️

[Amazon Rekognition](https://aws.amazon.com/rekognition/)

![](images/REKOG-LOGO.png)

Steps for task completion;

- Use Amazon Rekognition, a machine learning tool for image and video analysis,to analyze some image files and test its abilities to detect people, faces, emotions, activities, and celebrities. 
- Pass image files into Rekognition and obtain JSON output that describes the contents of the pictures.
- Use jq, a command-line JSON processor, to extract certain attributes from the JSON output obtained from Rekognition and saved the to a local .txt file.

![](images/REKOG.webp)





