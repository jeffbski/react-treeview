# React-treeview

Easy, light, flexible treeview made with [React](http://facebook.github.io/react/).

Modified from Cheng Lou's version to not display the arrow in the code, but yet allow it to be driven by CSS. Allow additional classes to be applied to the open or collapsed tree icon so font-awesome can be used to set icons. Alternatively CSS content can be used to set the text content to display for the icon (if not using something like font-awesome).


## install

Npm:
```sh
npm install jeffbski/react-treeview#font-awesome
```

The CSS file:

```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css">
<link rel="stylesheet" type="text/css" href="path/to/react-treeview.css">
```

## API

#### &lt;TreeView />
The component accepts [three props](https://github.com/chenglou/react-treeview/blob/07132c6ad33a7b94d479eae60e84a0f02b2126da/src/react-treeview.jsx#L5-L7).

- `collapsed`: whether the node is collapsed or not.
- `defaultCollapsed`: the [uncontrolled](http://facebook.github.io/react/docs/forms.html#uncontrolled-components) equivalent to `collapsed`.
- `nodeLabel`: the component or string (or anything renderable) that's displayed beside the TreeView arrow.
- `iconOpenClassNames`: string of space separated additional classNames to apply to the uncollapsed icon. Modify to set the opened icon to a font-awesome icon like `fa fa-minus-square`
- `iconCollapsedClassNames`: string of space separated additional classNames to apply to the collapsed icon. Modify to set the collapsed icon to a font-awesome icon like `fa fa-plus-square`

**Note:** No icon is displayed by default, so either use `iconOpenClassNames` and `iconCollapsedClassNames` or use CSS content to define the icon to be used.

TreeViews can be naturally nested.

The extra properties are transferred onto the icon, so all attributes and events naturally work on it.

## Styling
The CSS is flexible, commented and made to be easily customized. Feel free to inspect the demo's classes and check the short CSS code.

## Build It Yourself/Run the Demos

Build: `npm install && npm run prerelease`

Demos: `npm install && npm start && open http://localhost:3000`

## License

MIT.
