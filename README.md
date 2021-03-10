
## Sassy SandBox  
A simple sass setup with Parcel for playing with css with live reloading.

![app screen shots](https://firebasestorage.googleapis.com/v0/b/images-aae96.appspot.com/o/sassy-sandbox.png?alt=media&token=079224cb-eef5-41d5-8b7f-ae4a37a3bdd9)

### Snippets

```css
// Grid styles examples with vars and calc:

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


### Run Locally:
Run the following commands in terminal from the root of the project:
```
npm install
npm run dev
```
