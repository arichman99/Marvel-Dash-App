# Marvel Character and Comic Explorer
This Dash application allows users to explore Marvel Comics characters, their comic appearances, and connections to major events...

## Purpose
Discover insights into your favorite Marvel characters!...

## Features
- **Interactive Components**: Dropdown, Checklist, Date Picker Range, Text Input, Radio Buttons.
- **Visualizations**: Bar Chart, Line Chart, Network Graph, Word Cloud.
- **Reset Functionality**: Reset all filters with a button.

## Setup instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/marvel_dash_app.git
   cd marvel_dash_app
   
2. **Install dependencies**:
	pip install -r requirements.txt
	
3. **Set up API keys**:
	- Register at [Marvel Developer Portal](https://developer.marvel.com/) to obtain API keys.
	- Create a `.env` file in the root directory with:
	- MARVEL_PUBLIC_KEY=your_public_key
	- MARVEL_PRIVATE_KEY=your_private_key
	>Example: Replace placeholders with actual keys from the portal.
	
4. **Prepare data**:
	- Use the provided data/marvel_data.csv for instant access (recommended).
	- To fetch fresh data, run Cell 4 in marvel_dash_app.ipynb. Note: This can take ~1 hour due to API rate limits (3,000 calls/day). Ensure API keys are set.
	
5. **Run application**:
	- Execute all cells in marvel_dash_app.ipynb. Access at http://127.0.0.1:8050.
	
## Usage
	- **Character Selection**: Choose a character (e.g., "Spider-Man") from the dropdown.
	- **Filters**: Select comic formats, set a date range, or search for "Civil War" to see related comics.
	- **Output**: View appearances (bar), trends (line), connections (network), and titles (word cloud).

## Repository structure
```
marvel_dash_app/
├── .env.example
├── marvel_dash_app.ipynb
├── data/
│   ├── marvel_data.csv
├── requirements.txt
├── README.md
├── license.txt
```
## Data sources
	Marvel Comics API: Dynamic data on characters, comics, events.
	Static CSV: data/marvel_data.csv for offline use.
	Character List: From Comic Vine’s “Top 300 Most Published Marvel Characters”.
	
## Limitations
- The Marvel API has a 3,000 calls/day limit.
- Character aliases are not aggregated. For example, "Spider-Man" is recorded with ~400 comics, but has more appearances under aliases like Peter Parker or Miles Morales, treated as separate entities.
	
## Notes
	Marvel-themed colors (red #E6242A, gold #FFD700).
	Licensed under MIT. Data from Marvel Comics API.