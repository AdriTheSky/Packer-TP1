# Packer-TP1 | Adrien Parra

# Ansible Install :

Update :
```bash
dnf update
```

Enable EPEL repo :
```bash
dnf install epel-release
```

Installation Ansible :
```bash
dnf install ansible
```

Vérifier la version :
```bash
ansible --version
```

# Git Install :

```bash
dnf install git
git config --global user.name "AdrienPfr"
git config --global user.email "parra.adrien@gmail.com"
```

# Execut build with Packer :

```bash
packer build <File_Name>.pkr.hcl
```

Une fois le build lancé, on peut se connecter avec VNC sur le port donnée lors du build.

# Execut buil after stop :
```bash
/usr/libexec/qemu-system-x86_64 -name Rocky-GolangMyIP-packer -netdev user,id=user.0,hostfwd=tcp::4141-:22 -device virtio-net,netdev=user.0 -drive file=build-rocky-8/tdhtest,if=virtio,cache=writeback,discard=ignore,format=qcow2 -machine type=pc,accel=kvm -smp cpus=2,sockets=2 -m 4096M
```
