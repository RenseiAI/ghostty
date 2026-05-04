<h3 align="center">
  Rensei for <a href="https://github.com/ghostty-org/ghostty">Ghostty</a>
</h3>

<p align="center">
  <a href="https://github.com/RenseiAI/ghostty/stargazers"><img src="https://img.shields.io/github/stars/RenseiAI/ghostty?colorA=111113&colorB=F97316&style=for-the-badge" alt="GitHub stars"></a>
  <a href="https://github.com/RenseiAI/ghostty/issues"><img src="https://img.shields.io/github/issues/RenseiAI/ghostty?colorA=111113&colorB=FB923C&style=for-the-badge" alt="GitHub issues"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=FAFAFA&colorA=111113&colorB=C2410C" alt="MIT license"></a>
</p>

Rensei terminal themes for Ghostty, built from the Rensei brand kits in `docs/brand/`.

## Themes

- `rensei-dark.conf`: the dark brand kit's code block palette: charcoal, muted comments, forge keywords, hot strings, and white identifiers.
- `rensei-light.conf`: the light brand kit's terminal treatment, which intentionally keeps code surfaces dark for syntax legibility.

## Usage

### Direct/Manual

1. Copy the theme files from [`themes/`](./themes/) into the `themes/` subdirectory of your Ghostty configuration directory:

   ```sh
   mkdir -p ~/.config/ghostty/themes
   cp themes/rensei-*.conf ~/.config/ghostty/themes/
   ```

2. Set one theme in your Ghostty configuration file:

   ```conf
   theme = rensei-dark.conf
   ```

   or:

   ```conf
   theme = rensei-light.conf
   ```

3. To follow your desktop light/dark appearance, set both:

   ```conf
   theme = light:rensei-light.conf,dark:rensei-dark.conf
   ```

4. Reload or restart Ghostty.

> [!NOTE]
> Ghostty looks for named custom themes in `~/.config/ghostty/themes/`. It also supports absolute paths. See the Ghostty [`theme` option reference](https://ghostty.org/docs/config/reference#theme).

## Palette Source

The colors are mapped from the Rensei brand system:

- Dark source: `docs/brand/rensei-brand-kit-v3-dark.html`
- Light source: `docs/brand/rensei-brand-kit-v3-light.html`

The terminal palette follows the brand kit's Code / Terminal section. Dark mode maps to the Rensei charcoal code block, with `#FB923C` keywords and `#FDBA74` strings. Light mode follows the kit's rule that code blocks stay dark, using `#1E1E2E`, `#CDD6F4`, `#FAB387`, and `#F9E2AF` for terminal legibility.
