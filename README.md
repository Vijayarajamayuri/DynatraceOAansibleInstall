# DynatraceOAansibleInstall

##simple playbook with no hostgroups:

---
- hosts: all
  become: true
  roles:
    - role: Dynatrace-OneAgent-Ansible
  vars:
    dynatrace_environment_url: qwl01543.live.dynatrace.com
    dynatrace_paas_token: dt0c01.MLZ6TKLZPSIMQSMLIWWTZJEB.43IDVLZV75T6ORBUFUI45V3DGKPITA6HOVP4QGAPB4P2FTRDJXRLLKUKOIHENAHB
    
    **ansible-playbook main.yml -i /etc/ansible/hosts -e vars.yml -kK
  


## with hostgroups
