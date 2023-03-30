# King-Size Homer

Simple game based on Homer Simpson's work-from-home computer terminal, as seen in the Season 7 episode of _The Simpsons_, "King-Size Homer".

I will be writing it using Svelte and TypeScript.

Due to me being new to the whole HTML canvas game thing, this game won't have a mobile-friendly version (for now).

## General concept

The bird bobs down when the player "presses the Any key", while the `Y` and `N` keys move from left to right independently, bumping into each other, thereby reversing direction.

The aim is to press `Y` every time. If one accidentally presses `N`, the text on the screen changes to something like "Venting prevents explosion. Are you sure you want to avoid it?", thereby making `N` the correct answer until the text changes back to default. You lose if you press `Y` at this point.

There will be some points scored along the way, and probably some increasing of speed of the letters as the game progresses.

**Potential special features:** a third key appears sometimes, called Tab, which you can peck to earn bonus points.

## To-do

1. ~~Set up TS and Svelte~~
2. ~~Draw wireframe and plan in more detail~~
3. ~~Set up Prettier~~
4. ~~Create page outlines with basic styling for mobile~~
5. ~~Create page outlines with basic styling for web~~
6. Plan exact gameplay design
7. Draw static canvas (is this a good first step?)
8. Animate bird on press of any key
9. Make `Y` and `N` keys move
10. Make keys bump into each other
11. Combine on-demand bird movement with moving keys
12. Update score when player hits correct key
13. Display score on screen
14. Change text when `N` is pressed
15. Create Start screen, as well as Pause screen and Game Over screens
16. Add ads
17. ...

## Svelte's README

## This repo is no longer maintained. Consider using `npm init vite` and selecting the `svelte` option or — if you want a full-fledged app framework — use [SvelteKit](https://kit.svelte.dev), the official application framework for Svelte

---

## svelte app

This is a project template for [Svelte](https://svelte.dev) apps. It lives at <https://github.com/sveltejs/template>.

To create a new project based on this template using [degit](https://github.com/Rich-Harris/degit):

```bash
npx degit sveltejs/template svelte-app
cd svelte-app
```

_Note that you will need to have [Node.js](https://nodejs.org) installed._

## Get started

Install the dependencies...

```bash
cd svelte-app
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:8080](http://localhost:8080). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.

If you're using [Visual Studio Code](https://code.visualstudio.com/) we recommend installing the official extension [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode). If you are using other editors you may need to install a plugin in order to get syntax highlighting and intellisense.

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).

## Single-page app mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for _any_ path. You can make it so by editing the `"start"` command in package.json:

```js
"start": "sirv public --single"
```

## Using TypeScript

This template comes with a script to set up a TypeScript development environment, you can run it immediately after cloning the template with:

```bash
node scripts/setupTypeScript.js
```

Or remove the script via:

```bash
rm scripts/setupTypeScript.js
```

If you want to use `baseUrl` or `path` aliases within your `tsconfig`, you need to set up `@rollup/plugin-alias` to tell Rollup to resolve the aliases. For more info, see [this StackOverflow question](https://stackoverflow.com/questions/63427935/setup-tsconfig-path-in-svelte).

## Deploying to the web

### With [Vercel](https://vercel.com)

Install `vercel` if you haven't already:

```bash
npm install -g vercel
```

Then, from within your project folder:

```bash
cd public
vercel deploy --name my-project
```

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public my-project.surge.sh
```
