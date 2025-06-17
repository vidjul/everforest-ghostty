# Everforest Theme for Ghostty

Custom [Everforest](https://github.com/sainnhe/everforest) port for [Ghostty](https://ghostty.org/) terminal emulator. Official theme only had dark hard variant.

## Available Themes

### Dark Variants

- **everforest-dark-hard** - High contrast dark theme
- **everforest-dark-medium** - Medium contrast dark theme (recommended)
- **everforest-dark-soft** - Low contrast dark theme

### Light Variants

- **everforest-light-hard** - High contrast light theme
- **everforest-light-medium** - Medium contrast light theme (recommended)
- **everforest-light-soft** - Low contrast light theme

## Installation

### Download individual themes

Create the themes directory if it doesn't exist:

```bash
mkdir -p "$HOME/.config/ghostty/themes"
```

Download the theme you want:

```bash
# Dark themes
curl -o "$HOME/.config/ghostty/themes/everforest-dark-hard" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-dark-hard
curl -o "$HOME/.config/ghostty/themes/everforest-dark-medium" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-dark-medium
curl -o "$HOME/.config/ghostty/themes/everforest-dark-soft" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-dark-soft

# Light themes
curl -o "$HOME/.config/ghostty/themes/everforest-light-hard" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-light-hard
curl -o "$HOME/.config/ghostty/themes/everforest-light-medium" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-light-medium
curl -o "$HOME/.config/ghostty/themes/everforest-light-soft" https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/everforest-light-soft
```

### Download all themes at once

```bash
# Create themes directory
mkdir -p "$HOME/.config/ghostty/themes"

# Download all themes
for theme in everforest-dark-hard everforest-dark-medium everforest-dark-soft everforest-light-hard everforest-light-medium everforest-light-soft; do
  curl -o "$HOME/.config/ghostty/themes/$theme" "https://raw.githubusercontent.com/vidjul/everforest-ghostty/main/themes/$theme"
done
```

## Usage

After installing the themes, edit your Ghostty configuration file (`$HOME/.config/ghostty/config`) and add your theme name. e.g:

```
...
theme = everforest-dark-medium
...
```

Replace `everforest-dark-medium` with your preferred theme name.

You can sync theme with OS by prefixing with dark and light keywords:

```
theme = dark:everforest-dark-medium,light:everforest-light-medium
```
