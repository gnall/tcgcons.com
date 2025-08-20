# tcgcons.com
Simple app for tracking upcoming TCG Conventions http://tcgcons.com/

# Contributing

We welcome contributions to help expand our event database! Here's how you can add new events to the project:

## How to Contribute Events

### 1. Fork the Repository
- Click the "Fork" button at the top right of this repository
- This creates a copy of the project in your GitHub account

### 2. Clone Your Fork
```bash
git clone https://github.com/YOUR_USERNAME/REPOSITORY_NAME.git
cd REPOSITORY_NAME
```

### 3. Create a New Branch
```bash
git checkout -b add-new-events
```

### 4. Add Your Events
- Open `eventdata.json` in your preferred editor
- Add your new events following the existing JSON structure
- Ensure your JSON is valid and properly formatted
- Include all required fields for each event

### 5. Commit Your Changes
```bash
git add eventdata.json
git commit -m "Added <EVENT_NAME_AND_DATE>"
```

### 6. Push to Your Fork
```bash
git push origin add-new-events
```

### 7. Open a Pull Request
- Go to your fork on GitHub
- Click "New Pull Request"
- Select your branch (`add-new-events`) as the source
- Provide a clear description of the events you've added
- Submit the pull request

## Event Data Format

Each event should follow this JSON structure:

```json
{
  "name": "MagicCon Atlanta 2025",
  "organizer": "Wizards of the Coast", 
  "region": "US East",
  "date": "September 26-28, 2025",
  "location": "Georgia World Congress Center",
  "city": "Atlanta, GA",
  "formats": "Pro Tour, Side Events, Artist Alley, Cosplay",
  "tcgs": "Magic the Gathering",
  "link": "https://mcatlanta.mtgfestivals.com/en-us.html",
  "status": "Upcoming"
}
```

### Required Fields

- **name**: Full event name
- **organizer**: Company or organization hosting the event
- **region**: Geographic region (e.g., "US East", "Europe", "Asia Pacific")
- **date**: Event dates in "Month DD-DD, YYYY" or "Month DD, YYYY" format
- **location**: Venue name
- **city**: City and state/country
- **formats**: Event types/activities (comma-separated)
- **tcgs**: Trading card games featured
- **link**: Official event website URL
- **status**: Current status ("Upcoming", "Past", "Cancelled", etc.)

## Event Data Guidelines

When adding events to `eventdata.json`, please ensure:
- All required fields are included and follow the format above
- Dates are in the specified format
- Event information is accurate and verified
- No duplicate events are added
- JSON syntax is valid (use a JSON validator if unsure)

## Questions?

If you have questions about contributing or need help with the process, please open an issue and we'll be happy to help!

# Disclaimer
All code created using Generative AI (Primarily Claude).
