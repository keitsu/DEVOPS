# DEVOPS

# Pour executer le playbook via ssh
ansible-playbook -vvv -i inventory/dev/hosts infrastructure.yml

# Pour tester avant d'executer
ansible-playbook -vvv -i inventory/dev/hosts infrastructure.yml --check

# Pour executer seulement ce qui n'a pas fonctionné 
ou remplacer "@YOUR_PATH/infrastructure.retry" par un host pour tester la configuration que sur celui ci.

ansible-playbook -vvv -i inventory/dev/hosts infrastructure.yml --limit @YOUR_PATH/infrastructure.retry



