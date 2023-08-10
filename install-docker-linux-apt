### Installing Docker on Linux with APT

### 1. Update the apt package index & install packages to allow apt to use repository over HTTPS:

sudo apt-get update
sudo apt-get install ca-certificates curl gnupg

### 2. Add Docker's Official GPG key:

sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

### 3. Use the following command to setup the repository:

echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

### 4. Update the apt package index:

sudo apt-get update

### 5. Install Docker Engine, Containerd & Docker Compose

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
