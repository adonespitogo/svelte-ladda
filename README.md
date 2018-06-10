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
  class="{class}"
  style="{style}" 
  color="{color}
  size="{size}
  spinnersize="{spinnersize}"
  spinnercolor="{spinnercolor}"
  spinnerlines="{spinnerlines}"
  progress="{progress}">

  This is a submit button

</Ladda>
```

```javascript
<script>

import Ladda from 'svelte-ladda';

export default {
  components: { Ladda },
  data: () => {
    return {
      ladda: true,                // show loading spinner
      class: 'btn btn-primary',   // additional classe(s) for button
      style: 'expand-left',       // data-style ladda option
      color: 'purple',            // data-color ladda option
      size: 'medium',             // data-size ladda option
      spinnersize: 35,            // data-spinner-size ladda option
      spinnercolor: '#000',       // data-spinner-color ladda option
      spinnerlines: 12,           // data-spinner-lines ladda option
      progress: 0                 // passed to ladaElement.setProgress()
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

```
Copyright (c) <year> <copyright holders>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

