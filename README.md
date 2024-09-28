# JavaScript Utilities

A collection of reusable JavaScript utilities for web development.

## Table of Contents
- [notifications.js](#notificationsjs)
- [listButtons.js](#listbuttonsjs)

---

## notifications.js

### Usage
```javascript
showNotification(type, time, text);
```

#### Parameters
- **type**: Notification type (integer)
  - `1`: success (green)
  - `2`: error (red)
  - `3`: info (blue)
  
- **time**: Duration the notification will be displayed (milliseconds)
- **text**: Notification message (string)

---

## listButtons.js

### Usage
```javascript
initOverlay(modalID, modalClass, overlayID, overlayClass, buttonID, mainURL);
```

#### Parameters
- **modalID**: ID of the modal to initialize
- **modalClass**: Class name for the modal
- **overlayID**: ID of the overlay
- **overlayClass**: Class name for the overlay
- **buttonID**: ID of the button
- **mainURL**: Base URL to redirect when button is pressed

#### Definition of `listButton`
```javascript
const listButton = [
  {
    icon: "iconname",       // Name of the icon (leave empty to hide)
    iconType: "icontype",   // Type of the icon
    content: "string",      // Button content (string)
    m: 1,                   // Month (1-12)
    d: 1,                   // Day (1-31)
    y: 1999,                // Year
    size: "0B",             // Size (e.g., "0B")
    path: "download" // File path for redirection
  }
];
```

When the button is pressed, it will redirect to `mainURL + filepath`, for example:  
`"https://example/redirect?link=" + "home"`  
If `icon` is left empty, the icon will not be displayed. If `mainURL` is left empty, it will directly redirect to `path`.

---

Feel free to contribute or suggest improvements!
