#### Virtualização #2

- Para ver se a máquina tem suporte a virtualização do tipo 1:
```
 $ lscpu
 
 $ grep vmx /proc/cpuinfo (intel)
 $ grep svm /proc/cpuinfo

```

- Para instalar o virt-manager:
```
 # apt-get install virt-manager
```

- Para instalar o virsh:
```
 # apt-get install virsh
```

- Para ver o status do serviço libvirts:
```
 # systemctl status libvirtd.service
```

- Para entrar na ferramenta virsh:
```
 $ virsh
```

- Para ver o manual do virsh:
```
 $  man virsh
```

- Para listar as VMs que foram criadas:
```
 # virsh list --all
```

- Para ver a versão do meu Debian:
```
 $ lsb_release -a
```

- No ambiente gráfico abra o Gerenciador de Máquinas Virtuais.

- Para adicionar o usuário ao grupo libvirt, para não ter que
colocar senha a todo momento:
```
 $ adduser tiago libvirt
 $ id tiago
```

- Baixe a iso da qual você quer criar a máquina virtual.

- Estude os menus do Gerenciador Máquinas Virtuais.


- Crie um pool para as isos e outro pool para guardar
os discos virtuais

- Crie uma máquina virtual padrão com 2 gb de HD

- Para ver as minhas virtualizações no terminal:
```
 virsh list --all
```

- Para iniciar a máquina virtual:
```
 virsh start nome_da_maquina
```
- Para colocar a api em funcionamento( se necessário):
```
 $ systemctl is-enabled libvirtd.service
```

- Para desabilitar o funcionamento da api:
```
 $ systemctl disable libvirtd.service
```

- Para iniciar a virtualização:

```
 $ systemctl start libvirtd.service
```

- Para saber o nome das máquinas que tenho para trabalhar:
```
 $ virsh list --all
```

- Para fazer reboot na máquina:
```
 $ virsh reboot --domaain nome_da_maquina
```

- Para ver todas as redes virtuais que eu tenho:
```
 $ virsh net-list
```

- Para ver informações da rede, como um log do servidor
DHCP:
```
 $ virsh net-dhcp-leases default(nome_da_rede)
```

- Para editar uma máquina virtual:
```
 $ virsh edit --domain nome_da_maquina 
```
-- Abra o arquivo xml e faça as alterações necessárias








 

























