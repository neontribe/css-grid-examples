Example of css grids as layout. For each toggle-able piece of view furniture that needs to be accounted in the grid a new combination of the previous grids would need to be added. So for example: 4 optional pieces of view furniture = 15 css grids. Any additional pieces of view furniture will increase the number of css grid combinations at a fast rate.

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

...etc
```