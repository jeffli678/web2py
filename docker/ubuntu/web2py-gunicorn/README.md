# Start Service
	systemctl start docker

# Docker
	cd /Docker/Ubuntu/web2py-gunicorn
	docker build -t your_username/ubuntu-web2py-gunicorn .
	docker run -d -v applications:/home/web2py/web2py/applications -p 8000:8000 --name ubuntu-web2py-gunicorn your_username/ubuntu-web2py-gunicorn
	docker ps 
	docker volume ls
	docker volume inspect applications

# Docker Compose
	pip install docker-compose
	cd /Docker/Ubuntu/web2py-gunicorn
	docker-compose up -d
	docker-compose ps
	docker volume ls
	docker volume inspect root_applications

# Docker Cloud
	cd /Docker/Ubuntu/web2py-gunicorn
	docker login -u your_username
	docker build -t your_username/ubuntu-web2py-gunicorn .
	docker push your_username/ubuntu-web2py-gunicorn

# Shell (Copy the content of the file into this scaffolding shell and replace the variable text $ with \$ )
cat << EOF > docker-compose.yml

EOF
cat docker-compose.yml

cat << EOF > Dockerfile

EOF
cat Dockerfile

docker build -t your_username/ubuntu-web2py-gunicorn .
docker run -d -v applications:/home/web2py/web2py/applications -p 8000:8000 --name ubuntu-web2py-gunicorn your_username/ubuntu-web2py-gunicorn

docker-compose up -d
docker-compose ps
