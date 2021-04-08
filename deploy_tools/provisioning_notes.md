Provisionamento de um novo site
===============================

## Pacotes necessários:

* nginx
* python 3.8
* virtualenv + pip
* Git

Por exemplo, no Ubuntu:

	sudo add-apt-repository ppa:fkrull/deadsnakes
	sudo apr-get install nginx git python38 python3.8-venv

## Config do Nginx Virtual Host

* veja nginx.template.conf
* substitua SITENAME, por exemplo, por staging.my-domain.com

## Serviço Systemd

* veja gunicorn-systemd.template.service
* substitua SITENAME, por exemplo, por staging.my-domain.com

## Estrutura de pastas:
Suponha que temos uma conta de usuario em /home/username

/home/username
|__ sites
	|__ SITENAME
		|__ database
		|__ source
		|__ static
		|__ virtualenv
