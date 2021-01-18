# ansible-joomla-with-postgresql-nginx
1. Edit group_vars file
2. Edit roles/joomla/defaults/main.yaml
3. Run ansible-playbook playbook/joomla.yaml

You can use tags:
For install only postgresql: ansible-playbook playbook/joomla.yaml --tags "postgresql"
For install only joomla: ansible-playbook playbook/joomla.yaml --tags "joomla"
For create db, user, etc: --tags "create_db, create_user, grant"
