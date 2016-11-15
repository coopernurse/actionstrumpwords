
## Purpose

The goal of this project is to document the actions of Donald Trump.

This is important because Trump likes to talk and often says inflamatory and
contradictory things that absorb considerable press and social media attention that
detract from the concrete actions he takes.

We must focus on his actions - factually verifiable things that occurred.

* Adrian Chen - "He gets power from that misunderstanding--the more people fight over what he says, the less people fight about what he does." - https://twitter.com/AdrianChen/status/798224141153247232
* Thomas Ptacek - "Bannon’s job isn’t policy. It’s making sure you don’t think about policy." - https://twitter.com/tqbf/status/797935780870193153

## How you can help

### Add / curate / correct the data

When Trump takes action, add it to the data:

* Fork the repo
* Edit `data/actions.json`
* Submit a PR

### Do stuff with the data

* Make a web site that uses the data to generate something browsable
* Share the data with your friends / family / colleagues
* Write articles that use this data as a reference or starting point
* ??

## Content notes

Stuff to include:

* Appointments
* Bills proposed / signed / vetoed
* Agreements / treaties signed

Maybe (let's discuss):

* Actions by cabinet. Not sure where to draw the line here.

Please don't add:

* Rumors
* Trump statements / quotes / tweets
* Congressional action

## Notes on the data structure

`actions.json` is a JSON list of objects. Object fields:

* `date` - date the action occurred (yyyy-mm-dd)
* `action` - brief description of what he did
* `urls` - list of strings. neutral, reputable news sources preferred.
* `tags` - list of strings. this will need the most evolution/curation. my initial thoughts are:
  * lower case
  * no spaces (use hyphens instead)

If you have suggestions for additional fields, open an issue and let's discuss it.

## FAQ

* Will `actions.json` scale?

Probably not.  But let's see if we get much traction.  Open an issue if you have a better
idea of how to store this data, but a JSON file can be easily managed via PRs in the near term.

* How should the file be formatted?

I'm using `jq` to format the file.  Ideally we'd automate this.

