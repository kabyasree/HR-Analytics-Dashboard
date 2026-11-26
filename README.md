# HR Attrition Dashboard (Power BI)

An interactive dashboard that looks at why employees leave, and who is most likely to.

![image](<img width="1528" height="859" alt="PHOTO-2026-11-04-19-19-29" src="https://github.com/user-attachments/assets/7ace732e-8590-4bfc-91d3-b42bb1618635" />
)

## Why I built this

Companies often talk about attrition in vague terms like "people just leave." I wanted to see what the data actually says. This dashboard breaks attrition down by age, salary, role and department, so a manager can see where people are leaving from instead of guessing.

## What I found

- **Ages 26-35 have the most exits.** This group accounts for 116 employees who left, the highest of any age band. It points to a gap in career growth around the mid-level stage.
- **Attrition drops once salary passes 5k.** Below that mark people leave much more often, so 5k looks like a floor for keeping staff in this dataset.
- **Laboratory Technicians and Sales Executives leave the most.** Both roles are either physically or mentally demanding, so burnout or competing offers could be behind it. I can't confirm the cause from this data alone.

## How I built it

**Power Query (cleaning and prep)**
- Handled missing values and standardised job role names.
- Grouped raw age and salary into Age Groups and Salary Slabs, since bands are easier to read in a report than individual values.

**DAX (measures)**
- Attrition Rate = employees who left ÷ total employees. I used a rate instead of raw counts so large and small groups can be compared fairly.
- Added Department slicers (Sales, R&D, HR) so you can filter the whole dashboard down to one team.

**Design**
- Dark background with neon accents, so the two main KPIs (Attrition Count and Attrition Rate) catch the eye first.
- The page reads top to bottom: overall numbers first, then the breakdowns by salary, role and tenure.

## What I'd recommend

1. **Look at the "Up to 5k" salary bracket first.** It has the most turnover, so pay or growth for entry-level roles is the place to start.
2. **Focus on the 26-35 group.** Mentoring or clearer promotion paths could help.
3. **Run stay interviews with Laboratory Technicians.** 62 of them left, and asking current staff what's wearing them down is cheaper than losing more.

## How to open it

1. Download the `.pbix` file from this repo.
2. Open it in Power BI Desktop.
3. Use the Department filter at the top right to explore each team.

 [LinkedIn](https://www.linkedin.com/in/kabyasree-hazarika/).
