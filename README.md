# 3tierapplicationdeplyDevSecOps


=========on my local laptop.==============================================
358  cd 3tierapplicationdeplyDevSecOps/
359  ls -ltrh
  360  chmod 755 *.sh
  361  ls -ltrh
  362  ./2nd-Docker.sh
  363  ./3rd-Adduser+python.sh
  364  ls -ltrh
  365  cat /etc/group
  366  vi 3rd-Adduser+python.sh
  367  ./3rd-Adduser+python.sh
  368  ls -ltrh
  369  ./4th-Trivy.sh
  370  trivy version
  371  docker login -u vishaldocker85
  372  docker run -d --name sonar -p 9000:9000 sonarqube:lts-community
  373  systemctl status docker.socket
  374  systemctl start docker.socket
  375  systemctl status docker.socket
  376  docker run -d --name sonar -p 9000:9000 sonarqube:lts-community
  377  docker ps
  378  docker images
  388  hostname -i
  391  curl https://ifconfig.me/
  392  ip addr show eth0 | grep inet         ---------------- to see private ip of localhost
  394  netstat -tuln | grep 8080
  395  ls -ltrh
  396  cat 7th-Pipeline-WithoutTrivy
  397  systemctl status docker.socket
  398  sudo usermod -aG docker jenkins
  399  bash /etc/init.d/jenkins.ubuntu stop
  400  ps -ef | grep jenkins
  401  bash /etc/init.d/jenkins.ubuntu start
  402  ps -ef | grep jenkins
  403  ls -ld /var/run/docker.sock
  405  docker ps
  406  docker images
  407  docker exec -it mysql_db mysql -u root -prootpass
  408  docker exec -it mysql_db mysql -u root -p
--trivy commands - for image scanning
  410  trivy version
  411  docker images
  412  trivy image nginx
  413  trivy image 5107333e08a8
  414  history
