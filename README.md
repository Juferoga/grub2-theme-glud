```
     _____ ______ _   _______   _____  _     _   _______ 
    |  __ \| ___ \ | | | ___ \ |  __ \| |   | | | |  _  \
    | |  \/| |_/ / | | | |_/ / | |  \/| |   | | | | | | |
    | | __ |    /| | | | ___ \ | | __ | |   | | | | | | |
    | |_\ \| |\ \| |_| | |_/ / | |_\ \| |___| |_| | |/ / 
     \____/\_| \_|\___/\____/   \____/\_____/\___/|___/  
                                                        

```

## Diseño de GRUB con tema para el Grupo GNU/Linux UNiversidad Distrital.

## Instalar

Uso:  `sudo ./install.sh [OPCIONES...]`

|  OPCIONES:          | Descripcion |
|:-------------------|:-------------|
| -b, --boot         | Instalar el tema en  /boot/grub/themes |
| -v, --vimix        | Tema grub Vimix |
| -s, --stylish      | Tema grub Stylish |
| -t, --tela         | Tema grub Tela |
| -w, --white        | Instalar iconos en version Blanco |
| -u, --ultrawide    | Instalar imagen de fondo para 2560x1080 |
| -r, --remove       | Remover un tema (se debe agregar el nombre del tema) |
| -h, --help         | Mostrar Ayuda |

Por ejemplo:

1. Instalar tema Tela 

    `sudo ./install.sh -t`
    or
    `sudo ./install.sh --tela`

2. Instalar tema Tela en /boot/grub/themes

    `sudo ./install.sh -b -t`

3. Remover Tela theme

    `sudo ./install.sh -r -t`

## Resoluciones

#### Configrure la mejor resolución para su PC

En la pantall del grub , `precione c` para entrar a la linea de comandos, posterior ingrese `vbeinfo` o `videoinfo` en EFI boot para revisar que resoluciones puede utilizar, despues edite `/etc/default/grub` , añada la resolución `GRUB_GFXMODE=****x****x32` en el archivo, por ultimo ejecutar `grub-mkconfig -o /boot/grub/grub.cfg` para actualizar el grub.cfg.

## Capturas de Pantalla

### Tema grub Vimix

![vimix grub theme](screenshots/grub-theme-vimix.jpg?raw=true)

### Tema grub Stylish

![Stylish grub theme](screenshots/grub-theme-stylish.jpg?raw=true)

### Tema grub Tela 

![Tela grub theme](screenshots/grub-theme-tela.jpg?raw=true)