sudo apt update

sudo apt install curl

curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash

sudo apt-get install gitlab-runner

sudo systemctl enable --now gitlab-runner

sudo systemctl status gitlab-runner

sudo usermod -aG docker gitlab-runner
