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
