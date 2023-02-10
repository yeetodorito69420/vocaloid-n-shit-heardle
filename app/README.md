[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/M4M2CHKFQ)

# How to remix this to make your own Heardle game

I remixed this from the [Loona Heardle](https://loona-heardle.glitch.me/). It's built in Svelte and is already compiled so it's not the easiest to read

If you want to remix it and make your own version, here's what you need to do:

## Glitch

- make an account here on Glitch
- click the "Remix to Edit" button in the top right corner

## The start date

This is the date that the first song in your tracks array will be played, and how the game keeps track of which is today's song.

- edit "public/main.js"
- the main page title is on line #3907
- change the start date to today (or whenever you want to start your game)
  ```
  startDate: "2022-06-14",
  ```

## Songs

- all the audio needs to come from Soundcloud, not any other streaming service
- edit "public/songs.js"
- the songs should go in the order you want the game to go
- add new items in the format (and remember the comma at the end)
  ```
  {
    url: "https://soundcloud.com/harrystyles/woman",
    answer: "Harry Styles - Woman",
  },
  ```
- use a hyphen `-` to split the artist and track, don't use other dashes
- try to choose tracks that aren't blocked in a lot of countries

At some point your game will stop working, and it's because it's gone through your list of songs.

You can fix this by duplicating the songs in the tracks array, or by changing the start date.

Note that if you change the start date, it will also reset the day number (eg `Harry Styles Heardle #80` will go back to `Harry Styles Heardle #1`), and might mess up people's scores.

## Title

- edit "public/main.js"
- the main page title is on line #711

## Feedback

- feedback like "Unlucky!" is at around line #3906

## Sharing image and metadata

- edit "public/main.js"
- do a search for "Harry Styles Heardle" and update the text with your Heardle name and description
- edit "src/pages/index.hbs" to change the page metatags
- open the assets tab and upload your own image
- copy the image URL and add that to the page metadata

## How to contact you

- replace my contact details with yours so that people can let you know if there is a bug, or if they love it!
- edit "public/main.js" at line #1240, #1643, #3859 or search for "derekahmedzai"

## Analytics

- go to google.com/analytics and sign up for your own Google Analytics account
- edit "src/pages/index.hbs" and replace the id in line 32, eg. `gtag('config', 'G-GPSR1C0Q60');`
- if you don't want to use Google Analytics you can remove that whole script block

<img src="https://cdn.glitch.global/ddbe8776-c33e-4a0d-8de4-6a536510547f/harry-styles-as-it-was.jpg?v=1649009749963">

---

# Hello Node (blank)

[Node.js](https://nodejs.org/en/about/) is a popular runtime that lets you run JavaScript on the server. This project uses the [Fastify](https://www.fastify.io/) framework and basic templating with [Handlebars](https://handlebarsjs.com/).

## What's in this project?

← `README.md`: That’s this file, where you can tell people what your cool website does and how you built it.

← `public/style.css`: The styling rules for your pages and posts.

← `server.js`: The main server script for your new site.

← `src/`: This folder holds page templates, additional scripts.

### Working in the `src/` folder 📁

← `src/pages/index.hbs`: This is the main page template for your site.

![Glitch](https://cdn.glitch.com/a9975ea6-8949-4bab-addb-8a95021dc2da%2FLogo_Color.svg?v=1602781328576)

## You built this with Glitch!

[Glitch](https://glitch.com) is a friendly community where millions of people come together to build web apps and websites.

- Need more help? [Check out our Help Center](https://help.glitch.com/) for answers to any common questions.
- Ready to make it official? [Become a paid Glitch member](https://glitch.com/pricing) to boost your app with private sharing, more storage and memory, domains and more.
