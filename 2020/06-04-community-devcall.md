---
tags: InterMine, community-call 2020-06-04
---

# InterMine community call 2020-06-04

**Time/date:** June 4 2020, 17:00 UK time
**Other timezones:** https://arewemeetingyet.com/London/2020-06-04/17:00/InterMine%20Community%20Call


## Joining the call: 

Join Zoom Meeting
https://us02web.zoom.us/j/89442209503?pwd=MlV2N1JPWVpEaUNlcThibHFBdGQvUT09



Once you've joined the call:
- Add your name to the attendee list below 
- Don't forget to turn on your webcam! :) 
    

### Attendees: Name / InterMine / Project / social handles if desired / [Emoji mood](https://emojipedia.org/)

- Yo Yehudi / InterMine Cambridge / t: yoyehudi & intermineorg / github @yochannah
- Daniela Butano / InterMine Cambridge
- Joe Carlson / JGI (for the first 30 minutes)
- John Mendez
- Sven
- Jacqueline Campbell / Legume Mines / t: Campbell_JD_PhD & LegumeFed 
- Kevin Herald / InterMine Cambridge 
- Andrew Farmer / NCGR (BeanyMines)
- Asher Pasha / ThaleMine / BAR Araport / t: @AsherPasha g: @asherpasha / :ocean: :relieved: :palm_tree: 
- Gos Micklem / InterMine Cambridge

Icebreaker question: What book, TV show, video game, or music are you excited about? (Maybe it's new-to-you if not new for others!) 
- [name=Yo] I've been reading books on [Serial Box](https://www.serialbox.com/) - the first chapter is always free, and you can seamlessly switch from narrated audiobook to onscreen ebook. Machina was awesome! 
- [name=John Mendez] I'm excited to binge watch *Space Force* on Netflix this weekend. I've loved Steve Carell's work since The Office (US).
- [name=Sven] - <i>The Long Ships</i> by Frans Bengtsson, swashbuckling Viking adventures
- [name=Kevin] - I have been listening to the WW2 podcast lately (lots of exciting episodes!)
- [name=Asher] - Video game <i>Bloodborne</i> - One of the most difficult games and the best I have played.
- [name=adf] [ The Possessed by Dostoevsky- much funnier than I remember from my teenage days]
- Gos - Marking exams!!! :-) :-)

## Agenda

