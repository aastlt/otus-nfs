# otus-nfs
Работа с NFS

Описание стенда:

Виртуальные машины создаются средствами libvirt (при желании можно сменить провайдера в Vagrantfile):

nfss - сервер

nfsc - клиент

При запуске vagrant up, посредством скриптов nfss_script.sh и nfsс_script.sh, производится установка и настройка NFS:
- на сервере создается директория /srv/share/upload, автоматически монтируется в /mnt/upload клиента
- запускается firewall, разрешается доступ к сервисам NFS

Для проверки выполнить:

vagrant up
