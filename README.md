**Run create_ordered_leader_schedule.js to get a leader schedule with the identity address of validator next to "leader:"**

i.e.
  "leader": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
  "leader": "identity address of validator/leader"

This is useless as we need VoteKey address of validator. 

We can fetch the location and validator information by extracting the VoteKey addresses of all validators. We fetch all VoteKey addresses of each validator first, then use this to fetch the information of each validator. 
**Then hopefully the information of each validator can be linked back to the identity address of each validator.**


**New things to add once we link things up (VoteKey, Location and Coordinates are all in):**
[
  {
    "slot": 0,
    "absoluteSlot": 264816000,
    "leader": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
    "VoteKey": "dwadawdwa"
    "Location": "dwadwadwa"
    "Coordinates": "dwadawdwa"
  },
  {
    "slot": 1,
    "absoluteSlot": 264816001,
    "leader": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
  },
  {
    "slot": 2,
    "absoluteSlot": 264816002,
    "leader": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
  },
