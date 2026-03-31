# Holding Space

The Holding Space website, built with [SvelteKit](https://svelte.dev/docs/kit/introduction) and configured to deploy to [Netlify](https://www.netlify.com/).

- [Staging site](https://holding-space.netlify.app/)
- Live TBC

## Install and Start

First, install the dependencies:

```sh
npm install
```

Start a development server (you can omit `-- --open` if you don't want it to open in a new tab automatically):

```sh
npm run dev -- --open
```

## Developing

This site is built with SvelteKit, with pages represented by `+page.svelte` files in the the [routes](/src/routes/) directory.

Individual UI elements such as headers, form inputs and blocks to display facilitator information are in the [components](/src/components/) directory.

Svelte files typically look and behave like this:

```svelte
<script>
  // Import other elements into this one
  // Functions to bring data in or out of this page or element
</script>

<html>
  // The HTML layout and text content of the page or element
</html>

<style>
  /* CSS styling for the elements in this page only */
</style>
```

So to update text content, look for it in the `<html>` section of a likely component. To update appearance, look in the `<style>` section, though some global styles may originate from the overall [+layout.svelte](/src/routes/+layout.svelte) file.

## Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.
