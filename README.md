
# Usage

Vagrantfile
===========

```ruby
config.vm.provision "provision-user", type: "ansible" do |ansible|
  ansible.playbook = "adduser-cadizm.yml"
  ansible.sudo = true
end
```

Localhost
=========

```
$ ansible-playbook -i "localhost," -c local adduser-cadizm.yml
```
