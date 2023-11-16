# krueckeKontaktTheme

## Features

## Installation

1. Git Submodule installieren

    ```shell
    git submodule add https://github.com/cljoly/gohugo-shorturl.git themes/gohugo-shorturl
    git submodule add https://github.com/martignoni/hugo-cloak-email.git themes/hugo-cloak-email
    git submodule add https://github.com/jpanther/lynx.git themes/lynx
    ```

2. Config

    ```toml
    theme = [
      "krueckeKontaktTheme",
      "hugo-cloak-email",
      "gohugo-shorturl",
    ]
    ```

3. Starte den Server mit `hugo server`. Die Module werden automatisch heruntergeladen.

4. Ersetze die `config.toml` mit der config Datei: [download a copy]( DOWNLOADLINK https://minhaskamal.github.io/DownGit/#/home ) .

### Git Submodule deinstallieren

    ```shell
    git submodule deinit themes/gohugo-shorturl
    git rm themes/gohugo-shorturl
    ```


## Configuration

Kontaktdaten vor Bot's verstecken  

    ```go
    {{< cloakemail "jane.doe@example.com" >}}
    ```

### Optional parameters

- Use `protocol` to specify the protocol: `{{< cloakemail address="jane.doe@example.com" protocol="xmpp" >}}` or `{{< cloakemail address="+1 212 664-7665" protocol="tel" >}}`
- Use `display` to display any text on the page instead of the address: `{{< cloakemail address="jane.doe@example.com" display="Send us a mail!" >}}`
- Use `class` to indicate CSS classes to use: `{{< cloakemail address="jane.doe@example.com" class="vip company-a" >}}`
- Use `query` to specify a e-mail subject or other URI parameters (URI query): `{{< cloakemail address="jane.doe@example.com" query="subject=Message from contact form" >}}`. The query is never printed on the web page.