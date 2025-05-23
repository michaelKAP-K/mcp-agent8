# UI Theme Export

This directory contains automatically exported theme data from the UI component library for MCP service.

## Available Themes

A total of **20** themes were exported:

- **Default Theme** (default): A clean, modern light theme suitable for most application interfaces
- **Space Tech** (space-tech): Space tech style with dark backgrounds and bright cyan and blue accents, creating a futuristic feel
- **Dark Mode** (dark): A sleek dark mode theme with blue accents, providing reduced eye strain and modern aesthetics suitable for both professional and gaming applications
- **Mono Round** (mono-round): Minimalist rounded design with soft colors and large rounded elements for a modern look
- **Neon Arcade** (neon-arcade): Vibrant neon style with bright purples, blues and pinks, perfect for arcade or cyberpunk games
- **Dark RPG** (dark-rpg): Dark RPG style with deep tones and mysterious purple elements, suitable for role-playing games
- **Fantasy** (fantasy): Fantasy world theme with ancient styles and textures, perfect for medieval or magical games
- **Sci-Fi** (scifi): Sci-fi theme with futuristic blue tones and sharp edges, ideal for space or tech themed games
- **Retro** (retro): Retro style with pixel feel and vibrant contrasting colors, nostalgic game interface
- **Apocalypse** (apocalypse): Apocalypse style, dark and gritty tones, suitable for post-apocalyptic themes
- **Cyberpunk** (cyberpunk): Cyberpunk style with neon colors and future urban aesthetics
- **Candy** (candy): Candy style, bright and colorful, suitable for casual or children's games
- **Super Retro** (super-retro): Super retro style, 8-bit pixel art, extreme old-school game feel
- **Cartoon Game** (cartoon-game): Cartoon game style, lively and cute, suitable for casual games
- **Minimalist Dark** (minimalist-dark): Minimalist dark theme, clean and simple dark tone design
- **Glossy Cyan** (glossy-cyan): Glossy cyan theme, smooth surfaces and reflective effects, modern tech feel
- **Clash Style** (clash-style): Game UI style inspired by Clash of Clans with vibrant colors and visual hierarchy
- **Neon Teal** (neon-teal): Neon teal style, modern bright tones, suitable for fashionable game interfaces
- **Neon Blue** (neon-blue): Neon blue tones, cool neon effects with strong tech feel
- **Amber Gold** (amber-gold): Amber gold style, warm gold tones with luxurious feel

## Usage

### Get Theme List

```javascript
const themes = require('./themes-export/index.json');
console.log(themes.themes); // Basic info for all themes
```

### Get Specific Theme

```javascript
const themeInfo = require('./themes-export/themes/neon-arcade/theme.json');
const themeComponents = require('./themes-export/themes/neon-arcade/components.json');
```

## Structure

- `index.json`: Theme index and basic information
- `themes/{theme-name}/theme.json`: Detailed theme information and variables
- `themes/{theme-name}/components.json`: Theme component styles

## Auto Update

The contents of this directory are generated by the `export-themes.ts` script. Run the script when source files change to update the data.
