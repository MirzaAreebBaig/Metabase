# Metabase

Run Ubuntu Server

sudo apt update
sudo apt install docker.io
sudo systemctl enable --now docker
sudo usermod -aG docker $USER

docker pull metabase/metabase:latest
docker run -d -p 3000:3000 --name metabase metabase/metabase
