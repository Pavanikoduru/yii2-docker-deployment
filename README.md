# Yii2 Docker Deployment

Steps to Run

1. **Clone the repository**
git clone https://github.com/Pavanikoduru/yii2-docker-deployment.git
cd yii2-docker-deployment

2. Build the Docker image:
docker build -t yii2-app .

3. Run the Docker container:
docker run -d -p 8000:80 --name yii2_app yii2-app


4. Open your browser and visit:
http://localhost:8000

If port 8000 is already in use

Find the container ID running on the port: docker ps

Stop the container: docker stop <container_id>

Remove the container: docker rm <container_id>

Now run the container again:
docker run -d -p 8000:80 --name yii2_app yii2-app
