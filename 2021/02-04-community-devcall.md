---
tags: InterMine, community-call
---

# InterMine community call 2021-02-04

**Time/date:** 17.00 GMT 2021-02-04 (February 4th, 2021)
**Other timezones:** https://arewemeetingyet.com/London/2021-02-04/17:00


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
- Asher Pasha / BAR Araport ThaleMine / t: @AsherPasha
- Paulo Nuin / Wormbase
- Andrew Farmer / NCGR / LegumeInfo
- Lilly Winfree / Open Knowledge Foundation + Frictionless Data / @lilscientista (twitter)
- Kevin Herald / InterMine 
- Sam Hokin / NCGR / LegumeInfo 
- Joe Carlson / Phytozome/JGI
- Kalpana Karra / SGD
- Nikhil Vats / Frictionless Toolfund Grantee

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
 - Frictionless Data
     - Introduction [Lilly Winfree, PhD - Product Owner, Frictionless Data for Reproducible Research] ([slides](https://docs.google.com/presentation/d/e/2PACX-1vQMv0WFjYzwRKMi1v9pw2KG5pzHf9bmViRIC4GRYyPYwQlOfi2ewXg6YCFXeleo_OHIDDdhYVrl9qZH/pub?start=false&loop=false&delayms=3000)) email: lilly.winfree@okfn.org
     - Frictionless Specifications for InterMine [Nikhil Vats] ([slides](https://docs.google.com/presentation/d/1kOb1WpZS6aIiCTHGfemmKkxJ8NHpnTojEj4nP_dY3K4/edit?usp=sharing)) email: nikvats5499@gmail.com
     - Questions
         - Frictionless is involve machines and human, when describing data maybe better use the ontology term but also a more specific human readable descrption is fine
         - Frictionless python code (describe data, validate data, transform data): https://github.com/frictionlessdata/frictionless-py
         - browser tools:
             - create datapackages: https://create.frictionlessdata.io/
             - validata data: http://try.goodtables.io/
 - InterMine SPARQL endpoint [Daniela]
     - R2RML mapping and Ontop ([slides](https://docs.google.com/presentation/d/1DnQ9PsEQSfsHTB6TvGgHm-USKQO7U2C0M1hao_VdMNk/edit?usp=sharing))
     - SPARQL endpoint Demo
     - Questions
         - The code will be integrated as a new postprocess
         - The mapping should work for SimpleObject too, but it needs to be tested
         - federation queries with data providers using SPARQL endpoint (uniprot, disgenet)
         - this approach might bring new ideas, open new directions 
 - Outreachy December round [Rachel]
     - new user interface documention
     - update of existing intermine + bluegenes DEV documentation
 - GSoC - Deadlines: 29 Jan-19 Feb: Open source organizations applications
    - Interaction Tests for BlueGenes
    - Js library to allow clients to query InterMine
 - BlueGenes quick update [Kevin]
    - Quick overview of notable additions since last call
    - Introduction to configuring Bluegenes for your organisation's mines
    - [Flowchart for below](https://whimsical.com/bluegenes-deployment-QAYmWubSjSB1MH2gbHvSif)
    - Approaches to deployment of Bluegenes
	    - An instance for each organisation's mine
	    - One instance for all organisation's mines
    - How to allow an external Bluegenes to use visualization tools of a registry mine?
	    - Aim to deploy Bluegenes on the same domain as the mine(s)
		    - ex: `humanmine.org/humanmine/service` will point to the Intermine server, and any other path to Bluegenes
		    - An external Bluegenes will request `humanmine.org/api` (Bluegenes' backend) for its visualization tools
	    - Specify the URL of each mine's Bluegenes instance in the InterMine Registry
    - **Input from community is encouraged!**
 

### Next calls
- Next date: **May 6 2021**.
