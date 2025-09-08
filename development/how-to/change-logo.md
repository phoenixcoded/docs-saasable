# Change Logo

SaasAble admin offers a unique feature that allows you to replace all your branding elements from a single location, enabling you to launch your product faster. We provide a `branding.json` file where you can simply replace the values with your own brand properties.

{% hint style="warning" %}
Any reference to logos and branding in **images** will not be replaced automatically by this guide. You will need to manually update and replace those images with your own.
{% endhint %}

{% code title="src/branding.json" %}
```json
{
    "brandName": "SaasAble",
    "company": {
        "name": "Phoenixcoded",
        "url": "https://phoenixcoded.authordesk.app/"
    },
    "logo": {
        "main":"",
        "logoIcon": ""
    }
}
```
{% endcode %}

### Logo Guidelines

You need to provide the path of your logo in the `src/branding.json`, and the code will use the specified logo instead of the default SaasAble logo. If no path is provided, the SaasAble logo will be used by default. For each logo, there are size guidelines to ensure a better site experience, please check the below guidelines for each logotype:

<table><thead><tr><th width="203"></th><th width="266">main</th><th>logoIcon</th></tr></thead><tbody><tr><td>Size</td><td>140x27</td><td>37x40</td></tr><tr><td>Format</td><td>Image Format</td><td>Image Format</td></tr></tbody></table>

> Providing image logos will not change the color when updated using the customizer. If you need the logo color to change dynamically at runtime, please use an SVG format, similar to the one used for SaasAble logos.
