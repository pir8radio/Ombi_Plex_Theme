# Ombi Plex Theme Guide

## How to Use

To apply this theme in Ombi, follow these steps:

1. Navigate to `Ombi > Settings > Configuration > Customization > Custom CSS`.
2. Add the following line to import the theme from an external URL:
   ```css
   @import url("https://pir8radio.github.io/Ombi_Plex_Theme/theme.css");
   ```
- Alternatively, you can copy all the text from the [theme.css](https://raw.githubusercontent.com/pir8radio/Ombi_Plex_Theme/refs/heads/main/theme.css) file and paste it into your Custom CSS settings area.

## Additional Customizations

You can add the following custom CSS snippets to further customize your Ombi interface.

### Hide "Stream On" Services
This snippet hides the "Stream On" section in the interface:
```css
#streamingContainer {
    display: none;
}
.streaming-on {
    display: none;
}
```

### Hide "Open in Mobile" Button for Mobile Users
This snippet hides the "Open in Mobile" button when mobile users view the HTML version:
```css
#nav-openMobile {
    display: none !important;
}
```

### Hide "Requests" Button
This snippet hides the "Requests" button (only visible to admins of Ombi):
```css
#nav-featureSuggestion {
    display: none !important;
}
```

### Hide Local Login Options
This snippet disables local login options, allowing only Plex OAuth (Plex username/password) for login:
```css
#sign-in {
    display: none !important;
}
```

### Hide the Mobile APP links, button, and QR code in the users profile:
```
div[style*="margin-left: 4%;"] {
    display: none;
}
```

### Use a Logo Instead of a Large Title in the Top Left
This snippet replaces the large title in the top-left corner with a logo:
```css
.sidenav-container .sidenav .mat-toolbar.application-name {
    content: url("https://yourdomain.com/yourlogo.png");
}
```

---

Feel free to customize these snippets to suit your specific needs!
