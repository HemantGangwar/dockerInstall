## Docker Installation on CentOS7

![image](https://user-images.githubusercontent.com/38517925/87787631-970bd100-c859-11ea-8da5-b7f93d0acba4.png)

## Usage

* #### #git clone https://github.com/HemantGangwar/dockerInstall.git
* #### #cd dockerInstall
* #### # ansible-playbook playbook/docker-setup.yml

## Code Execution

> [root@workstation LabENV dockerInstall ]# ansible-playbook playbook/docker-setup.yml

> PLAY [|Docker| deployment on CentOS 7] ***********************************************************************************************

> TASK [Gathering Facts] ***************************************************************************************************************
> ok: [dnode1.technix.com]
> ok: [dnode3.technix.com]
> ok: [dnode2.technix.com]

> TASK [1. Pre-Requisite Package installation] *****************************************************************************************
> ok: [dnode3.technix.com]
> ok: [dnode1.technix.com]
> ok: [dnode2.technix.com]

> TASK [2. Adding required repository] *************************************************************************************************
> changed: [dnode3.technix.com]
> changed: [dnode2.technix.com]
> changed: [dnode1.technix.com]

> TASK [3. Installing Docker Community edition] ****************************************************************************************
> changed: [dnode2.technix.com]
> changed: [dnode1.technix.com]
> changed: [dnode3.technix.com]

> TASK [4. Starting docker Service and setting for autostart] **************************************************************************
> changed: [dnode2.technix.com]
> changed: [dnode3.technix.com]
> changed: [dnode1.technix.com]

> PLAY RECAP ***************************************************************************************************************************
> dnode1.technix.com         : ok=5    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
> dnode2.technix.com         : ok=5    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
> dnode3.technix.com         : ok=5    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0

> [root@workstation LabENV dockerInstall ]#