### Introduction 
Yo
 - 🎥 This call is being recorded - please turn your camera off if you'd rather your face doesn't end up on youtube :)
 - Reminder: Code of Conduct! [View code of conduct](http://intermine.org/code-of-conduct/)
      - Generally: please treat others with respect and kindness, no matter who they are. We know you do this already! 
      - If you have any issues, please speak to:
        - Yo Yehudi yo@intermine.org or
        - Daniela Butano daniela@intermine.org


### Items
- [Upcoming release plans](https://intermine.readthedocs.io/en/latest/intermine/roadmap/)
    - [InterMine Roadmap](https://github.com/intermine/intermine/projects/7)
        - Github project board that shows all tickets planned for a given release. 
- **Federation and managing multiple mines** - what is there now and what do we want to see?
    - Single Sign-On - GSoC 2019.
        - One single InterMine sign on, or a "neighborhood" managed set of instances? e.g. one for plants, one for animals, one for insects, etc...?
        - https://github.com/intermine/intermine-authorization-server 
    - Cross-InterMine Search (needs some performance improvements)
    - One BlueGenes, many mines?
        - Right now BlueGenes supports mine-switching. Possible use-cases:
        - Allow a mine admin to select a single neighborhood from the registry
        - Allow a custom-curated set of URLs
        - Other? 
    - Genuine federation
        - Update client libraries to accept an array or URLS or namespaces from the registry?
        - handling disparate models? 
    - Discussion notes:
        - ADF (legume mines) have multiple mines that are more details as well as a single larger (but sparser data) integrated mine.
        - Vivek did work on keyword searches across many intermines.
            - results integrated via ranking from InterMines
            - Sven moved this work from Drupal to Django.
        - What about template queries across multiple intermines? 
            - Sometimes this works
            - how do you manage lists across multiple intermines? 
            - Can be unexpected results for cross-intermine template queries. 
            - Gos: Different models could use the same template redefined in each mine so the same template works regardless of what's under it. 
            - This approach could limit federation functionality. 
        - 200+ organisms in PhytoMine. Federated queries could maybe help resolve this "wall" of size for PhytoMine. 
            - This is a scenario where you could have a 100% harmonised model, so wouldn't even need a template. 
            - How would you handle cross-species data, e.g. homology? 
            - One mine for monster relationship mediation maybe? 
        - ADF: Friendlymine functionality to use gene family relationships instead. Possibly need Sam to engage in this convo :) 
        - What about people who only want a given subset of data, e.g. Brachypodia? 
            - e.g. select a subset of intermines to respond to a query. 
        - What about a partitioned mine? E.G. only rebuild the parts that always change - database managed splits (sharding)
            - Sergio used to do this in MODEncode.
        - What about Citus https://github.com/citusdata/citus ? Would allow PostgreSQL to be sharded. Joe experimented with this but didn't deploy as it was not compatible with the OS that he was running. 
        - Does postgres support partitioning on its own? May bear further investigation. 
        - What about user perspectives? Multiple intermines - as a user it is a pain to have to log in to multiple intermines with separate accounts.
            - Simplest solution https://www.lastpass.com/ but doesn't handle things like templates, lists across mines. 
        - Federation gets cooler the more you can do with the federated results
            - http://gointermod.apps.intermine.org/# was a nice demo but needs to be fixed. 
- **CovidMine**: 
    - [Announcement blog](https://intermineorg.wordpress.com/2020/05/14/announcing-covidmine-analyse-integrated-covid-genomic-and-geographical-distribution-data/)
    - [Try it out (BlueGenes)](http://covid.apps.intermine.org/)
    - We will ask Sakshi to look at a map for GIS vis. 
- **Interns**
    - Projects include:
        - Upgrading our R client
        - Updating the InterMine Data Browser ( was originally a GSoC 2018 project). 
        - InterMine CLI + Boot
        - InterMine Training portal (focus on python tutorials with videos of the tutorials)
        - Data vis (adding more data vis tools for BlueGenes)
        - UX research on BlueGenes
            - If you can spare 30-60 minutes (tops) for a UX interview please ping Yo (yo@intermine.org) or add your email address here. 
    - Outreachy - five interns. [Blog posts](https://intermineorg.wordpress.com/tag/outreachy/).
    - Two in-house interns, would have been here physically if we were in non-pandemic conditions... :mask: 
    - No GSoC this year :sob: 
    - GSoD - applications open via [INCF](https://www.incf.org/activities/google-season-of-docs). Technical writers rather than students or interns. 
    - Possible projects (depends on us getting a slot): 
        - Video tutorials for BlueGenes
        - Update existing docs 
            - note: tours can function as a form of test as they will break when UIs get updated. 
            - Intro.js may replace the tour in legumemine germplasm page 

### Upcoming events
- [BCC2020](https://bcc2020.github.io/) (BOSC + GCC)
    - InterMine API training (both sessions are the same): 
        - Session 1: [Friday 17 July](https://bcc2020.sched.com/event/bzhZ/handling-integrated-biological-data-using-python-jupyter-and-intermine). UK evening, USA morning or early afternoon
        - Session 2: [Sunday 19 July](https://bcc2020.sched.com/event/c8Kq/handling-integrated-biological-data-using-python-jupyter-and-intermine). Early morning UK and late afternoon/evening in Australia
    - We can offer full-conference tickets to potential trainers who want to help out
    - Hopefully we will have a talk focusing on building long-term contributors and community. 
    
### Next calls

- If you would like to recieve an email invitation please add your email below (or email yo@intermine.org to be added to the list)
- Date not yet confirmed - Outreachy interns final presentations
    - Might be earlier than our usual timeslots, as we have interns ranging from East Coast USA to Singapore (12 hour time span - 09:00 in New York is 21:00 in Singapore). 
- September 3 
- December 3
