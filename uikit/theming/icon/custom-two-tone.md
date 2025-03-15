# Custom/two tone

## Custom/Twotone icon

We have created a separate file, `sprite-custom.svg` , located in the `public/assets/svg` path. Only the usable SVG icons are included in this file.

{% hint style="info" %}
Avoid using hex codes (e.g., `#EADDFF`) directly for stroke and fill colors. Follow these steps to customize your new icon properly.
{% endhint %}

### Here are the steps to add a new two-tone icon:

1.  Download the new two-tone SVG icon which you need to use, open it & copy SVG code

    <pre class="language-svg" data-overflow="wrap"><code class="lang-svg">&#x3C;!-- Copy svg code -->
    &#x3C;svg <a data-footnote-ref href="#user-content-fn-1">width="40" height="40"</a> viewBox="0 0 40 40" <a data-footnote-ref href="#user-content-fn-1">fill="none"</a> xmlns="http://www.w3.org/2000/svg">
        &#x3C;g clip-path="url(#clip0_185_40650)">
            &#x3C;path d="M20 24.5L24.8776 16.8229C24.7632 17.0487 25.1003 16.7029 24.8776 16.8229C24.992 16.5971 25.0347 16.3417 25 16.0909C24.9653 15.8401 24.8548 15.6059 24.6833 15.4198C24.5119 15.2337 24.2877 15.1046 24.0408 15.0497L8.5 12.5L14.0443 30.0402C14.0992 30.2873 14.2283 30.5117 14.4142 30.6833C14.6001 30.8548 14.834 30.9653 15.0844 31C15.3349 31.0347 15.5899 30.9918 15.8153 30.8772C16.0407 30.7626 16.2258 30.5817 16.3456 30.3588L18.5044 27.1596" <a data-footnote-ref href="#user-content-fn-1">fill="#EADDFF"</a>/>
            &#x3C;path d="M29.1451 24.8833L24.6301 20.37L29.8184 16.8867C30.1776 16.6932 30.4691 16.3945 30.6537 16.0306C30.8382 15.6668 30.9071 15.2552 30.8511 14.8511C30.795 14.4469 30.6167 14.0696 30.3401 13.7697C30.0635 13.4698 29.7017 13.2617 29.3034 13.1733L6.66675 6.66666L13.1734 29.2717C13.262 29.6699 13.4703 30.0314 13.7703 30.3079C14.0703 30.5843 14.4477 30.7624 14.8518 30.8183C15.2559 30.8741 15.6674 30.8051 16.0311 30.6204C16.3948 30.4357 16.6934 30.1442 16.8867 29.785L20.3701 24.63L21.6784 25.9383" <a data-footnote-ref href="#user-content-fn-1">stroke="#1D1B20" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"</a>/>
            &#x3C;path d="M25 31.6667L28.3333 35L35 28.3333" <a data-footnote-ref href="#user-content-fn-1">stroke="#1D1B20" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"</a>/>
        &#x3C;/g>
        &#x3C;defs>
            &#x3C;clipPath id="clip0_185_40650">
                &#x3C;rect width="40" height="40" fill="white"/>
            &#x3C;/clipPath>
        &#x3C;/defs>
    &#x3C;/svg>
    </code></pre>
2. Include the above code in the `sprite-custom.svg` file. between the SVG tag
3.  Customize as per other icons already added

    1. Replace SVG with **symbol tag**
    2. **Remove** **width & height** attributes & **add id** name&#x20;
    3. If symbol has `fill="none"` then **remove it** & **add** `stroke="currentcolor" stroke-linecap="round"`
    4. **Remove** `stroke="#1D1B20" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"` all attributes from where the path contains these attributes & with this **add** `fill='none'` also
    5. For secondary **fill color change**, `fill="#EADDFF"` **remove it** & **add** `data-two-tone="true" style="stroke-width:0" opacity="0.4"`
    6. **Remove defs** whole code then the final output like the below code example:

    <pre class="language-svg" data-title="sprite-custom.svg file" data-overflow="wrap"><code class="lang-svg">&#x3C;!-- Customize svg -->
    <strong>&#x3C;symbol viewBox="0 0 40 40" id="custom-arrow" stroke="currentcolor" stroke-linecap="round" xmlns="http://www.w3.org/2000/svg">
    </strong>    &#x3C;g clip-path="url(#clip0_185_40650)">
            &#x3C;path d="M20 24.5L24.8776 16.8229C24.7632 17.0487 25.1003 16.7029 24.8776 16.8229C24.992 16.5971 25.0347 16.3417 25 16.0909C24.9653 15.8401 24.8548 15.6059 24.6833 15.4198C24.5119 15.2337 24.2877 15.1046 24.0408 15.0497L8.5 12.5L14.0443 30.0402C14.0992 30.2873 14.2283 30.5117 14.4142 30.6833C14.6001 30.8548 14.834 30.9653 15.0844 31C15.3349 31.0347 15.5899 30.9918 15.8153 30.8772C16.0407 30.7626 16.2258 30.5817 16.3456 30.3588L18.5044 27.1596" data-two-tone="true" style="stroke-width:0" opacity="0.4" />
            &#x3C;path d="M29.1451 24.8833L24.6301 20.37L29.8184 16.8867C30.1776 16.6932 30.4691 16.3945 30.6537 16.0306C30.8382 15.6668 30.9071 15.2552 30.8511 14.8511C30.795 14.4469 30.6167 14.0696 30.3401 13.7697C30.0635 13.4698 29.7017 13.2617 29.3034 13.1733L6.66675 6.66666L13.1734 29.2717C13.262 29.6699 13.4703 30.0314 13.7703 30.3079C14.0703 30.5843 14.4477 30.7624 14.8518 30.8183C15.2559 30.8741 15.6674 30.8051 16.0311 30.6204C16.3948 30.4357 16.6934 30.1442 16.8867 29.785L20.3701 24.63L21.6784 25.9383" fill="none"/>
            &#x3C;path d="M25 31.6667L28.3333 35L35 28.3333" fill="none"/>
        &#x3C;/g>
    &#x3C;/symbol>
    </code></pre>



    Now you can compare copy svg with customize svg&#x20;
4.  After adding a new svg then use this svg id in your files

    <pre class="language-typescript" data-title="Pricing2.tsx"><code class="lang-typescript">// import common components
    import SvgIcon from '@/components/SvgIcon';

    &#x3C;SvgIcon
    <strong>    name="custom-arrow" // Add id which is added in sprite-custom.svg file
    </strong><strong>    type={IconType.CUSTOM} // Change icon type for twotone icon
    </strong>    color="primary.main" // Change outline color of icon
        stroke={3} // Change stroke width of the icon
        twoToneColor={theme.palette.background.default} // Change secondary fill color
    />
    </code></pre>
5. The icon has been successfully added! 👍

[^1]: 
