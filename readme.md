This a LEMP provisioned vagrant environment.

Playbook was designed to be suitable to set up environment on externals servers as well.

Roles are saved in their folders unaltered (as they should)

To start using this environment:
1. Update Vagrantfile with relevant ip for private network, synced folder and machine name
2. Create proper folders structure. Currently it assumes, that structure is: folders /html and /vagrant (content of this repository) are on the same level. /html contains /backend and /frontend plus /ssl folder with key and certificate generated for ssl to work.
3. Create env.config.yml from example
4. Don't forget to create relevant /etc/hosts entry

If adminer is enabled, it would be available through http://adminer.server_name