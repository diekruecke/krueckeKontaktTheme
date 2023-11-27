+++
title = 'Button Test Area'
date = 2023-10-27T03:04:27+01:00
draft = true
+++

<style>
  .lastedit, .subtitle, .template_hinweis {
    text-align: center;
  }
  .link-email_down, .link-phone_down, .link-contact_down {
    background: blue;
  }
  .link-email_full_down, .link-phone_full_down, .link-contact_full_down {
    background: green;
  }
  .link-email_circle_down, .link-phone_circle_down, .link-contact_circle_down {
    background: darkorange;
  }
  .link-email_circle_full_down, .link-phone_circle_full_down, .link-contact_circle_full_down {
    background: grey;
  }
</style>

{{< kontakt_button_hidden type="email_down" href="deine@email.de" text="icon_down" >}}
{{< kontakt_button_hidden type="phone_down" protocol="tel" href="+1234567890123" text="icon_down" >}}
{{< kontakt_button href="#" type="contact_down" text="icon_down" >}}

{{< kontakt_button_hidden type="email_full_down" href="deine@email.de" text="icon_full_down" >}}
{{< kontakt_button_hidden type="phone_full_down" protocol="tel" href="+1234567890123" text="icon_full_down" >}}
{{< kontakt_button href="#" type="contact_full_down" text="icon_full_down" >}}

{{< kontakt_button_hidden type="email_circle_down" href="deine@email.de" text="icon_circle_down" >}}
{{< kontakt_button_hidden type="phone_circle_down" protocol="tel" href="+1234567890123" text="icon_circle_down" >}}
{{< kontakt_button href="#" type="contact_circle_down" text="icon_circle_down" >}}

{{< kontakt_button_hidden type="email_circle_full_down" href="deine@email.de" text="icon_circle_full_down" >}}
{{< kontakt_button_hidden type="phone_circle_full_down" protocol="tel" href="+1234567890123" text="icon_circle_full_down" >}}
{{< kontakt_button href="#" type="contact_circle_full_down" text="icon_circle_full_down" >}}
