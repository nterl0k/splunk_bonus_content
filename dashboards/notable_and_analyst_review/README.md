# Notable and Analyst Review Dashboard 
A rough effort at pulling forward analyst and notable metrics for team/detection tuning needs.

## Requirements: 
- SA-Investigator (used for tab.js/tab.css content)
- This App is helpful and this dashboard leverages it's tab content, cause i'm lazy.
 
## Optional / Extras
- Includes "On Glass" and "Test Content" concession if neded.
  - "On Glass"
    - Helpful if your team as specific hours they are eye's on, this will adjust the data displayed so that metrics are more accurate.
    - The timeframe may be edited in the top level query.
    - If your team doesn't have time on glass/business hour it can be ignored, it defaults to "all" 
  -  "Test Content" status
     -  This is a custom status that can be leveraged to flag dev/test content.
     -  It can be helpful during initial content tuning to prevent analyst time waste/metric skew
        -  Create a custom status called "Test Content" and set as a "closed" state
        -  Notables under development or testing can be set to the "Test Content" state.
   
## How to build
- Create a new "classic"(XML) dashboard
- Name it "notable and analyst review" or whatever you wish
- Copy the XML from [Notable and Analyst Review](https://github.com/nterl0k/splunk_bonus_content/blob/main/dashboards/notable_and_analyst_review/notable_and_analyst_review.xml) into the source/code for the dashboard
- Save/Use
- Add premissions/deploy to ES navigation as appropriate
  
## How to use
- Tab "Overview"
  - This is the general overview tab with simple at a glance metrics, helpful for spot checking.
  - ![screenshot](https://github.com/nterl0k/splunk_bonus_content/blob/main/dashboards/notable_and_analyst_review/notable_overview.png)

- Tab "Analyst Details"
  - This is helpful for analyst metrics
    - Time to touch/close
    - Affinity for specific alerts
    - Count over time trending
    - Comment/close note details.
  - ![screenshot](https://github.com/nterl0k/splunk_bonus_content/blob/main/dashboards/notable_and_analyst_review/analyst_effort_1.png)
  - ![screenshot](https://github.com/nterl0k/splunk_bonus_content/blob/main/dashboards/notable_and_analyst_review/analyst_effort_2.png)

- Tab "Notable Details"
  - This is helpful for examining detections that fire often and the metrics associated with them
    - How often they fire
    - How long it takes to triage/remediate them
      - Count over time for trending
  - ![screenshot](https://github.com/nterl0k/splunk_bonus_content/blob/main/dashboards/notable_and_analyst_review/notable_details_1.png)

