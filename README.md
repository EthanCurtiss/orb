# Orb system

Orbs are listening devices, often located near metaboards, that people can attach themselves to as listeners so that they continue to hear a talk while elsewhere in the world. They also serve as recording devices for audio and video.

You can access the public [test server](https://www.roblox.com/games/8369549984/Orb-test) and watch some videos:

- [Initial implementation](https://youtu.be/0vuNKcCv1sk).

## Usage

Here's a scenario: two masters students graduated from the same University, have similar interests, but haven't seen each other in a while and have moved to different continents since then. They show up for a metauni day session (maybe Foundations) and while wandering around to sit on a floating ring while listening through an orb, they notice each other and disconnect from listening in order to chat about what they're working on now. An hour later they're still talking math, not even noticing that the event ended.

In this scenario the ability to wander off in listener mode **lowers the activation energy for informal social interaction around mathematics**. I think people are much less likely to break out their personal boards and start chatting in the middle of the talk venue, because it feels kinda rude and they might be in the way. But off in some cave or corner of the world it feels OK.

Lowering this activation energy seems important, and is the main purpose of the Orbs.

## Implementation

Just as metaboards are parts in the world tagged with `metaboard`, an orb is a part tagged `metaorb`.

TODO:

- Detach as listener either with proximity prompt or GUI
- Create ghost near orb on attach
- Destroy ghost on detach
- Attach as speaker to orb (no permissions) (proximity)
- Speaker can see the ghost orb
- Detach as speaker to orb (in GUI)
- When attached as speaker, orb follows you (straight track)
- Check that listeners hear from new orb position?
- Listener ghosts follow moving orb
- Orb follows you (spline track)
- Orb looks at nearest board
- Listeners have viewport view of board
- Warn to detach as speaker if you walk too far away (in GUI)
