# Playa - An HTML5 audio player

A simple utility to hotlink audio content.

## Why

Many people I send audio streams to ~~don't know how to~~ [face difficulties](#common-difficulties) with playing those streams back in a media player of their choice. This utility lets me hotlink any audio or video stream in it and plays back the audio stream.

This way, I can share content with others in the plain form of URLs and be sure it can play right in their browser, as long as the codec is supported.

## Usage

Playa can be used in two ways:

1. Using the on-site form to hotlink content on the player.

2. Using the URL itself to load content directly on the player.

To do the later, you may add a `?src=` after the URL of the player and paste in the direct link to your source. This should load it on the player and this whole URL is sharable with others.

Example:

[https://pgram1.github.io/playa/?src=http://radio.plaza.one/mp3](https://pgram1.github.io/playa/?src=http://radio.plaza.one/mp3)

The whole execution of the utility is done locally, live. No reloads needed.

## Common Difficulties

(Those are all anecdotal and depend on the user's platform and prefered browser. Solutions are provided for justification of some design choices.)

- In-browser player has no controls or they are too close or overlapping one another, making the audio stream a very loud trap.

✔️ The reason the inline CSS of my utility has fixed proportions.

- What's a media player?

✔️ No need to know, here you go :)

- Audio stream is not started in-browser and instead starts downloading infinitely on the device.

✔️ The whole purpose of creating this utility!

- The audio played is not the one in the URL!

✔️ That's what the reset button is for.
