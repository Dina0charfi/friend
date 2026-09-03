# The Cat Code 🐱🔒

A cute, personalized lock-screen surprise made for a friend. They enter a secret code, get asked (sweetly, and repeatedly if they say no 🙈) whether they want to see their surprise, type their name, and get a lucky cat sticker that's unique to them — plus a heartfelt message. At the end, they can fill in a Snoopy photo-booth filmstrip with their own photos and save it.

## Features

- 🔐 Phone lock-screen style secret code entry, with a soft hint
- 🐑 Cute sheep stickers reacting as they hesitate to say yes
- 🐈 12 possible lucky cat stickers — the same name always gets the same cat
- 💌 A warm, personal message on reveal
- 📸 A Snoopy photo-booth strip: take a photo or upload one for each of the 5 frames, then save the finished strip as an image
- 📱 Works on both phone and desktop

## Deploying

This is a static site — no build step, no dependencies.

1. Go to [vercel.com/new](https://vercel.com/new) and sign in
2. Drag this folder onto the page (or connect this repo)
3. Vercel gives you a live link (e.g. `your-project.vercel.app`) to send to your friend

## Notes

- The secret code is set in `index.html` (search for `PASSWORD`)
- Cat and sheep art is in `assets/`
- There's no backend: the page quietly pings [ntfy.sh](https://ntfy.sh) so you know when someone unlocks it — no account needed, just open the topic URL in a browser or the ntfy app
