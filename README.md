
# UFC Fighter Comparison App

A web app I built to compare UFC fighters side-by-side with interactive charts and real-time data. Because arguing about who's better should be backed by actual stats! 

**Live Demo**: https://combat-compare-8686dd813e69.herokuapp.com/

## What It Does

Ever wanted to compare two fighters, for example; Conor McGregor and Khabib Nurmagomedov, to see who's better at punching, grappling, or defending? My app makes this easy! 

But it's way more than just comparisons. You can:

### Fighter Comparisons & Profiles
- **Head-to-Head Analysis**: Compare any two fighters with interactive radar charts showing striking accuracy, takedown defense, knockout power, and more
- **Detailed Fighter Profiles**: Click on any fighter to see their complete stats, fight record (wins/losses/draws), physical stats (height, reach, weight), and career highlights
- **Visual Insights**: Instantly see who's better at what with color-coded charts and easy-to-read breakdowns
- **Data Context** statistical validity to prevent misleading rankings I used data from active UFC fighters to ensure fair comparisons. Fighters need minimum attempts to qualify - this prevents misleading stats like a 100% takedown accuracy based on just 2 attempts when the average fighter has 9 or more career takedown attempts.

### Live UFC Data
- **Current Rankings**: Browse official UFC rankings for all weight classes - from Flyweight to Heavyweight, plus Women's divisions and Pound-for-Pound lists
- **Upcoming Fight Cards**: Never miss an event! See all scheduled UFC fights with dates, venues, and main card matchups
- **Fighter Records**: Every fighter's complete UFC record with win/loss ratios and finish rates

### Smart Features
- **Fuzzy Search**: works well with misspellings 
- **Statistical Leaders**: See who leads each weight class in categories like most knockouts, highest takedown accuracy, or best striking defense
- **Mobile Friendly**: Works on your phone for accessing data anywhere

## Why I Built This

As an MMA fan, I was constantly frustrated trying to compare fighters. I'd have to:
- Check one site for basic stats
- Visit another for fight records  
- Hunt through forums for rankings
- Guess at who was actually better based on incomplete info

Most MMA sites either had outdated information, terrible mobile experiences, or made you dig through endless tables of numbers. I wanted something that could instantly show me "McGregor hits 4.5 strikes per minute vs Khabib's 3.1" with a visual that made sense.

Plus, I thought building a full-stack app around something I'm passionate about

### Key Features
- **Fighter Comparisons**: Compare striking, grappling, and defense stats with cool radar charts
- **Smart Search**: Finds fighters even if you spell their names wrong 
- **Statistical Leaders**: See who's the best at what in each weight class
- **Live Rankings**: Current UFC rankings that update automatically
- **Upcoming Events**: Never miss a fight card again
- **Mobile Friendly**: Works great on your phone

## Why I Built This

As an MMA fan, I was constantly frustrated trying to compare fighters. I'd have to:
- Check one site for basic stats
- Visit another for fight records  
- Hunt through forums for rankings
- Guess at who was actually better based on incomplete info..

Plus, I thought it would be a cool way to combine my love of MMA with learning full-stack development!

## How It Works

### The Tech Stack
- **Backend**: Python with Flask (handles all the logic)
- **Database**: MySQL hosted on AWS (stores all the fighter data)
- **Frontend**: HTML/CSS/JavaScript with some fancy charts
- **Hosting**: Heroku (so anyone can use it)
- **Data Updates**: Automated scripts that grab fresh data weekly

### The Data Pipeline
Every week, my app automatically:
1. **Scrapes** the latest fighter stats from public MMA sources
2. **Cleans** the messy data 
3. **Updates** the database with fresh numbers
4. **Caches** everything for fast loading

This means you always get current stats without me having to manually update thousands of fighters.

## What I Learned

Building this taught me a ton about:
- **Full-stack development** 
- **Data scraping and cleaning** 
- **Cloud deployment** (AWS, and Heroku)
- **Performance optimization** 
- **User experience**

## Technical Details

### Database Structure
- **Fighter Stats**: 2,400+ fighters with 50+ statistical categories and  9,000+ fights from 1996 to present 
- **Events**: Upcoming fight cards and schedules  
- **Rankings**: Official UFC rankings by weight class
- **Eligibility Rules**: Smart filtering to avoid ambiguous stats



## Screenshots

*see screenshots*
- Fighter comparison with radar charts
- Statistical leaders page  
- UFC rankings
- Mobile responsive design

## Future Ideas

- Historical fight analysis
- More advanced visualizations;; round by round visualizations career stats  
- User accounts and favorites
- Fight outcome predictions

## Setup (For Developers)

Since this is a portfolio project, the full source code is private. But here's the general setup:

```bash
# Environment variables needed
DB_HOST=your-aws-rds-endpoint
DB_NAME=comp_site_ufc_db  
DB_USER=admin
DB_PASS=your_password

# Main dependencies
Flask==2.0.1
mysql-connector-python==8.0.26
pandas==1.3.3
beautifulsoup4==4.9.3
```

## Contact

Want to see the code or chat about the project? Hit me up!

Email : combatcompare@gmail.com

**Note**: Source code is private but available for review by recruiters or potential collaborators.

---

*Built with passion and way too much coffee by a student who loves both coding and combat sports*
