# Branding

SaasAble offers a unique feature that allows you to replace all your branding elements from a single location, enabling you to launch your SaaS product faster. We provide a `branding.json` file where you can simply replace the values with your own brand properties.

{% hint style="warning" %}
Any reference to logos and branding in **images** will not be replaced automatically by this guide. You will need to manually update and replace those images with your own.
{% endhint %}

{% tabs %}
{% tab title="src/branding.json" %}
```json
{
  "brandName": "SaasAble",
  "title": "React Multipurpose UI Kit and Dashboard Template",
  "company": {
    "name": "Phoenixcoded",
    "url": "https://phoenixcoded.net",
    "socialLink": {
      "linkedin": "https://in.linkedin.com/company/phoenixcoded",
      "instagram": "#",
      "facebook": "https://www.facebook.com/Phoenixcoded/",
      "youtube": "https://www.youtube.com/@Phoenixcoded",
      "github": "https://github.com/phoenixcoded",
      "dribble": "https://dribbble.com/Phoenixcoded",
      "discord": "https://discord.com/invite/AfJqqYeG",
      "support": "https://support.phoenixcoded.net"
    }
  },
  "logo": {
    "main": "",
    "logoIcon": "",
    "logoFab": "",
    "logoWatermark": ""
  }
}
```
{% endtab %}
{% endtabs %}



### Logo Guidelines

You need to provide the path of your logo in the `src/branding.json`, and the code will use the specified logo instead of the default SaasAble logo. If no path is provided, the SaasAble logo will be used by default. For each logo, there are size guidelines to ensure a better site experience, please check the below guidelines for each logotype:

<table><thead><tr><th width="116"></th><th>main</th><th>logoIcon</th><th>logoFab</th><th>logoWatermark</th></tr></thead><tbody><tr><td>Size</td><td>140x27</td><td>37x40</td><td>94x94</td><td>430x466</td></tr><tr><td>Format</td><td>Image Format</td><td>Image Format</td><td>Image Format</td><td>Image Format</td></tr></tbody></table>

> Providing image logos will not change the color when updated using the customizer. If you need the logo color to change dynamically at runtime, please use an SVG format, similar to the one used for SaasAble logos.
