# ansible_local_practise (Make it work, Make it right, Make it fast)
Repository contains ansible setup on local using vagrant and  playbook for multiple task 
 Useful commands:-

(ansible-playbook ./exercise1/web_db.yaml --syntax-check) --to check the syntax

(ansible-playbook ./exercise1/web_db.yaml --tags "apache" --limit "webservers") --to execute playbook for particular tag and server fleet

(ansible <ip address> -i inventory_dev -u vagrant -m ping -k) -- to execute playbook with particular user and module

(ansible-playbook ./exercise1/web_db.yaml --syntax-check) -- to check the syntax of the ansible-playbook

(ansible webservers -i inventory -m yum -a "name=httpd state=present" --sudo -vvv) -- to execute the playbook with verbose module
