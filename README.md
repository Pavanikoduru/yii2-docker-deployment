# yii2 Docker Deployment

This project demonstrates how to deploy a **PHP Yii2 application** using **Docker** on **Ubuntu 24.04** without using any cloud provider. You can access the application locally via browser at `http://localhost:8000`.

1. Clone the repository
git clone https://github.com/Pavanikoduru/yii2-docker-deployment.git
cd yii2-docker-deployment/yii2-docker

2. Build the Docker image
docker build -t yii2-app .

3. Run the Docker container:
docker run -d -p 8000:80 --name yii2_app yii2-app

If port already in use means:
Stop and Remove the container:
docker stop yii2_app
docker rm yii2_app

then agaon run the docker conatiner command
 
4. Open the app in your browser
Go to http://localhost:8000


