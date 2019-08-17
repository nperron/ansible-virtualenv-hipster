# ansible-virtualenv-hipster
```bash
$ ansible-playbook -kK -i 00_init/all.ini playbook-init.yaml -D
[...]
```

```bash
$ ansible-playbook -kK -i inventories/dev.ini play
[...]
PLAY [Dummy playbook] *********************************************************************************************************************************************************************************************

TASK [Gathering Facts] ********************************************************************************************************************************************************************************************
ok: [ansible-sandbox]

TASK [dummy : Show variables] *************************************************************************************************************************************************************************************
ok: [ansible-sandbox] => {
    "msg": "Python version: {'version': {'major': 3, 'minor': 7, 'micro': 4, 'releaselevel': 'final', 'serial': 0}, 'version_info': [3, 7, 4, 'final', 0], 'executable': '/usr/local/ansible/ansible-venv/bin/python', 'has_sslcontext': True, 'type': 'cpython'}"
}

PLAY RECAP ********************************************************************************************************************************************************************************************************
ansible-sandbox            : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
```
