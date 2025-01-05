# sddm-binary-theme

A theme for the [SDDM login manager](https://github.com/sddm/sddm).

- Screen resolution: 1080p
- Font: Open sans

### Preview

You can easily change how it looks in **[config](./Themes/binary.conf)**. 
Here are some examples:

![Preview](./Previews/preview1.png)
![Preview](./Previews/preview2.png)
![Preview](./Previews/preview3.png)
![Preview](./Previews/preview4.png)

### Dependencies

#### Arch, Void
```sh
sddm qt6-svg
```
#### Fedora
```sh
sddm qt6-qtsvg
```
#### OpenSUSE
```sh
sddm-qt6 qt6-svg
```

### Install

1. Clone this repository, copy fonts to `/usr/share/fonts/`:

   ```sh
   sudo git clone https://github.com/binaryharbinger/sddm-binary-theme.git /usr/share/sddm/themes/sddm-binary-theme
   sudo cp /usr/share/sddm/themes/sddm-binary-theme/Fonts/* /usr/share/fonts/
   ```

2. Then edit `/etc/sddm.conf` using the following command:

    ```sh
    echo "[Theme]
    Current=sddm-Binary-theme" | sudo tee /etc/sddm.conf
    ```


### Virtual keyboard

![Preview](./Previews/preview5.png)

#### Arch
1. Install package.
    ```sh
    sddm qt6-virtualkeyboard
    ```

2. Then edit `/etc/sddm.conf.d/virtualkbd.conf`, so that it looks like this:

    ```sh
    [General]
    InputMethod=qtvirtualkeyboard
    ```

### Credits

Based on the theme [`SDDM Astronout Theme`](https://github.com/kittydev/sddm-astronout-theme) by **MarianArlt**.

### License

Distributed under the **[GPLv3+](https://www.gnu.org/licenses/gpl-3.0.html) License**.    
Copyright (C) 2025 BinaryHarbinger.
