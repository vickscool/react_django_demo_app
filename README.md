# react_django_demo_app
A demo app for React and Django Deployment

docker-compose down
docker-compose up -d

-----steps to be followed to deploy a sample react-django app using dockerfile------

-git clone https://github.com/vickscool/react_django_demo_app.git
-mkdir react-django-app
-cd react-django-app
-update the dockerfile with content from this repository 
-Build the image from dockerfile : docker build . -t react-django-app:latest
-Check the images : docker images
-Run the container from build image : docker run -d -p 8000:8000 react-django-app:latest
-Enable port 8000 in inbound security group of VM you are working on . For  ex. from AWS Console
