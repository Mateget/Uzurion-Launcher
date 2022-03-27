# Mise en place d'un serveur Web avec PHP

Cette partie est dédié aux utilisateurs qui n'ont pas de serveur web déjà mise en place.<br>
Le serveur web va permettre au launcher lors de son démarrage d'aller chercher la configuration et les fichiers que vous voulez ajouter au client minecraft comme des mods par exemple. <br>

Il y a ici deux possibilités:
 - Soit vous n'avez pas de serveur distant, dans ce cas nous utiliserons une machine virtuel en local, le launcher ne fonctionneras donc que pour vous
 - Soit vous avez un serveur distant et le launcher fonctionneras pour tous les utilisateur à qui vous partager votre launcher

## Mise en place d'un serveur en local

Si vous avez un serveur distant, passez directement à l'installation du serveur web et de Php.
Pré-requis : 
 - Installer Virtual Box
    - [Windows](https://download.virtualbox.org/virtualbox/6.0.24/VirtualBox-6.0.24-139119-Win.exe)
    - [Mac]
 - [Télécharger une image Debian](https://cdimage.debian.org/debian-cd/current/amd64/iso-cd/debian-11.3.0-amd64-netinst.iso)

Une fois Virtual Box installé, il faut créer une machine virutel à partir de l'image téléchargé.

![Virutal box Add](./images/virtual_box_add.png)

Il faut bien choisir le type de la machine virtuel.

![Type VM](./images/type_vm.png)

Concernant la RAM à alloué 1024 Mo est largement suffisant.<br>
Choissiez ensuite "Créer un disque dur virtuel maintenant".<br>
Choissiez ensuite "VDI (image de Disque VirtualBox)".<br>
Choissiez ensuite "Créer un disque dur virtuel maintenant".<br>
Choissiez ensuite "Dynamiquement alloué".<br>

Vous pouvez changer l'endroit ou le fichier de la machine virtuelle sera enregistré, vous pouvez également changer la mémoire disponible, mais sachez que 8Go est largement suffisant.

![Path VM](./images/vb_path.png)

Voux pouvez démarrer votre machine virtuel.

![Launch VM](./images/launch_vb.png)

Lors du premier démarrage il va vous être demandé de choisir l'image a utilisé.

![Choose Image VM](./images/choose_image.png)

Vous devez idiquer l'emplacement de l'image que vous avez télécharger plustôt.

![Add Image VM](./images/add_image_vb.png)

Vous pouvez ensuite cliquer sur "Démarrer".

![Start VM](./images/start_vb.png)