## Docker Installation on CentOS7

![image](https://user-images.githubusercontent.com/38517925/87787631-970bd100-c859-11ea-8da5-b7f93d0acba4.png)

## Usage

* #### #git clone https://github.com/HemantGangwar/dockerInstall.git
* #### #cd dockerInstall
* #### # ansible-playbook playbook/docker-setup.yml

## Code Execution

<blink>
[root@workstation LabENV dockerInstall ]# ansible-playbook playbook/docker-setup.yml

PLAY [|Docker| deployment on CentOS 7] ***********************************************************************************************

TASK [Gathering Facts] *************************************************************************************************************** </br >
ok: [dnode1.technix.com] </br >
ok: [dnode3.technix.com] </br >
ok: [dnode2.technix.com] </br >

TASK [1. Pre-Requisite Package installation] ***************************************************************************************** </br >
ok: [dnode3.technix.com] </br >
ok: [dnode1.technix.com] </br >
ok: [dnode2.technix.com] </br >

TASK [2. Adding required repository] ************************************************************************************************* </br >
changed: [dnode3.technix.com] </br >
changed: [dnode2.technix.com] </br >
changed: [dnode1.technix.com] </br >

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
</blink>
