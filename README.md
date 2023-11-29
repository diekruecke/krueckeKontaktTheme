# krueckeKontaktTheme - Hugo Theme

## Installation / Einrichtung

1. Hugo Mod init

   ```zsh

   hugo mod init github.com/diekruecke/krueckeKontaktTheme
   ```

2. Hugo Modul-Imports in die Config rein

   ```toml
   [module]
   [[module.imports]]
      path = "joly.pw/gohugo-shorturl"
   [[module.imports]]
      path = "github.com/diekruecke/krueckeKontaktTheme"
   ```

3. Starte den Server mit `hugo server`. Die Module werden automatisch heruntergeladen.

4. Ersetze die `config.toml` mit der config Datei: [DOWNLOAD]( https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/diekruecke/krueckeKontaktTheme/blob/main/hugo.toml ).


---

## Terminal

Starte lokalen DEV Server inkl. Erreichbarkeit via LAN
```zsh
hugo server --bind 0.0.0.0 
```

Hugo Module aktualisieren
```zsh
hugo mod get -u
```

---

## Buttons

Standard Buttons

```md
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

### EMail & Telefon -> Bot Sicher

```md
EMail 
{{< kontakt_button_hidden type="email" href="deine@email.de" text="E-Mail" >}}

Telefon
{{< kontakt_button_hidden type="phone" protocol="tel" href="+1234567890123" text="Mobile" >}}
```

### V-Card

```md
{{< kontakt_button_vcard type="contact" text="Kontakt Speichern" >}}
```

<details>
<summary>V-Card Speicherort</summary>
   
- VCard für Apple Systeme (iPhone, iPad, iPod, Mac)

  ```
  /vcard/robin_schroeter_apple.vcf
  ```

- VCard für alle sonstigen Systeme (Windows, Android, alles was nicht als Apple erkannt wird)

  ```
  /vcard/robin_schroeter.vcf
  ```

</details>

---

### EMail & Telefon -> Bot Sicher - ohne Button

EMail Adressen:

```md
{{< data_hide "deine@email.de" >}}  
```

Telefonnummern

```md
{{< data_hide address="+49 123 456 789 00" protocol="tel" >}}  
```

---

### Optionale Dinge

<details>
<summary>Template für neue SVG Dateien</summary>

```svg
<svg viewBox="0 0 XX_width_XX XX_height_XX" class="apple_svg" version="1.1" aria-hidden="true" focusable="false" role="img" xmlns="http://www.w3.org/2000/svg">
  <g fill="currentColor">
    <path d="XXX"/>
    <path d="XXX"/>
  </g>
</svg>
```

</details>

