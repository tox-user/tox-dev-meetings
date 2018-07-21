tox-user: hi everyone
Ingvar: hello
Ingvar: topics for this meeting: https://github.com/tox-user/tox-dev-meetings/blob/master/2018-07-21/README.md
tox-user: is hugbubby here for the meeting?
tox-user: !users
toxync: [toxync12@irc] There are 82 users, [toxync12@irc] +tux3, @CeBe, @ChanServ, @Emcy, @Impyy, @Jfreegman, @SmokedCheese, @clever, @e0f, @iphy, @irungentoo, @nicoo, @nurupo, @robinli, @sudden6, @wiiaam, @zugz, BottomFeeder, CcxWrk, DeX77, Encrypt, GDR[m], Hunger-, Just[m], LittleVulpix, MissingTwins[m], Myrl-saki, Piraty, PyroLagus, SkyzohKey[m], Sorunome, Toxit, Yaniel, _redmanmale, ahve, albel727, anonus, anthonybilinski, arza, chainsawbike, chron0, cisc, coy[m], dan-, dfceaef[m], dontstalkmepls[m, drEquivalent, drEquivalent1, dxld, eater, esainane, f8l, foxkjrdyezstogcr, gzs[m], gzs[m]1, halbeno, hxgkcgytxmgmxg[m, kevun, kivutar, koshii, kurnevsky, lnostdal, mario, matt-h, mitfree[m], neunon, orzo, psyk, quantized[m], ranter-, return0e, riot13ar[m], sonOfRa, strfry, szh7379[m], tobiasBora, toxirc, toxync12, ullbeking, xYuusha, xek, zero-one currently on IRC
tox-user: first topic: PGC development state
tox-user: what is the current state?
tox-user: any changes lately?
Ingvar: iphy zugz ^
tox-user: seems nothing has changed https://github.com/TokTok/c-toxcore/milestone/31
toxync: [BottomFeeder@irc] only im here
toxync: [BottomFeeder@irc] and i know nothng about nothing
toxync: [BottomFeeder@irc] but hugbubby is a good name
tox-user: :)
Ingvar: looks like ngc will be done faster than pgc :D
tox-user: true
tox-user: the only thing left in ngc is improving ban feature??
Ingvar: ban, group audio and typing notifications
Ingvar: bug fixing and minor refactoring
toxync: [zugz@irc] I'm just writing a proposal for a minimal version of pgc, without the api changes and hacks
tox-user: group audio wasn't supposed to be a part of it and group typing notifications sound like a small optional feature
Ingvar: yeah, typing notifications can be easily added later
tox-user: zugz: cool, you think that might get it done faster?
tox-user: so bans are the only important thing that is left?
toxync: [zugz@irc] yes
toxync: [zugz@irc] the downside is that it won't work if your friends are using current toxcore
Ingvar: tox-user: bans and group audio, but audio will be done later. so yes, only bans
toxync: [zugz@irc] and there's no saving, it's just for recovering from network disconnections
tox-user: still better than normal but worse than current pgc
tox-user: Ingvar: are bans easy to finish?
toxync: [zugz@irc] in terms of features, yes
Ingvar: yes
tox-user: so ngc only have one small feature left to make while pgc still has breaking bugs
Ingvar: 1 small feature and few bugs probably
tox-user: I see
tox-user: it's getting closer and closer
tox-user: let's move on to our second topic
tox-user: Branches in Toktok repository [Ingvar]
Ingvar: I have pretty simple suggestion 
Ingvar: right now users can't donwload last stable release easily
tox-user: release of what?
Ingvar: toxcore
Ingvar: because there is only master branch in repo
Ingvar: and sometimes it contains commits like version x.y.z while last version is still x.y.(z-1)
Ingvar: so confusing
tox-user: you can do git clone https://github.com/TokTok/c-toxcore; then git checkout v0.2.4
Ingvar: I need to know latest version number in this caase
Ingvar: case*
tox-user: true
tox-user: you can also get it from https://github.com/TokTok/c-toxcore/releases
Ingvar: I suggest to create develop branch and update master after release only
Ingvar: yes, I can, but this is bad idea when you need a script for latest toxcore downloading
Ingvar: like script I have on travis
tox-user: we do that in qTox
tox-user: we update the version with every qTox release which is every few months
Ingvar: cool
Ingvar: time for next topic?
tox-user: we could create a develop branch
tox-user: or a stable branch
Ingvar: next topic:
Advertising for new developers [hugbubby]
toxync: [foxkjrdyezstogcr@irc] zugz: why no saving?
toxync: [foxkjrdyezstogcr@irc] not possible, or u don't like it?
toxync: [zugz@irc] foxkjrdyezstogcr: actually I think it could be added easily
toxync: [zugz@irc] I'll check - anyway, ignore me on this until I actually put up a proposal, still need to think through some details
toxync: [zugz@irc] foxkjrdyezstogcr: actually no, there's a reason for avoiding saving, but let's discuss after the meeting
tox-user: hugbubby isn't here so we should skip it
tox-user: Ingvar: in that case the meeting is over?
tox-user: unless you know what he meant
tox-user: and what to discuss it
Ingvar: no
Ingvar: so looks like meeting is over
tox-user: ok
Ingvar: our shortest meeting ever
tox-user: poor attendance
Ingvar: all devs are dead
Ingvar: so it's ok
tox-user: looks like it
tox-user: at least zugz came :)
Ingvar: but other devs are inactive :(
