Ansible-SSL-nginx-docker

Generate Intermidiate certificate and sign server certs by Intermidiate. 
Start nginx https server with generated server certificates.

Certificate to import on client's mashines: ca.crt

Prerequisetes:
- docker-py
- openssl
- python-pyOpenSSL

Options(can be edited in int_cert.yml):
- com_name: CommonName
- countryName: -
- stateOrProvinceName: -
- localityName: -
- organizationName: -
- alt_name: alternative domain name
- nginx_conf_folder: Name of the foldr that will contain certs and nginx conf files. It will be connected to docker conteiner
- docker_container_name: Name of the docker container 
- domain_certs: domain names for server certificates

Start executing module:
#ansible-playbook inter_cert.yml
