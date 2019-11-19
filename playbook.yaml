---
- name: Creating a simple playbook
  hosts: all
  tasks:
  - name: IIS service is installed
    win_feature:
       name: Web-Server
       state: present
  - name: IIS service started
    win_service:
       name: W3Svc
       state: started
  - name: Website index.html created
    win_copy:
       content: "Hello World!"
       dest: C:\Inetpub\wwwroot\index.html
...
