# \<my-project\>



## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.

```
Custom CSS Properties

https://www.smashingmagazine.com/2017/04/start-using-css-custom-properties/

https://www.sitepoint.com/practical-guide-css-variables-custom-properties/

```


```
What is CSS preprocessors?
- LESS and SASS are the CSS prepocessors
- They make use of variables and mixins to define style
- Avoid copy pasting of css code
- They store color, font preferences and layout related properties
```

```
Limitations of Preprocessors
- Cannot be change dynamically
- They not aware of DOM structure
- They cannot be changed from javascript
- LESS uses @ and SASS uses $ as prefixes
- They have their code language which has to be learned before implemented
- Different declaration method
```

```
These limiations made a base to invent CSS Custom Properties by a WWW community
```

```
CSS Custom Properties uses simple -- (two dash)
- learn once and implement and works through all browsers
- CSS variables is written as var()

///Variables with fallback value
.box {
    padding: var(--box-padding, 10px);
    color: var(--box-color, #ff0088);
}

///CSS mixin
--box: {
    padding: var(--box-padding, 10px);
    color: var(--box-color, #ff0088);
}

///apply mixin
.your-box {
    @apply --box;
}
```

```
Browser Support
- All modern browsers support
- IE Edge fully support, but older version does not have full support 
```

```
What is Polymer?
Polymer is a JavaScript library that helps you create custom reusable HTML elements, and use them to build performant, maintainable apps.
```

```
Web Components Basic things to consider
- Should be re-usable with respect to styling and functionality.
- So will be able to use it in any project and multiple projects.
- Dont style elements if you don't have any specified VD from designer, keep it raw.
- Create CSS styles only if it is designed intentionally as per requirement.
- If you need to write a CSS styles than use variables with fallback values.
- That means fallback values will be applied in your component.
- And those variables will be used in the project theme CSS style to override the fallback value of that component.
```

```
Project Shared Style
- Its a custom theme style of the project.
- We can pre define the variables style of the elements.
- Keep design of the element same all through.
- If the external component has variables with fallback values shared style will not affect it.
- If you need to override those use the redefine the variables of the component in shared style.
```

```
Create an project base svg icon set here
https://poly-icon.appspot.com

Create a html file named myicons.html in project
Copy the icon generated code in html file
and use it
<link rel="import" href="/path/to/myicons.html">
<iron-icon icon="myicons:ICON_NAME"></iron-icon>
```

```
```



