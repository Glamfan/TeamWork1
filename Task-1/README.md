#### Описание файлов

1. Task-1/ansible.cfg - конфига ansible
2. Task-1/hosts - интвентори файл
3. Task-1/docker-compose.yml - docker-compose.yml файл для развертывания 3-х контейнеров adminer и 1 контейнера nginx. Порты на которых запукаются эклемпляры adminer 10001,10002,10003
4. Task-1/docker_install_ubuntu.yml - Ansible плейбук для утановки docker
5. Task-1/start_nginx_lb.yml - Ansible плейбук для развертывания 3 контейнером adminer и контейнера c nginx как балансировщика. 
6. Task-1/nginx.conf - конфига nginx для балансировки
7. Task-1/Dockefile - для создания контейнера nginx и копирования в него файла конфигурации


 Переменные в docker_install_ubuntu.yml и start_nginx_lb.yml :

1. директория на удаленном компьютере для копирования  docker-compose.yml
   - tmp_folder: /tmp/Docker 
2. директория на локальном компьютере с docker-compose.yml
   - tmp_folder_local: /TEST/ansible 
