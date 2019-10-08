---
tags: InterMine, community-call
---

[Original HackMD URL](https://hackmd.io/hWib_uyURhmXutt1D_JoQQ?view)

# 2019-10-03 InterMine community call 

**Time/date:** 3 October, 2019
**Other timezones:** https://arewemeetingyet.com/London/2019-10-03/17:00

## Joining the call: 
Zoom Meeting: https://zoom.us/j/328144808
- Meeting ID: 328 144 808
- Find your local number: https://zoom.us/u/abbfWdnE78

Once you've joined the call:
- Add your name to the attendee list below 
- Don't forget to turn on your webcam! :) 
    

### Attendees: 
Name / Organisation / InterMine / social handles if desired / [Emoji mood](https://emojipedia.org/)
- Yo Yehudi / InterMine / FlyMine and HumanMine /  G: @yochannah, t: @yoyehudi / 🍁🍂
- Andrew Farmer/NCGR/LegumeMine(s)//:/
- Kevin Herald Reierskog / InterMine / §=
- Daniela Butano /InterMine / 🌞
- Asher Pasha / BAR - Araport - University of Toronto / ThaleMine / G: @asherpasha, t: @AsherPasha / :coffee: :fire: :rice_scene:
- Paulo Nuin / WormBase / WormMine :-1: :camera:
- Joe Carlson
- Sam Hokin
- Kalpana Karra
- Howie Motenko
-  

### Icebreaker question: 
_Please fill this in while we're waiting for everyone to arrive!_
What's the last film you saw in the cinema - did you like it?
- [name=Yo] The new Lion King 🦁 - I loved it, but I love Lion King in all its forms, whether play, cartoon, or "live action". 
- [name=Andrew] [ possibly "Jeannette" a rock opera based on the early childhood of Jeanne d'Arc; HATED IT!]
- [name=Kevin] [ I prefer watching movies at home, so I really can't remember what I last saw in a cinema. ]
- [name=Daniela] [ Pain and Glory. I like Almovodovar...but always the same 2 themes!!]
- [name=Joe] Downton. I must admit
- [name=Sam] May have been a film at the Maine Film Fest, Cassandro, the Exotico! which I really enjoyed. It's about a Lucha Libre Exotico (gay) performer from El Paso.
- +


## Agenda

### Introduction 
(Yo)
 - Reminder: Code of Conduct! [View code of conduct](http://intermine.org/code-of-conduct/)
      - Generally: please treat others with respect and kindness, no matter who they are. We know you do this already! 
      - If you have any issues, please speak to:
        - Yo Yehudi yo@intermine.org or
        - Daniela Butano daniela@intermine.org

### Updates
(Yo)
- **Call agenda format:** You've probably noticed we're now using hackmd. This will allow us to easily export meeting notes to a GitHub repo, making it easier to search and view them in the future.
- **Call time & date:** We'd like to double-check if this is still the best time for our community. If you would like to attend InterMine community calls regularly, please fill out your availability here: http://whenisgood.net/intermine-community-calls  
- **Staffing:** Julie has now left us :cry: we wish her the best of success at Genomics England! Here's what to do if you'll need support for InterMiney things: 
    - Email: support@intermine.org
    - Pop by our discord chat: [chat.intermine.org](http://chat.intermine.org)
    - For very short things - [twitter.com/intermineorg](http://www.twitter.com/intermineorg) 
    - Open an issue on the relevant [GitHub](http://www.github.com/intermine) repository

#### InterMine 4.1.0 release
(Daniela)
- [Release blog](https://intermineorg.wordpress.com/2019/09/24/intermine-4-1-0/) and [release notes](https://github.com/intermine/intermine/releases/tag/intermine-4.1.0). 
- General points:
    - Better [Galaxy integration](https://intermine.readthedocs.io/en/latest/webapp/third-party-tools/galaxy/): you'll be able to import/export data to any InterMine from Galaxy EU and Galaxy USA without having to create a mine-specific Galaxy tool. 
    - Integrates neatly with [Elixir AAI](https://elixir-europe.org/services/compute/aai): an Elixir single sign in server
    - Java 11 Support
    - Various bugfixes
    - Update from Joe for incremental edits, since phytomine is large & can take a while. 
        - Sam uses this in all his builds! 
-  Questions / comments? 
    -  Is there guidance for upgrading? 
        -  Yes - youdon't need to rebuild database, just increment the gradle version number
            -  There have been errors trying this - is all okay? 
            -  InterMine will test with FlyMine and report back. 
    -  Q: Have we thought of integrating with Kbase? 
        -  We're not sure what Kbase is, so not yet
            -  https://kbase.us/ 
            -  Could be very useful for Sam as he may need to use it. 
    -  Will ELIXIR replace other logons? 
        -  No, it's in addition to Google, MyMine, etc. 
    - Asher has recently upgraded to 4.1.0, and will try Java 11. 
    - Joe will be submitting bug reports - Solr indexing error, solr dies but gradle says it worked. Possibly related to indexing on a huge field. 


#### BlueGenes 
(Kevin)

- Recent updates: *(well since I started in June)*
    -  Deep linking (lists, reports, even mine!)
        -  Reworked routing and URL paths
    -  Datavis tools added for GSoC
        -  Visual tool management WIP
    -  Stability improvements
        -  Lots of changes to initialisation code
    -  Pulls all InterMines from registry
        -  Switch between mines whether you're logged in or not
    -  Automatic handling of expired token alert
    -  Improved search page
        -  Fix various bugs (like filter not applying)
        -  Support multiple filters
-  Upcoming plans (required before release)
    -  Login/Auth improvements (requires some updates from InterMine)
        -  Superuser support (admin panel)
    -  Improve MyMine (requires some updates from InterMine)
        -  Personal templates
        -  List folders
        -  Preferences and password
    -  New report page design
    -  Dynamic page titles (I at least want this)
        -  +1 Yo agrees :) 
-  Q: How do I run my own BlueGenes? 
    - A: you'll need to have your InterMine working with a recent gradle version.  [Deployment instructions](https://intermine.readthedocs.io/en/latest/system-requirements/software/gradle/?highlight=bluegenes#deploy-blue-genes).
- Status update blog (June) https://intermineorg.wordpress.com/2019/06/05/status-update-for-bluegenes/
-  Questions / comments? 
    -  [name=Paulo] Will the SuperUser be actually a superuser, "owning" all the public templates for instance?
        -  [name=Yo] (summarising discussion) superusers can't see any templates belonging to other superusers -it would be handy to have a higher level superuser to make multi-admin settings easier. Specifically, sharing public templates is a problem here. 
    - [name=Kalpana]  Is MyMine i.e userprofile shared between the mine and bluegenes?
        -  [name=Yo] Yep, Bluegenes won't have its own backend - the backend will be InterMine. 
    -  [name= Kalpana] Is there a task to 'stop' bluegenes? Each time mine is built, should bluegenes 'start' run?
        -  [name=Daniela] I don't think there is a task to do this - we can look into it though. 
        -  The auto restart won't be required in newer BlueGenes versions, so rebuilding mines should be fine and won't break bluegenes. 
    -  [name=adf] Can I see the data visualisations? 
        - See https://medium.com/intermine/google-summer-of-code-2019-with-intermine-43e4b8c4f9ba 
        - [flymine](http://bluegenes.apps.intermine.org/default/report/Gene/1007235)
        - [humanmine](http://bluegenes.apps.intermine.org/humanmine/report/Gene/1257384)

#### Hacktoberfest!
(Yo)
[Hacktoberfest](https://hacktoberfest.digitalocean.com/) is coming up soon (during the full month of October)! During Hacktoberfest, people submit pull requests to open source repositories on GitHub - if they make four PRs, they get a free tshirt.
- Feel free to make PRs to InterMine repos in October :wink: 
- Mark up your own issues with Hacktoberfest if you'd like contributors! 

##### What makes a good hacktoberfest issue?
- it needs to be clearly defined and easy to pick up
- someone needs to monitor it and respond to queries / PRs.
- could be as simple as requesting colour changes and typo fixes, or "make a logo for this" - these sometimes take longer to writeup than to fix yourself, but can be worth it if it leads to further engagement.
- Possible good targets for labels like this include repos where we have small bugs or feature wishes but haven't gotten around to fixing things. Repos that require a lot of setup are less optimal. 

### Upcoming events

- November 2019: [Paris Biohackathon](https://www.biohackathon-europe.org/)
    - Attending: Sergio, Kevin, Yo, Daniela
    - Possible topics include: 
        - Registering all InterMines from the registry to bio.tools - make sure [your registry entry](http://registry.intermine.org) is up-to-date! 
        - Further Galaxy integrations
        - FAIR in practice for InterMine: identifying challenges. 

### Next calls

[View in calendar](https://intermineorg.wordpress.com/events/)

- 7 November 2019 - Normal dev call
- 5 December 2019 - Community outreach call 
