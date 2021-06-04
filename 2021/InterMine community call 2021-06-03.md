---
tags: InterMine, community-call
---

# InterMine community call 2021-06-03

**Time/date:** 17.00 BST 2021-06-03 (June the 3th, 2021)
**Other timezones:** https://arewemeetingyet.com/London/2021-06-03/17:00/InterMine%20Community%20Call


## Joining the call: 
Join Zoom Meeting
https://us02web.zoom.us/j/88094897403?pwd=UE00Q2FEOGNiUzRUd0k0NHFFdUYzZz09

- Meeting ID: 880 9489 7403
- Passcode: 539009 

Once you've joined the call:
- Add your name to the attendee list below 
- Don't forget to turn on your webcam! :) 

Attendees: Name / InterMine / Project / social handles if desired
- Daniela Butano / Cambridge team
- Kevin Herald / InterMine 
- Sergio Contrino / InterMine
- Asher Pasha / ThaleMine, University of Toronto
- Paulo Nuin / WormBase/Alliance of Genome Resources
- Andrew Farmer / LegumeMine(s)/NCGR
- Eric Marcus
- Kalpana Karra
- Sam Hokin
- Ankur Kumar
- Ankit Kumar

## Agenda

### Introduction 
[Daniela]
 - 🎥 This call is being recorded - please turn your camera off if you'd rather your face doesn't end up on youtube :)
 - Reminder: Code of Conduct! [View code of conduct](http://intermine.org/code-of-conduct/)
      - Generally: please treat others with respect and kindness, no matter who they are. We know you do this already! 
      - If you have any issues, please speak to:
        - Rachel Lyne rachel@intermine.org or
        - Daniela Butano daniela@intermine.org

### Items
#### InterMine 5.0.2 release [Daniela]
- 5.0.1 broken (due to [Nexux Repository Manager](https://s01.oss.sonatype.org) sync issue)
- [XSS vulnerability](https://github.com/intermine/intermine/issues/2358)
- list/chart and /list/enrichment WSs fixed when using IDs
- [GFF3Converter](https://github.com/intermine/intermine/issues/2344) (thanks Sam Hokin)
- [BioGrid loader](https://github.com/intermine/intermine/issues/2335)
- Questions?

#### BlueGenes 1.1.0 release [Kevin]
- Adding back chart and table widgets
    - In contrast to legacy webapp, will show for all query results containing a supported class (e.g. genes)
- What new features would you like to see the most?
    - More customisability without having to edit source files [#718](https://github.com/intermine/bluegenes/issues/718) +
        - could include reordering/removing existing pages and adding new ones
        - a guide which describes what we can add where (instead of an editor, we could write documentation to make it easier to edit source files)
    - Integrating BLAST service [#576](https://github.com/intermine/bluegenes/issues/576), Integration with a sequence server ++
        - seems to be widely used and integration/linkouts could be useful
    - Missing admin features (create/edit templates, set a user as admin)
        - and try to fix the issue related to multiple admins wich own different templates, they will no be public
    - List sharing (how many people use this?) [#652](https://github.com/intermine/bluegenes/issues/652)
        - some in wormmine could be using this - would be useful to add back
    - Improving im-tables used in BlueGenes
    - Improve experience when switching between mines (keep query/activity history for each mine, instead of clearing)
    - More features for list analysis [#572](https://github.com/intermine/bluegenes/issues/572) +


### Upcoming events
#### Upgrade-thon
Thu, 7th of October 16.00-20.00 GMT
- Agenda
    - migrate the mine webapp and custom data sources to maven directory structure,
    - overview of the basic gradle tasks,
    - overview of the new user interface and installation (bluegenes),
    - discuss about new functionalities in bluegenes

### Next calls
- Not scheduled yet