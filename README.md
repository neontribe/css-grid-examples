# CSS Grid Examples

This is a small repository of grid examples. The examples are from the perspective of the highest level of layout. Where content can contain any of the "main" content of the document.
- [The index.html](https://neontribe.github.io/css-grid-examples/index.html) file shows an example of a "holy grail" grid layed out using css grid.
- [missing.html](https://neontribe.github.io/css-grid-examples/missing.html) shows several examples of the same grid with missing components.
- [missing.fix.html](https://neontribe.github.io/css-grid-examples/missing.fix.html) shows the same set of examples as missing.html, but with a potential clean fix to erroneous whitespace left over by the missing grid areas

For each toggle-able piece of view furniture that needs to be accounted in the grid a new combination of the previous grids would need to be added. So for example: 4 optional pieces of view furniture = 16 css grids. 2<sup>n</sup> combinations are required, where n is the number of optional components.

e.g.
```css
.hg.grid_main {
	grid-template-areas: "main";
	grid-template-columns: 1fr;
	grid-template-rows: 1fr;
	min-height: 100vh;
}

.hg.grid_main-right {
	grid-template-areas: "main ads";
	grid-template-columns: 1fr 150px;
	grid-template-rows: 1fr;
	min-height: 100vh;
}

.hg.grid_main-left {
	grid-template-areas: "main ads";
	grid-template-columns: 1fr 150px;
	grid-template-rows: 1fr;
	min-height: 100vh;
}

.hg.grid_main-header {
	grid-template-areas: "main ads";
	grid-template-columns: 1fr 150px;
	grid-template-rows: 1fr;
	min-height: 100vh;
}

.hg.grid_main-footer {
	grid-template-areas: "main ads";
	grid-template-columns: 1fr 150px;
	grid-template-rows: 1fr;
	min-height: 100vh;
}

...etc
```