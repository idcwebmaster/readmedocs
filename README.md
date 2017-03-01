NFL Combine Site
=================

NFL SCOUTING COMBINE
The NFL Scouting Combine is a vital event in the path to the draft. More than 300 prospects will participate in the Combine in their quest to achieve their NFL dreams. 

# Resources and Links

- http://www.nfl.com/combine 
- http://www.nfl.com/combine/live
- http://www.nfl.com/combine/participants
- http://www.nfl.com/combine/tracker
- http://www.nfl.com/combine/top-performers
- http://www.nfl.com/combine/workouts
- http://www.nfl.com/photos?eventseason=-1&event=combine
- http://www.nfl.com/videos/nfl-combine
- Documentation for [Combine Console](http://confluence.la3.nfl.com/confluence/display/COMSOFTDEV/Combine+and+Draft+Console+Tech+Guide) 
- Documentation for [Combine Live](https://confluence.dm.nfl.com/pages/viewpage.action?pageId=25658886)

### Combine Landing Page
	- Desktop: /content/public/static/html/combine/combine-desktop.html
	- Mobile: /content/public/static/html/combine/combine-mobile.html
	- Ranking: http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp
		- [2 Col Centerpiece]( http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_2col_cp_combine)
		- [Centerpiece] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_cp_combine)
		- [Conteent Stream] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_content_stream_combine)
		- [Headlines] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_headlines_combine)
		- [Headlines Top Piece] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_headlines_toppiece_combine)
		- [Hot Topic] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_hot_topic_combine)
		- [NFL Now] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_nfl_network_combine)
		- [Photo Gallery] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_combine_photo_galleries)
		- [Spotlight] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_spotlight_combine)
		- [Video Row] (http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_videorow_1_combine)
		- [Voices] http://prodpolls-vip.la3.nfl.com/cmsconsole/ranktool/load.do/Events/combine_lp/widget_voices_combine)
	- Combine Live Traffice Driver: widget/home-2011/views/live-traffic-driver

### Combine Live

#Code - All in Alfresco
Live landing page: 
	- /content/public/static/html/combine/live.html

Config Change State - /widgets/config-files/combine/live.html 
	- PLAYER_ENABLED - Switch Pre and Active states
	- COMBINE_LANDING_TRAFFIC_DRIVER - controls Combine landing page Live traffic driver

Widgets:
	- Pre State: /content/public/static/html/widgets/combine/live/pre-state-content 
	- Active State: /content/public/static/html/widgets/combine/live/static-triple-wide
	- Active State Spotlight: /content/public/static/html/widgets/widgets/combine/live/player-spotlight
	
#Data:
live player schedule	
	- /content/public/static/config/combine/2016/live/combine_schedule.xml
participants data	
	- /content/public/static/config/combine/2017/live/combine_live_data_day1.xml
	- /content/public/static/config/combine/2017/live/combine_live_data_day2.xml
	- /content/public/static/config/combine/2017/live/combine_live_data_day3.xml
	- /content/public/static/config/combine/2017/live/combine_live_data_day4.xml
video meta data	
	- /content/public/static/config/combine/2017/live/video-json-day1.json
	- /content/public/static/config/combine/2017/live/video-json-day2.json
	- /content/public/static/config/combine/2017/live/video-json-day3.json
	- /content/public/static/config/combine/2017/live/video-json-day4.json
player spotlight	
	- /content/public/static/config/combine/2017/live/spotlight/player-spotlight_d1.json
	- /content/public/static/config/combine/2017/live/spotlight/player-spotlight_d2.json
	- /content/public/static/config/combine/2017/live/spotlight/player-spotlight_d3.json
	- /content/public/static/config/combine/2017/live/spotlight/player-spotlight_d4.json

#Console Info
Fantasy Live Console: 
	- http://prodpolls-vip.la3.nfl.com/fantasy-live/login

Documentation: 
	- https://github.dm.nfl.com/NFL/fantasy-live-console/blob/master/README.md
							
Console (STAGE):
	- http://stagepolls-vip.la3.nfl.com/fantasy-live?sandcastle=true						

Console (PROD):
	- http://prodpolls-vip.la3.nfl.com/fantasy-live?sandcastle=true						

Video playback:
	- http://stage.www.nfl.com/static/content/static/config/fantasy/2016/live/week25/video-json-w25d4.json						

Video playback alfresco	
	- http://alfresco.la3.nfl.com/share/page/site/nfl-com/documentlibrary#filter=path%7C%2Fstatic%2Fconfig%2Ffantasy%2F2016%2Flive%2Fweek26%7C&page=1	Update this with "base url for video playback" + the {day}					

Base URL for video playback:
	- http://nflioslivesvg6-i.akamaihd.net/hls/live/268409/combine/2017Combine_w00{d9}.m3u8						

Current week 	
	- http://vmstagepolls01.la3.nfl.com:8080/console-api/fantasy/currentWeek									
							
#Segment JSON						
live:	
	- http://www.nfl.com/liveupdate/fantasy/live/episode.json						
archive:
	- http://www.nfl.com/fantasyfootball/live/episode?season=2016&seasonType=POST&week=26&day=FRI						
	- http://www.nfl.com/fantasyfootball/live/episode?season=2016&seasonType=POST&week=26&day=SAT						
	- http://www.nfl.com/fantasyfootball/live/episode?season=2016&seasonType=POST&week=26&day=SUN						
	- http://www.nfl.com/fantasyfootball/live/episode?season=2016&seasonType=POST&week=26&day=MON	

### Participants

#Code
	- Desktop: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/participants-desktop.jsp
	- Mobile: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/participants-mobile.jsp
	- Documentation: https://confluence.dm.nfl.com/display/PROJECTS/Upload+Player+Profiles

#Data 
	JSON: http://www.nfl.com/widget/combine/person/json?id={playerId} 
		Ex: http://www.nfl.com/widget/combine/person/json?id=2557979
	Controller: com.nfl.site.web.controller.prospect.CombinePlayersController

### Top Performers

#Code
	- Desktop: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/top-performers-desktop.jsp
	- Mobile: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/top-performers-mobile.jsp

#Data 
	- JSON: /ajax/combine/top-performers-json?years={years}&positionGroups={position}&workout={workout}	
		Ex: http://www.nfl.com/ajax/combine/top-performers-json?years=2017&positionGroups=QB,RB,WR,TE,S,DL,LB,CB,OL,SPECIALISTS&workout=FORTY_YARD_DASH

### Tracker

#Code
	- Desktop: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/tracker-desktop.jsp
	- Mobile: https://github.dm.nfl.com/NFL/site/blob/master/NFL-site-web/src/main/webapp/WEB-INF/pages/combine/tracker-mobile.jsp

#Data 
	- JSON: /liveupdate/combine/{year}/{event}/ALL.json
		Ex: http://www.nfl.com/liveupdate/combine/2017/FORTY_YARD_DASH/ALL.json?957
	- Controller: com.nfl.site.web.controller.combine.CombineTrackerController 
