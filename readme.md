# VS Code Custom CSS & JS Setup

A custom configuration to enhance VS Code's appearance with modern styling, blur effects, and interactive features.

## 📁 Files Location

Both files should be placed in your `C://` directory:

```
C://
├── vscode-custom.css
└── vscode-custom.js
```

## 🚀 Installation

### 1. Install Required Extension

Install the **Custom CSS and JS Loader** extension:
- Open VS Code
- Go to Extensions (`Ctrl+Shift+X`)
- Search for "Custom CSS and JS Loader" by be5invis
- Install it

### 2. Configure VS Code Settings

Open your VS Code `settings.json` (`Ctrl+Shift+P` → "Preferences: Open Settings (JSON)") and add:

```json
{
  "vscode_custom_css.imports": [
    "file:///C://vscode-custom.css",
    "file:///C://vscode-custom.js"
  ],
  "vscode_custom_css.policy": true
}
```

### 3. Enable Custom CSS

- Press `Ctrl+Shift+P`
- Type "Enable Custom CSS and JS"
- Select it and restart VS Code

## ✨ Features

### CSS Customizations
- 🎨 **Custom Fonts**: JetBrains Mono for editor, Geist Mono for UI
- 🌈 **Modern Scrollbars**: Rounded, purple-themed scrollbars
- 💫 **Blur Effects**: Command palette with backdrop blur
- 🎯 **Explorer Styling**: Enhanced file tree with custom fonts
- 📊 **Status Bar**: Lighter font weight for cleaner look
- 🔍 **Tooltips**: Glassmorphism effect with gradient backgrounds
- 🎮 **Command Palette**: Centered, styled with blur backdrop

### JavaScript Enhancements
- 🌫️ **Background Blur**: Automatically blurs background when Command Palette opens
- ⌨️ **Keyboard Shortcuts**: 
  - `Ctrl+P` / `Cmd+P`: Opens Command Palette with blur
  - `Esc`: Closes palette and removes blur
- 👁️ **Widget Management**: Hides sticky widgets during Command Palette
- 🔄 **Auto-detection**: Monitors Command Palette state dynamically

## 🎨 Color Scheme

Primary accent color: `#bc9abc` (Purple)
- Scrollbars
- Explorer title
- Active highlights
- Borders and accents

## ⚙️ Customization

### Change Accent Color

Find and replace `#bc9abc` in `vscode-custom.css` with your preferred color:

```css
/* Example: Change to blue */
color: #4a90e2 !important;
background: #4a90e2 !important;
```

### Adjust Blur Intensity

In `vscode-custom.css`, modify the blur value:

```css
#command-blur {
  backdrop-filter: blur(8px); /* Change 8px to your preference */
}
```

### Change Fonts

Update font families in `vscode-custom.css`:

```css
font-family: 'Your Font Name', monospace !important;
```

## 🔧 Troubleshooting

### Custom CSS not loading?
1. Make sure file paths use `file:///` prefix (three slashes)
2. Verify files are actually in `C://` directory
3. Run "Reload Custom CSS and JS" command
4. Restart VS Code completely

### Permission errors?
- Run VS Code as Administrator (Windows)
- Check that `"vscode_custom_css.policy": true` is set

### Blur effect not working?
- Ensure JavaScript file is loaded
- Check browser console: `Ctrl+Shift+I` → Console tab
- Verify no JavaScript errors

## 🔄 Updates

After modifying CSS or JS files:

1. Press `Ctrl+Shift+P`
2. Type "Reload Custom CSS and JS"
3. Restart VS Code

## 📝 Notes

- **Windows**: Use `file:///C://filename.ext`
- **Mac/Linux**: Use `file:///path/to/filename.ext`
- Changes require VS Code restart to take effect
- Some updates may require running "Enable Custom CSS and JS" again

## ⚠️ Important

- This modifies VS Code installation files
- Updates to VS Code may reset customizations
- Always backup your files
- Re-run "Enable Custom CSS and JS" after VS Code updates

## 🤝 Need Help?

If something isn't working:
1. Check the Console for errors (`Ctrl+Shift+I`)
2. Verify file paths are correct
3. Ensure extension is enabled
4. Try disabling other extensions temporarily

---

**Enjoy your customized VS Code! 🎉**


ref: https://www.youtube.com/watch?v=9_I0bySQoCs
