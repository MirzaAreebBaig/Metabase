# Metabase

Run Ubuntu Server<br><br>

sudo apt update<br>
sudo apt install docker.io<br>
sudo systemctl enable --now docker<br>
sudo usermod -aG docker $USER<br>
<br><br>
docker pull metabase/metabase:latest<br>
docker run -d -p 3000:3000 --name metabase metabase/metabase<br>
