This is a handy Bugzilla need info flag dashboard that supports displaying summary needinfo counts for
teams categorized by developer / release management setters. Need infos are broken down into four
columns - developer related needinfos on open and closed bugs, and release management related needinfos.
The main pane provides needinfo counts linked to both Bugzilla bug lists as well as a needinfo list
details sub page. The details page provides a list of each needinfo matched to the bugzilla comment
when the flag was set, as well as additional meta data such as bug title, severity, priority, and
assignee. A basic set of bulk action options are also provided for authenticated users.

Note authentication through a Bugzilla API key is required for visibility of security related bugs
and for access to bulk actions. API keys can be generated through Bugzilla account preferences.

See the dashboard settings for api key configuration and other display options.

Improvements and bug fixes for the dashboard are welcome!

If you would like to add an additional team to this dashboard submit a new team specific json config
file with an updated 'developers' entry and update the 'team-select' select in the index file. See
js/media.json for an example of the json format.

For testing changes there's a switch in each json config file that will point the dashboard at the test
instance of Bugzilla Mozilla maintains. For API key generation or new accounts generation on the test
instance ask in chat.mozilla.org's bugzilla.mozilla.org channel.

This dashbaord was originally based on Bob Hood's Need Info Leaderboard.