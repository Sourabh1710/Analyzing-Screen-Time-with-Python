# Analyzing Screen Time

## Getting Started
For the task of analyzing my screen time, I need data about my app usage activity on a particular device. This dataset contains features like:

- **Date**: The date on which the data was recorded.
- **App**: The name of the application being used (e.g., Instagram, WhatsApp).
- **Usage (minutes)**: The total number of minutes spent on the app daily.
- **Notifications**: The number of notifications received from the app each day.
- **Times Opened**: The number of times the app was opened on the recorded day.

## Analyzing Screen Time with Python
I start by importing the necessary Python libraries and the [dataset](https://statso.io/screen-time-case-study/).

### Summary Statistics
Before moving forward, I take a quick look at the summary statistics of the dataset.

### Screen Time Trends Over Time
I analyze the screen time trends of all the apps in the data over time.

![Screen Time Trends](https://github.com/Sourabh1710/Analyzing-Screen-Time-with-Python/blob/main/images/Screen%20Time%20Trends%20for%20Different%20Apps.png)

The graph illustrates my screen time usage of various apps throughout August 2024:
- **Instagram** shows the most fluctuating and high usage, peaking around mid-August and August 26.
- **X, WhatsApp, and Netflix** generally show lower and more consistent usage.
- **Safari and 8 Ball Pool** exhibit significant variability, with 8 Ball Pool peaking around August 11.
- **LinkedIn and Facebook** maintain relatively low and stable usage throughout.
- **Instagram dominates** my screen time, while other apps experience occasional spikes but lower overall engagement.

## Relationship Between Screen Time, Notifications, and App Openings

![Pair Plot](https://github.com/Sourabh1710/Analyzing-Screen-Time-with-Python/blob/main/images/Relationships%20between%20Screen%20Time%2C%20Notifications%2C%20and%20Times%20Opened.png)

The pair plot shows:
- A **moderate positive correlation** between notifications and times opened.
- A **moderate correlation** between times opened and usage minutes, indicating that more notifications lead to more app usage and openings.
- A **weaker correlation** between usage and notifications, suggesting that receiving many notifications does not always result in higher screen time.
- Most data points cluster around low values for usage, notifications, and times opened.

## Top Apps Based on Screen Time
Now, I analyze the top apps based on screen time and break down the average usage, notifications, and times opened per app.

### Key Insights:
- **Instagram**: Leads in screen time (76 min/day) and notifications (49), being opened around 41 times daily.
- **WhatsApp**: Ranks second in times opened (68/day) with the highest notifications (~100), but lower screen time than Instagram and Netflix.
- **Netflix**: I spend significant time (72 min/day) but have low interaction (2.56 opens/day, almost no notifications), indicating long continuous sessions (e.g., watching shows).
- **Other Apps**: Facebook, LinkedIn, and Safari have lower usage and interaction metrics.

## Average Screen Time by Day of the Week

![Average Screen Time by Day](https://github.com/Sourabh1710/Analyzing-Screen-Time-with-Python/blob/main/images/Average%20Screen%20Time%20Usage%20per%20Day%20of%20the%20Week.png)

- **Monday (48.6 min) and Wednesday (46.5 min)** show the highest usage.
- **Friday (27.1 min) has the lowest usage**.
- **Saturday (41.4 min) and Sunday (35.8 min) show moderate usage**.
- This suggests higher screen engagement during workdays and moderate usage over the weekend.

## Daily Patterns for Top Three Apps

![Daily Patterns](https://github.com/Sourabh1710/Analyzing-Screen-Time-with-Python/blob/main/images/Average%20Daily%20Usage%20for%20Instagram%2C%20Netflix%2C%20and%20WhatsApp.png)

- **Instagram** peaks on **Saturday (91.0 min)** and **Wednesday (90.4 min)**.
- **Netflix** has high engagement on **Wednesday (110.0 min)** and **Saturday (78.8 min)**.
- **WhatsApp** usage is highest on **Sunday (59.0 min)** and **Wednesday (76.0 min)**.
- **Wednesday and Saturday** show the highest overall screen time for these apps.

## Calculating the Probability of App Openings Through Notifications
To calculate the probability of opening an app after receiving a notification:

[ P(Open | Notification) = \frac{\text{Number of days the app was opened when notifications were received}}{\text{Total number of days notifications were received}} \]

![Probability](https://github.com/Sourabh1710/Analyzing-Screen-Time-with-Python/blob/main/images/Probability.png)

For all listed apps (**8 Ball Pool, Facebook, Instagram, LinkedIn, Netflix, Safari, WhatsApp, and X**), the probability is **1.0**, meaning I open the app **every time a notification is received**. 

### Insight:
- **Notifications are highly effective** in prompting my engagement.
- **To reduce screen time, turning off notifications** could be an effective strategy.

## Summary
- **Instagram dominates** my engagement, with high usage peaks on **Monday, Wednesday, and Saturday**.
- **Netflix has strong mid-week and weekend engagement**, while WhatsApp shows moderate usage throughout.
- **I open apps every time a notification is received**, indicating a strong response to notifications.

---

## Author
Sourabh Sonker <br>
Data Scientist
