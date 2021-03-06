<% facebook = {:u=>"http://#{request.host}/us"}
                      twitter = {:url=>"http://hourofcode.com", :related=>"codeorg", :hashtags=>"", :text=>hoc_s(:twitter_default_text)}
                      twitter[:hashtags] = "HourOfCode" unless hoc_s(:twitter_default_text).include? "#HourOfCode" %>



# Bedankt dat je je hebt opgegeven om een Uur Code te organiseren!

**EVERY** Hour of Code organizer will receive 10 GB of Dropbox space or $10 of Skype credit as a thank you. [Details](<%= hoc_uri('/prizes') %>)

<% if @country == 'us' %>

Get your [whole school to participate](<%= hoc_uri('/prizes') %>) for a chance for big prizes for your entire school.

<% end %>

## 1. Zegt het voort

Vertel je vrienden over het Uur Code, #HourOfCode.

<%= view :share_buttons, facebook:facebook, twitter:twitter %>

<% if @country == 'us' %>

## 2. Vraag je hele school een Uur Code aan te bieden

[Send this email](<%= hoc_uri('/resources#email') %>) or [this handout](http://hourofcode.com/files/schools-handout.pdf). Is je school aan boord, [ding dan mee naar $10.000 aan technologie voor je school](/prizes) en daag andere scholen in je district uit ook mee te doen.

<% else %>

## 2. Vraag je hele school een Uur Code aan te bieden

[Send this email](<%= hoc_uri('/resources#email') %>) or give [this handout](http://hourofcode.com/files/schools-handout.pdf) to your principal.

<% end %>

## 3. Maak een donatie

[Donate to our crowdfunding campaign.](http://<%= codeorg_url() %>/donate) To teach 100 million children, we need your support. We just launched what could be the [largest education crowdfunding campaign](http://<%= codeorg_url() %>/donate) in history. Every dollar will be matched by major Code.org [donors](http://<%= codeorg_url() %>/about/donors), doubling your impact.

## 4. Vraag uw werkgever om betrokken te raken

[Send this email](<%= hoc_uri('/resources#email') %>) to your manager, or the CEO. Or [give them this handout](http://hourofcode.com/resources/hoc-one-pager.pdf).

## 5. Promoot het Uur Code in je gemeenschap

Werk samen met een vereniging — scouting, kerk, universiteit of vakbond. Of organiseer een Uur Code "buurtfeest" voor je wijk.

## 6. Vraag een politicus het Uur Code te ondersteunen

[Send this email](<%= hoc_uri('/resources#politicians') %>) to your mayor, city council, or school board. Or [give them this handout](http://hourofcode.com/resources/hoc-one-pager.pdf) and invite them to visit your school.

<%= view 'popup_window.js' %>