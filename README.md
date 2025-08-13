IPL Analysis (Power BI)
A simple, insightful Power BI dashboard to explore IPL match, team, and player performance across seasons.
Focus areas include season winners, Orange/Purple Cap trends, toss impact, venue analysis, and top player stats.

🔧 Tech & Files
Tool: Power BI Desktop (.pbix), SQL

Main File: IPL_Analysis(BI).pbix

📊 Key Features
Season Overview: champions, finalists, most wins, win %.

Team Performance: wins/losses by season, head-to-head, chasing vs. defending.

Player Insights: Orange Cap (runs), Purple Cap (wickets), best strike rate/economy.

Toss & Match Outcome: toss decision impact by venue/season.

Venue Analysis: batting/bowling friendly grounds, average scores.

Interactive Slicers: season, team, player, venue.

🧠 Measures (Examples)
Add/adjust to match your model

Total Runs = SUM(deliveries[total_runs])
Total Wickets = CALCULATE(COUNTROWS(deliveries), deliveries[is_wicket] = 1)
Matches Played = DISTINCTCOUNT(matches[id])
Win % = DIVIDE([Wins], [Matches Played], 0)
📁 Data Model (Typical)
matches (match_id, season, date, team1, team2, toss_winner, toss_decision, winner, venue)

deliveries (match_id, over, ball, batting_team, bowling_team, batter, bowler, total_runs, is_wicket)

players (player_id, player_name, batting_style, bowling_style, team_history)

Create relationships: matches[id] 1—* deliveries[match_id], and map player/team dimensions as needed.

🚀 How to Use
Clone the repo

git clone https://github.com/<your-username>/<your-repo>.git
Open IPL_Analysis(BI).pbix in Power BI Desktop.

If you use external CSVs, update Transform Data → Data Source Settings to point to your local paths.

Refresh the model and explore the report pages.

📷 Screenshots
Add images to a screenshots/ folder and reference them here.
