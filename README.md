
## Sassy SandBox  
A simple sass setup with Parcel for playing with css with live reloading.

![app screen shots](https://firebasestorage.googleapis.com/v0/b/images-aae96.appspot.com/o/sassy-sandbox.png?alt=media&token=079224cb-eef5-41d5-8b7f-ae4a37a3bdd9)

### Snippets
Grid styles using vars and calc:
```css

:root {
    --gap: 10px;
    --col-count: 3;
    --col-width: calc(100% / var(--col-count) - var(--gap));
    --grid: repeat(auto-fill, minmax(var(--col-width), 1fr));
}


.grid {
    display: grid;
    gap: var(--gap);
    margin: var(--gap);
    grid-template-columns: var(--grid);
    .card {
        margin: 0;
    }
}
```

Example of inline styles to span rows and cols in Grid for the first child of the Grid class (above)
```html
        <div class="grid">
                <div class="card" style="grid-column: 1 / 3; grid-row: 1 / 3;">
                    <h4>Some Stuff</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum aut quae at quos excepturi in.</p>
                </div>
                <div class="card">
                    <h4>Some Stuff</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum aut quae at quos excepturi in.</p>
                </div>
                {...}
```


### Run Locally:
Run the following commands in terminal from the root of the project:
```
npm install
npm run dev
```
