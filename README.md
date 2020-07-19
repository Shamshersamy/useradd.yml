# useradd.yml
This is for user creation in Linux servers.
---
# this is for add a user useing ansible
 - name: Add new user user1
   hosts: all
   become: ansadmin
   tasks:
           - name: add user1
             user:
                name: user1
                state: present
