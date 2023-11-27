# krueckeKontaktTheme

https://ileriayo.github.io/markdown-badges/  
https://github-readme-stats.vercel.app/

![DieKruecke GitHub stats](https://github-readme-stats.vercel.app/api?username=diekruecke&show_icons=true&theme=dark)

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

4. Ersetze die `config.toml` mit der config Datei: [DOWNLOAD]( https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/diekruecke/krueckeKontaktTheme/blob/main/hugo.toml ).

5. Überprüfe ob der Modul-Import richtig eingetragen ist

    ```yaml
    [module]
      [[module.imports]]
        path = "joly.pw/gohugo-shorturl"
    ```

## Terminal

Starte lokalen DEV Server inkl. Erreichbarkeit via LAN
```zsh
hugo server --bind 0.0.0.0 
```

Git Submodule aktualisieren
```zsh
git submodule update --remote  
```

Git Submodule deinstallieren
```zsh
git submodule deinit themes/krueckeKontaktTheme
git rm themes/krueckeKontaktTheme
```

## Buttons

### Standard Buttons
<details>
<summary>show / hide</summary>

```go
Whatsapp
{{< kontakt_button type="whatsapp" href="/l/wa" text="Whatsapp" >}}

Instagram
{{< kontakt_button type="instagram" href="/l/insta" text="Instagram" >}}

Discord
{{< kontakt_button type="discord" href="/l/dc" text="Discord" >}}

Facebook
{{< kontakt_button type="facebook" href="/l/fb" text="Facebook" >}}

Twitch
{{< kontakt_button type="twitch" href="/l/tw" text="Twitch" >}}

Youtube
{{< kontakt_button type="youtube" href="/l/yt" text="Youtube" >}}

Link
{{< kontakt_button type="link" href="https://www.diekruecke.de/" text="Private Kontaktdaten" >}}
{{< kontakt_button type="link" href="/button-test-area" text="Button Test Area" >}}
```
</details>

### EMail & Telefon -> Bot Sicher
<details>
<summary>show / hide</summary>

```toml
EMail 
{{< kontakt_button_hidden type="email" href="deine@email.de" text="E-Mail" >}}

Telefon
{{< kontakt_button_hidden type="phone" protocol="tel" href="+1234567890123" text="Mobile" >}}
```
</details>

### V-Card
<details>
<summary>show / hide</summary>

#### Code Block
```go
{{< kontakt_button_vcard type="contact" text="Kontakt Speichern" >}}
```

#### V-Card Speicherort

<details>
<summary>VCard für Apple Systeme (iPhone, iPad, iPod, Mac)</summary>
```markdown
/vcard/robin_schroeter_apple.vcf
```
</details>

<details>
<summary>VCard für alle sonstigen Systeme (Windows, Android, alles was nicht als Apple erkannt wird)</summary>
```markdown
/vcard/robin_schroeter.vcf
```
</details>

</details>



### Kontaktdaten vor Bot's verstecken  

#### In Markdown Dateien
EMail Adressen:
  ```go
  {{< data_hide "deine@email.de" >}}  
  ```

Telefonnummern
  ```go
  {{< data_hide address="+49 123 456 789 00" protocol="tel" >}}  
  ```

### Optional parameters

```
<svg viewBox="0 0 XX_width_XX XX_height_XX" class="apple_svg" version="1.1" aria-hidden="true" focusable="false" role="img" xmlns="http://www.w3.org/2000/svg">
  <g fill="currentColor">
    <path d="XXX"/>
    <path d="XXX"/>
  </g>
</svg>
```
