# Marketing-Analytics-Projects
This Repo includes my collection of all the Data Science projects created in domain of Marketing.

## 1. Performance Analysis of YouTube Channel 
### Introduction

This project analyzes YouTube channel performance data to uncover insights about subscriber growth, engagement levels, and content performance trends. Using Python (Pandas, Matplotlib, Seaborn) for data cleaning and analysis, this project demonstrates how data analytics can be applied to real-world digital marketing and influencer analysis.

The objective of this analysis is to:
- Understand how subscribers, views, and engagement metrics relate.
- Identify top-performing channels based on key performance indicators (KPIs).
- Provide actionable insights that can help creators, marketers, and agencies make data-driven decisions.


### About Dataset
This [dataset](https://www.kaggle.com/datasets/positivealexey/youtube-channel-performance-analytics/data) provides an in-depth look at YouTube video analytics, capturing key metrics related to video performance, audience engagement, revenue generation, and viewer behavior. Sourced from real video data, it highlights how variables like video duration, upload time, and ad impressions contribute to monetization and audience retention. This dataset is ideal for data analysts, content creators, and marketers aiming to uncover trends in viewer engagement, optimize content strategies, and maximize ad revenue. Inspired by the evolving landscape of digital content, it serves as a resource for understanding the impact of YouTube metrics on channel growth and content reach.

Video Details: Columns like Video Duration, Video Publish Time, Days Since Publish, Day of Week.

Revenue Metrics: Includes Revenue per 1000 Views (USD), Estimated Revenue (USD), Ad Impressions, and various ad revenue sources (e.g., AdSense, DoubleClick).

Engagement Metrics: Metrics such as Views, Likes, Dislikes, Shares, Comments, Average View Duration, Average View Percentage (%), and Video Thumbnail CTR (%).

Audience Data: Data on New Subscribers, Unsubscribes, Unique Viewers, Returning Viewers, and New Viewers.

Monetization & Transaction Metrics: Details on Monetized Playbacks, Playback-Based CPM, YouTube Premium Revenue, and transactions like Orders and Total Sales Volume (USD).


### Dataset Descriptions

| Column Name                        | Description                                                                 |
|------------------------------------|-----------------------------------------------------------------------------|
| id                                 | Unique video identifier.                                                    |
| video_duration                     | Video length in seconds.                                                    |
| video_publish_time                 | Date and time of video publication.                                         |
| days_since_publish                 | Days since video was published.                                             |
| day                                | Day of month video was published.                                           |
| month                              | Month video was published.                                                  |
| year                               | Year video was published.                                                   |
| day_of_week                        | Day of week video was published.                                            |
| revenue_per_1000_views_usd         | Revenue per 1,000 views (RPM), in USD.                                      |
| monetized_playbacks_estimate        | Estimated ad-shown playbacks (±2% error).                                    |
| playback_based_cpm_usd             | Revenue per 1,000 monetized playbacks, in USD.                              |
| cpm_usd                            | Revenue per 1,000 ad impressions, in USD.                                   |
| ad_impressions                     | Number of ad impressions served.                                            |
| estimated_adsense_revenue_usd      | Estimated AdSense revenue, in USD.                                          |
| doubleclick_revenue_usd            | Estimated DoubleClick revenue, in USD.                                      |
| youtube_ads_revenue_usd            | Estimated YouTube-sold ads revenue, in USD.                                 |
| watch_page_ads_revenue_usd         | Revenue from watch page ads, in USD.                                        |
| youtube_premium_usd                | Revenue from YouTube Premium, in USD.                                       |
| transaction_revenue_usd            | Revenue from memberships, Super Chat, etc., in USD.                         |
| transactions                       | Number of transactions (e.g., memberships, Super Chat).                     |
| revenue_from_transactions_usd      | Revenue from transactions, in USD.                                          |
| reactions                          | Total likes and dislikes.                                                   |
| chat_messages_count                | Number of live stream or premiere chat messages.                            |
| reminders_set                      | Number of reminders set for live streams/premieres.                         |
| stream_hours                       | Total live streaming hours.                                                 |
| remix_views                        | Views on remixes of the video.                                              |
| remix_count                        | Number of remixes created from the video.                                   |
| subscribers_from_posts             | Subscribers gained from community posts.                                    |
| new_comments                       | Number of new comments on the video.                                        |
| shares                             | Number of video shares.                                                     |
| like_rate                          | Ratio of likes to views or engagements.                                     |
| dislikes                           | Number of dislikes.                                                         |
| likes                              | Number of likes.                                                            |
| unsubscribes                       | Number of unsubscribes linked to video.                                     |
| new_subscribers                    | Number of new subscribers gained.                                           |
| returned_items_usd                 | Value of returned transaction items, in USD.                                |
| unconfirmed_commissions_usd        | Unconfirmed affiliate/partner commissions, in USD.                          |
| approved_commissions_usd           | Approved affiliate/partner commissions, in USD.                             |
| orders                             | Number of orders via YouTube Shopping.                                      |
| total_sales_volume_usd             | Total sales value from orders, in USD.                                      |
| end_screen_click_through_rate      | End screen clicks divided by impressions.                                   |
| end_screen_impressions             | Number of end screen element impressions.                                   |
| end_screen_clicks                  | Number of end screen element clicks.                                        |
| teaser_click_through_rate          | Card teaser clicks divided by impressions.                                  |
| teaser_impressions                 | Number of card teaser impressions.                                          |
| teaser_clicks                      | Number of card teaser clicks.                                               |
| card_click_through_rate            | Card clicks divided by impressions.                                         |
| card_impressions                   | Number of card impressions.                                                 |
| card_clicks                        | Number of card clicks.                                                      |
| views_per_playlist_start           | Average views per playlist start (web only).                                |
| playlist_views                     | Views of videos in playlist context.                                        |
| playlist_watch_time_hours          | Total playlist watch time in hours.                                         |
| clip_watch_time_hours              | Total clip watch time in hours.                                             |
| clip_views                         | Number of clip views.                                                       |
| youtube_premium_watch_time_hours   | Watch time by YouTube Premium members, in hours.                            |
| youtube_premium_views              | Views by YouTube Premium members.                                           |
| returning_viewers                  | Estimated returning viewers.                                                |
| new_viewers                        | Estimated new viewers in last 28 days.                                      |
| average_views_per_user             | Average views per unique viewer.                                            |
| unique_viewers                     | Estimated distinct viewers in time period.                                  |
| watched_not_skipped                | Views or ad impressions not skipped.                                        |
| feed_impressions                   | Impressions from YouTube feed.                                              |
| average_view_percentage             | Average percentage of video watched.                                        |
| average_view_duration              | Average watch time per view, in seconds.                                    |
| views                              | Total video views.                                                          |
| watch_time_hours                   | Total watch time in hours.                                                  |
| subscribers                        | Net subscriber change (gained - lost).                                      |
| estimated_revenue_usd              | Total estimated revenue from all sources, in USD.                           |
| impressions                        | Number of thumbnail impressions on YouTube.                                 |
| video_thumbnail_ctr                | Thumbnail views divided by impressions.                                     |
| revenue_from_transactions_usd      | Revenue from transactions, in USD.                                          |
| reactions                          | Total likes and dislikes.                                                   |
| chat_messages_count                | Number of live stream or premiere chat messages.                            |
| reminders_set                      | Number of reminders set for


### References
- Dataset: [Kaggle - YouTube Channel Performance Analytics](https://www.kaggle.com/datasets/positivealexey/youtube-channel-performance-analytics/code)
- Libraries used:
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `numpy`


### Contact Information
- Email: mihir.d1234@gmail.com
- Linkedin: https://www.linkedin.com/in/mihirdamania/
