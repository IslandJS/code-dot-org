<% facebook = {:u=>"http://#{request.host}/us"}
                      twitter = {:url=>"http://hourofcode.com", :related=>"codeorg", :hashtags=>"", :text=>hoc_s(:twitter_default_text)}
                      twitter[:hashtags] = "HourOfCode" unless hoc_s(:twitter_default_text).include? "#HourOfCode" %># Ευχαριστούμε που γράφτηκες για να πραγματοποιήσεις μια Ώρα του Κώδικα!

**EVERY** Hour of Code organizer will receive 10 GB of Dropbox space or $10 of Skype credit as a thank you. [Details](<%= hoc_uri('/prizes') %>)

<% if @country == 'us' %>

Get your [whole school to participate](<%= hoc_uri('/prizes') %>) for a chance for big prizes for your entire school.

<% end %>

## 1. Διάδωσέ το

Πες στους φίλους σου για την Ώρα του Κώδικα (#HourOfCode).

<%= view :share_buttons, facebook:facebook, twitter:twitter %>

<% if @country == 'us' %>

## 2. Ask your whole school to offer an Hour of Code

[Send this email](<%= hoc_uri('/resources#email') %>) or [this handout](http://hourofcode.com/files/schools-handout.pdf). Once your school is on board, [enter to win $10,000 worth of technology for your school](/prizes) and challenge other schools in your area to get on board.

<% else %>

## 2. Ask your whole school to offer an Hour of Code

[Send this email](<%= hoc_uri('/resources#email') %>) or give [this handout](http://hourofcode.com/files/schools-handout.pdf) to your principal.

<% end %>

## 3.Κάντε μια γενναιόδωρη δωρεά 

[Donate to our crowdfunding campaign.](http://<%= codeorg_url() %>/donate) To teach 100 million children, we need your support. We just launched what could be the [largest education crowdfunding campaign](http://<%= codeorg_url() %>/donate) in history. Every dollar will be matched by major Code.org [donors](http://<%= codeorg_url() %>/about/donors), doubling your impact.

## Ζήτα από τον εργοδότη σου να εμπλακεί 

[Send this email](<%= hoc_uri('/resources#email') %>) to your manager, or the CEO. Or [give them this handout](http://hourofcode.com/resources/hoc-one-pager.pdf).

## Προωθήστε την ώρα του κώδικα μέσα στην κοινωνία σας

Φτιάξε ένα τμήμα για — ένα σώμα προσκόπων, μια ενορία, ένα πανεπιστήμιο, μια ενώση εργαζομένων. Ή κάνε μια Ώρα του Κώδικα για το τετράγωνο της γειτονιάς σου.

## 5. Ζήτα από ένα τοπικό άρχοντα να υποστηρίξει την Ώρα του Κώδικα

[Send this email](<%= hoc_uri('/resources#politicians') %>) to your mayor, city council, or school board. Or [give them this handout](http://hourofcode.com/resources/hoc-one-pager.pdf) and invite them to visit your school.

<%= view 'popup_window.js' %>