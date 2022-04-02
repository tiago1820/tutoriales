#### Virtualização

- Para ver se meu processador é compativel com a 
virtualização do tipo 1. Se tiver a flag vmx no arquivo
, então é compatível (Para processadores intel):

```
 $ vmx /proc/cpuinfo | less
```

- Para processadores AMD faça (talvez seja necessário
habilita-lo na BIOS):

```
 $ grep svm /proc/cpuinfo
```

- Virtualização do tipo 1 - Bare Metal

  Hardware
   -hypervisor
      -VM
         -OS
           -app
           -app

- Conceitos:
  kvm->módulo kernel
  QEMU->hardware
  libvirt->API
  
  virsh->CLI
  virt-manager->gráfico

- Recursos:

 Memória
 Processador
 BIOS/UEFI
 
 Dispositivos
 usb, vídeo, etc

- Discos
 
 HD virtual->arquivo máquina real
 qcow2, raw

 DVD virtual->arquivo ISO

- Rede
 
 Interface virtual->máquina real
 
 Switch virtual
 Servidor DHCP
 NAT

 Interface->VM

 Real
  -Virtual
    -VM-1
    -VM-2

- Mão na massa:

  -Instalação
  -Funcionamento

  -Criação de VM
  -Uso Virsh
  -Uso virt-manager



 
























