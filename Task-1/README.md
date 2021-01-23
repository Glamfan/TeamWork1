#### Описание файлов

1. Task-1/ansible.cfg - конфига ansible
2. Task-1/hosts - интвентори файл
3. Task-1/docker-compose.yml - docker-compose.yml файл с 3-мя сервисами  adminer. Порты на которых запукаются эклемпляры adminer 10001,10002,10003
4. Task-1/docker_install_ubuntu.yml - Ansible плейбук для утановки docker и запуска docker-compose.yml


 Переменные в docker_install_ubuntu.yml:

1. директория на удаленном компьютере для копирования  docker-compose.yml
   - tmp_folder: /tmp/Docker 
2. директория на локальном компьютере с docker-compose.yml
   - tmp_folder_local: /TEST/ansible 
