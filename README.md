# krueckeKontaktTheme

## Features

## Installation / Einrichtung

1. Hugo Mod init

  ```shell
  hugo mod init github.com/diekruecke/krueckeKontaktTheme

  hugo mod get -u -v joly.pw/gohugo-shorturl
  ```

2. Git Submodule init

  ```bash
  git submodule add https://github.com/diekruecke/krueckeKontaktTheme themes/krueckeKontaktTheme
  ```

3. Starte den Server mit `hugo server`. Die Module werden automatisch heruntergeladen.

4. Ersetze die `config.toml` mit der config Datei: [download a copy]( DOWNLOADLINK https://minhaskamal.github.io/DownGit/#/home ) .

### Git Submodule aktualisieren

  ```shell
  git submodule update --remote
  ```

### Git Submodule deinstallieren

  ```shell
  git submodule deinit themes/krueckeKontaktTheme
  git rm themes/krueckeKontaktTheme
  ```


## Configuration

Kontaktdaten vor Bot's verstecken  

    ```go
    {{< cloakemail "jane.doe@example.com" >}}
    ```

### Optional parameters

```
<svg viewBox="0 0 XX_width_XX XX_height_XX" version="1.1" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="font-awesome-flag" class="svg-inline--fa fa-font-awesome-flag fa-w-14" role="img" xmlns="http://www.w3.org/2000/svg">
  <path fill="currentColor" d="XXXXX"/>
</svg>
```

<svg viewBox="0 0 29.2546 27.2269" version="1.1" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="font-awesome-flag" class="svg-inline--fa fa-font-awesome-flag fa-w-14" role="img" xmlns="http://www.w3.org/2000/svg">
