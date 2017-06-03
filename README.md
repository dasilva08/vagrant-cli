# Vagrant comandos

Comandos úteis para manipulaçao da VM.

[Lista completa de comandos](https://www.vagrantup.com/docs/cli/)

#### Acesso a VM
- vagrant up (Inicia a VM)
- vagrant ssh (Acessa a VM)
- vagrant suspend (suspender)
- vagrant resume (reiniciar VM)
- vagrant reload (Reinicia a VM)
- vagrant destroy (remove a máquina virtual existente)

### Instalação de Plugins

Rodando o comando: **`vagrant`** 

**EX:** **`vagrant plugin install vagrant-vbguest`**

- expunge
- install
- license
- list
- repair
- uninstall
- update

### Controlando a quantidade de memoria que a box da máquina:
Dentro de sua VM abra o arquivo: **`Vagrantfile`**
```ruby
  config.vm.provider :virtualbox do |vb|
    vb.customize ['modifyvm', :id, '--memory', '2048']
  end
```

### Senha para acesso vagrant
user: vagrant
senha: vagrant
