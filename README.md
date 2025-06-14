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
    # clone repository called webserver
    git clone https://github.com/devbeisong/webserver.git
    # this creates a folder called webserver with all our files inside

    # remove old content from current nginx serving directory
    sudo rm -R /var/www/html/*
    # the * sign tells the script to remove everything in the html folder. sudo used for permission

    # replace content with repository by copying all items inside folder
    sudo cp -R webserver/* /var/www/html
    # this copies everyting inside the webserver folder and into the html folder. sudo was used to override restriction
```


- Public IP: [18.119.29.217](http://18.119.29.217/index.html)

- Screenshot

![image](screenshot.png) 
