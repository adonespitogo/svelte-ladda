# svelte-ladda

Buttons with loading indicators for Svelte

### Install
```

npm i --save svelte-ladda

```

### Usage

Include styles:

```javascript
import 'ladda/dist/ladda-themeless.min.css';
```
or

```javascript
import 'ladda/dist/ladda.min.css';
```

In your component:

```html

<Ladda
  ladda="{ladda}
  class="btn btn-primary"
  style="{style}" 
  color="{color}
  size="{size}
  spinnersize="{spinnersize}"
  ...
  />

<script>

import Ladda from 'svelte-ladda';

export default {
  components: { Ladda },
  data: () => {
    return {
      ladda: true,            // show loading spinner
      class: '',              // additional classe(s) for button
      style: 'expand-left',   // data-style ladda option
      color: 'purple',        // data-color ladda option
      size: 'medium',         // data-size ladda option
      spinnersize: 35,        // data-spinner-size ladda option
      spinnercolor: '#000',   // data-spinner-color ladda option
      spinnerlines: 12,       // data-spinner-lines ladda option
      progress: 0             // passed ladaElement.setProgress()
    };
  }
}

</script>

```

### Supported Events

 - onclick(event)
 - onmousedown(event)
 - onmouseup(event)
 - onmouseover(event)

### Todo
 - Unit tests

### License

MIT

