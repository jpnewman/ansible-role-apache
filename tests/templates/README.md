### Testing role 'jpnewman.apache' template

~~~
mkdir tmp
~~~

~~~
ansible-playbook ./test_template.yml -i "127.0.0.1," -c local -vvv
~~~

# Proxy

~~~
ansible-playbook ./test_template.yml -i "127.0.0.1," -c local --extra-vars "varfile=./defaults/main_proxy.yml" --extra-vars "output_filename=vhost_proxy.conf" -vvv
~~~

# Alias

~~~
ansible-playbook ./test_template.yml -i "127.0.0.1," -c local --extra-vars "varfile=./defaults/main_alias.yml" --extra-vars "output_filename=vhost_alias.conf" -vvv
~~~
