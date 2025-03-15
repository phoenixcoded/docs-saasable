# Tabler

## Tabler outline icons

The minified `tabler-sprite-outline.svg` file is already included here: `public/assets/svg`, allowing you to use any of the Tabler stroke icons. To add an icon, simply reference its name from the [icon list](https://tabler.io/icons).

To add a new Tabler outline icon, refer to the [icon list](https://tabler.io/icons) and get the icon name.&#x20;

Use the format <mark style="color:purple;">tabler-\[iconname]</mark> in your code. Here's an example:

{% tabs %}
{% tab title="src/blocks/pricing/Pricing5.tsx" %}
<pre class="language-typescript"><code class="lang-typescript">// import common components
import SvgIcon from '@/components/SvgIcon';

&#x3C;SvgIcon
    name="tabler-check" // Make sure this name available in tabler outline icon
<strong>    type={IconType.STROKE} // It is the default set so no need to add this for this icon
</strong>    size={16} // Change icon size
    color="text.secondary" // Change icon color
    stroke={2} // Change icon stroke width
/>
</code></pre>
{% endtab %}
{% endtabs %}

## Tabler fill icons

We have created a separate file, `tabler-sprite-fill.svg` , located in the `public/assets/svg` path.&#x20;

{% hint style="warning" %}
Only the usable fill SVG icons are included in this file at this moment.
{% endhint %}

### How can I add new fill icons?

1.  To add a new fill icon, copy the SVG code from the [icon list](https://tabler.io/icons).\


    {% code overflow="wrap" %}
    ```svg
    <!-- Copy svg code -->
    <svg  xmlns="http://www.w3.org/2000/svg"  width="24"  height="24"  viewBox="0 0 24 24"  fill="currentColor"  class="icon icon-tabler icons-tabler-filled icon-tabler-star">
      <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
      <path d="M8.243 7.34l-6.38 .925l-.113 .023a1 1 0 0 0 -.44 1.684l4.622 4.499l-1.09 6.355l-.013 .11a1 1 0 0 0 1.464 .944l5.706 -3l5.693 3l.1 .046a1 1 0 0 0 1.352 -1.1l-1.091 -6.355l4.624 -4.5l.078 -.085a1 1 0 0 0 -.633 -1.62l-6.38 -.926l-2.852 -5.78a1 1 0 0 0 -1.794 0l-2.853 5.78z" />
    </svg>
    ```
    {% endcode %}
2. Include the above code in the `tabler-sprite-fill.svg` file. between the SVG tag
3.  Customize as per other icons already added

    1. Replace SVG with **symbol tag**
    2. **Remove width & height** attributes
    3. Also, **remove the class & add id** attributes with a specific name, here is an example:\
       Remove: `class="icon icon-tabler icons-tabler-filled icon-tabler-star"`\
       Add: `id="tabler-filled-star"`

    <pre class="language-javascript" data-title="tabler-sprite-fill.svg file"><code class="lang-javascript">&#x3C;!-- Customize final code -->
    &#x3C;symbol xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" id="tabler-filled-star">
      &#x3C;path stroke="none" d="M0 0h24v24H0z" fill="none"/>
    <strong>  &#x3C;path d="M8.243 7.34l-6.38 .925l-.113 .023a1 1 0 0 0 -.44 1.684l4.622 4.499l-1.09 6.355l-.013 .11a1 1 0 0 0 1.464 .944l5.706 -3l5.693 3l.1 .046a1 1 0 0 0 1.352 -1.1l-1.091 -6.355l4.624 -4.5l.078 -.085a1 1 0 0 0 -.633 -1.62l-6.38 -.926l-2.852 -5.78a1 1 0 0 0 -1.794 0l-2.853 5.78z" />
    </strong>&#x3C;/symbol>  




    </code></pre>

    &#x20;
4.  After adding a new svg then use this svg id in your files

    <pre class="language-typescript" data-title="Icon.tsx file (example)"><code class="lang-typescript">// import common components
    import SvgIcon from '@/components/SvgIcon';

    &#x3C;SvgIcon
    <strong>    name="tabler-filled-star" // Add id which is added in tabler-sprite-fill.svg
    </strong><strong>    type={IconType.FILL} // Change icon type for fill icon
    </strong>    size={16} // Change icon size
        color="text.secondary" // Change icon color
    />
    </code></pre>


5. The icon has been successfully added! 👍
