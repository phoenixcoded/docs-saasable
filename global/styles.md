# Styles

Global styles are centralized in one place and can be added in `src/app/globals.css`. Any new global styles should be added there.

{% tabs %}
{% tab title="VITE(TS)" %}
{% code title="src/main.tsx" %}
```css
/* simpebar styles */
import 'simplebar-react/dist/simplebar.min.css';
```
{% endcode %}
{% endtab %}

{% tab title="VITE(JS)" %}
{% code title="src/main.jsx" %}
```css
/* simpebar styles */
import 'simplebar-react/dist/simplebar.min.css';
```
{% endcode %}
{% endtab %}

{% tab title="NEXT(TS)" %}
{% code title="src/app/globals.css" %}
```css
/* simpebar styles */
@import 'simplebar-react/dist/simplebar.min.css';

/* public styles */
@import '../../public/assets/styles/index.css';

```
{% endcode %}
{% endtab %}

{% tab title="NEXT(JS)" %}
{% code title="src/app/globals.css" %}
```css
/* simpebar styles */
@import 'simplebar-react/dist/simplebar.min.css';

/* public styles */
@import '../../public/assets/styles/index.css';

```
{% endcode %}
{% endtab %}
{% endtabs %}
