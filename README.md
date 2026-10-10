# Bricks

[Русская версия](README.ru.md)

A browser brick-breaker set on a building site. Keep the steel ball in play with a hazard-striped paddle and break every brick in the wall.

**[Play in the browser](https://posoxai.github.io/Bricks/)**

<p>
  <img src="screenshots/day.png" width="300" alt="Bricks in the light theme with the Russian interface: level 3, a half-broken wall of coloured and cracked bricks, the ball in flight">
  <img src="screenshots/night.png" width="300" alt="The same game in the dark theme with the English interface: level 6, a wall framed by steel bricks">
</p>

Left: the light theme with the Russian interface. Right: the dark theme with the English one.

## Rules

- You have three balls. A ball that falls past the paddle is lost; the next one waits on the paddle.
- The further from the middle of the paddle the ball lands, the steeper it flies off. Every hit on the paddle makes the ball a little faster.
- A level is cleared when every breakable brick is gone.
- After the sixth level the levels come round again, faster each time.

## Bricks

| Brick | What it takes | Points |
| --- | --- | --- |
| Coloured | one hit | 10 |
| Strong, dark | two hits; cracks after the first | 20 |
| Steel, with bolts | never breaks, not needed to clear the level | — |

A cleared level adds 100 points times its number.

## Capsules

A broken brick sometimes drops a capsule. Catch it with the paddle.

| Picture | Effect |
| --- | --- |
| Bar with two arrows | A wider paddle for 18 seconds |
| Hourglass | A slower ball for 14 seconds |
| Three dots | Every ball in play splits into three |
| Heart | An extra ball, up to five |

The capsules carry pictures rather than letters, so they read the same in both languages.

## Controls

- Mouse: the paddle follows the pointer, a click launches the ball.
- Phone: drag a finger anywhere on the field and the paddle follows the movement, so the finger never hides it. A tap launches the ball.
- Keyboard: arrow keys or A and D move the paddle, Space or the up arrow launches the ball, P or Esc pauses.

The game pauses by itself when you leave the tab. An unfinished game, the best score and the settings are kept in the player's browser; a reload brings back the same wall with the ball on the paddle.

## Language

The interface is in English and Russian. It opens in Russian when Russian is among the browser's languages and in English otherwise. The RU/EN switch remembers your choice.

## How to run

The whole game is one file, `index.html`. There is no build step and there are no dependencies.

- Locally: open `index.html` in a browser.
- Online: the game is published with GitHub Pages at https://posoxai.github.io/Bricks/. Every commit to `main` updates it automatically.

Fonts load from Google Fonts. Without a network the game falls back to system fonts.

## Visit counter

The published page counts visits with [GoatCounter](https://www.goatcounter.com/). According to the service, it sets no cookies and stores no personal data. The counter does not run when `index.html` is opened from disk.

## Credits

The game was written by Claude, the AI assistant made by Anthropic: the logic and physics, the six levels, the canvas graphics, the sound and the page design.

The rules come from the brick-breaker games: Breakout (Atari, 1976) and Arkanoid (Taito, 1986). The name, the levels and the design of this version are its own.

The idea of making a browser version came from posoxAI.

## License

MIT. The full text is in [LICENSE](LICENSE).
