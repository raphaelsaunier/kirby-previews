# Kirby Previews

Add some missing structure previews in the panel.

![screenshot](https://user-images.githubusercontent.com/14079751/50736950-dcab0080-11c3-11e9-9548-02a04cdacaaf.jpg)

<br/>

## 1. Installation

Download and copy this repository to ```/site/plugins/previews```

Alternatively, you can install it with composer: ```composer require sylvainjule/previews```

<br/>

## 2. Setup

That's it, no need for additional config. This plugin currently provides those field-previews : 

- Multiselect
- Structure
- Tags
- Toggle
- [Color](https://github.com/TimOetting/kirby-color)
- [Color-palette](https://github.com/sylvainjule/kirby-color-palette)
- [Locator](https://github.com/sylvainjule/kirby-locator)

<br/>

## 3. Add / edit a preview

- Clone the repo
- `cd` to your newly created folder (named `kirby-previews`, or whatever you have chosen)
- `npm install` to get all the dependencies (first, [install npm](https://www.npmjs.com/get-npm) if needed)
- There are two useful command lines:

```bash
# Dev mode
npm run dev

# Build plugin + autoprefix styles
npm run build
```

- Start by running the plugin in dev mode to benefit from hot-reload while working on your preview (`npm run dev`)
- Create a new preview under `src/components` (check the existing previews for how to structure content).
- Add your preview CSS in `src/assets/styles.scss`
- Register you new preview in `src/main.js` (check the existing previews for how to do this).
- Create a new preview under `src/components` (check the existing previews for how to structure content).
- Build the plugin (`npm run build`)
- Create a pull request

> You **must** run the build process before pushing the repo, else the hot-reload code will prevent it to work in any install.

<br/>

## 4. License

MIT