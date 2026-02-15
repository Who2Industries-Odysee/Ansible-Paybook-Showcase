## piinstall.yml ##
### Edit the inventory.ini file ###
Edit the inventory.yml file and change ``ansible_host`` as well as ``ansible_user``.
Optionally edit ``debian_vm`` and ``vm`` to something you prefer.
If you choose to not use key based ssh authentication, you may want to remove ``ansible_ssh_private_key_file``.

### Execute the playbook ###
Now that you edited the **inventory.ini** file, you may proceed to execute the playbook.
For that, there are two options.
Note that both commands do the same thing, the only difference is in how you write it.

**- Option 1**
``ansible-playbook -i inventory.ini -b --ask-pass --ask-become-pass  piinstall.yml``


**- Option 2**
``ansible-playbook -i inventory.ini -b -k -K  piinstall.yml``


## Footer ##
Made by **spoljarevic**, founder of **Who2Industries**.
This Repository is for showcasing on Odysee.
If you see it on any other platform or from any other channel then Who2Industries, don't click on any links since it's unofficial and might be a scam.

To follow and see updated versions of these files and to create pull requests and issues, please go to the main repo [here](https://codeberg.org/Spoljarevic/Ansible/src/branch/master/installation/piinstall.yml#).

We wish you a nice day and remember... **Stay private. Stay root.**
