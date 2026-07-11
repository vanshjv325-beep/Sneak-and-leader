# Digital Clock - Multi Timezone

A beautiful, real-time digital clock application that displays the current time across multiple time zones with local storage functionality.

## Features

✨ **Core Features:**
- 🕐 Real-time digital clock display (updates every second)
- 🌍 Support for multiple time zones simultaneously
- 💾 Persistent storage using browser localStorage
- 🎨 Modern, dark-themed UI with gradient effects
- 📱 Fully responsive design (mobile, tablet, desktop)
- ⚡ Smooth animations and hover effects
- 🗑️ Individual timezone deletion
- 🔄 Clear all timezones with one click

## Time Zone Support

Includes 13 preset time zones:
- **Americas:** New York (EST), Chicago (CST), Los Angeles (PST), Toronto (EST)
- **Europe:** London (GMT), Paris (CET)
- **Asia:** Tokyo (JST), Dubai (GST), India (IST), Singapore (SGT), Hong Kong (HKT)
- **Oceania:** Sydney (AEDT)

Plus support for **any valid IANA timezone**.

## How to Use

1. **Add a Timezone:**
   - Type a timezone name directly (e.g., `America/New_York`)
   - OR select from the dropdown preset list
   - Click "Add Timezone" or press Enter

2. **View Current Time:**
   - Each timezone displays:
     - Digital time (HH:MM:SS)
     - AM/PM indicator
     - Full date with day of week
     - UTC offset

3. **Remove Timezone:**
   - Click the "✕" button on any clock card

4. **Clear All:**
   - Click "Clear All" button to remove all clocks at once

## Valid IANA Timezone Examples

```
America/New_York
Europe/London
Asia/Tokyo
Australia/Sydney
America/Los_Angeles
Asia/Kolkata
Pacific/Auckland
Africa/Cairo
America/Mexico_City
```

[Full list of IANA timezones](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)

## Technical Details

- **Built with:** HTML5, CSS3, JavaScript (ES6+)
- **Storage:** LocalStorage API (persistent across sessions)
- **Time API:** Intl.DateTimeFormat (native JavaScript)
- **No Dependencies:** Pure vanilla JavaScript, no external libraries

## Features Explained

### Real-Time Updates
The clock updates every 1000ms (1 second) to display the current time with smooth precision.

### Local Storage
Your selected time zones are automatically saved to the browser's localStorage and restored when you visit again.

### Validation
Invalid time zones are rejected with an alert. Only valid IANA timezone identifiers are accepted.

### Responsive Design
- Grid layout adapts to screen size
- Desktop: 3-4 clocks per row
- Tablet: 2 clocks per row
- Mobile: 1 clock per row

## Browser Compatibility

Works on all modern browsers:
- Chrome/Chromium (v24+)
- Firefox (v25+)
- Safari (v10+)
- Edge (v15+)

## File Structure

```
digital-clock-timezones/
├── index.html          Main application file (self-contained)
└── README.md          Documentation
```

## Customization

Edit the preset timezones list in the HTML:
```html
<select id="presetSelect">
    <option value="Your/Timezone">Your Label</option>
</select>
```

Change the color scheme by modifying CSS variables in the `<style>` section.

## License

Open source, free to use and modify.

---

**Enjoy tracking time across the globe! 🌍⏰**
