# ansible-role-mysql2
geerlingguy / ansible-role-mysql 의 소스를 forked 하였습니다. MySQL 8 버전을 ubuntu, rocky8 버전에 설치할 수 있습니다.

실행에 앞서 아래 명령어로 mysql 관련 ansible 모듈을 받아야합니다.

ansible-galaxy collection install community.mysql

ubuntu 설치의 경우 tar 볼을 이용한 설치방식이기 때문에 아래와 같은 명령어로 로컬에 다운로드하고 시작해야합니다.

wget https://downloads.mysql.com/archives/get/p/23/file/mysql-8.0.39-linux-glibc2.12-x86_64.tar.xz
wget https://downloads.mysql.com/archives/get/p/23/file/mysql-8.0.31-linux-glibc2.12-x86_64.tar.xz

ansible-playbook -i inventory/aws-mysql-server mysql_deploy.yml