# Project Information  

This project is for the Second Semester Examination Project

## Requirements

A cloud virtual machine 
- I created an EC2 instance in AWS, with a key.pem file. Downloaded the key.pem file and used it to ssh into the instance using `ssh -i /path/to/key.pem ubuntu@18.119.29.217`

- Installation of Nginx: After the SSH i used the terminal to install nginx with `sudo apt install nginx -y`. the `-y` flag is to accepts the question to download package for the nginx

- Providing my HTML Files: From my local machine, I have created `index.html` file and `style.css` file. I have also updated them to show my information

- Push to repo: Using git. i have done the following to push my code to my repository:
```bash
git add .
git commit -m "init"
git push
```

- Deployment: In my ssh terminal, I did the following

```bash
```
