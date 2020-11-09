## Ansible Playbooks

###userCreation.yml

**Install passlib password hashing library**
pip install passlib

**Generate a hashed output of the password**
python -c “from passlib.hash import sha512_crypt; import getpass; print(sha512_crypt.using(rounds=5000).hash(getpass.getpass()))”

- Enter a password for john.doe
- Paste into the playbook, replacing <hashed output>
