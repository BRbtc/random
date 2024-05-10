
1. Match Nodepubkey address from validators_data.json with "leader:" address from hashtestingE.json
2. Then add all information from validators_data.json for the match under leader:

i.e. 

[
  {
    "slot": 0,
    "absoluteSlot": 264816000,
    "leader / nodePubkey ": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
    "votePubkey": "6D2jqw9hyVCpppZexquxa74Fn33rJzzBx38T58VucHx9",
    "country": "JP",
    "timezone": "Asia/Tokyo",
    "ll": [35.695126,139.75391]
    "moniker": "Coinbase Cloud 02",
  },
  {
    "slot": 1,
    "absoluteSlot": 264816001,
    "leader / nodePubkey ": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
    "votePubkey": "6D2jqw9hyVCpppZexquxa74Fn33rJzzBx38T58VucHx9",
    "country": "JP",
    "timezone": "Asia/Tokyo",
    "ll": [35.695126,139.75391]
    "moniker": "Coinbase Cloud 02",
  },
  {
    "slot": 2,
    "absoluteSlot": 264816002,
    "leader / nodePubkey ": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
    "votePubkey": "6D2jqw9hyVCpppZexquxa74Fn33rJzzBx38T58VucHx9",
    "country": "JP",
    "timezone": "Asia/Tokyo",
    "ll": [35.695126,139.75391]
    "moniker": "Coinbase Cloud 02",
  },
  {
    "slot": 3,
    "absoluteSlot": 264816003,
    "leader / nodePubkey ": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
    "votePubkey": "6D2jqw9hyVCpppZexquxa74Fn33rJzzBx38T58VucHx9",
    "country": "JP",
    "timezone": "Asia/Tokyo",
    "ll": [35.695126,139.75391]
    "moniker": "Coinbase Cloud 02",
  },
  {
    "slot": 4,
    "absoluteSlot": 264816004,
    "leader / nodePubkey": "3fpcsJ2WPdrmpjVVA5Lmv4m9Qx5xqND1xJhFprDSjWJ4"
    "votePubkey": "6D2jqw9hyVCpppZexquxa74Fn33rJzzBx38T58VucHx9",
    "country": "JP",
    "timezone": "Asia/Tokyo",
    "ll": [35.695126,139.75391]
    "moniker": "Coinbase Cloud 02",
  },

  

3. Extra quest, combine all the code into 1 .mjs file and the output would simply look like the example above.






~~**Run create_ordered_leader_schedule.js to get a leader schedule with the identity address of validator next to "leader:"**~~

~~i.e.
  "leader": "MCFmmmXdzTKjBEoMggi8JGFJmd856uYSowuH2sCU5kx"
  "leader": "identity address of validator/leader"~~

~~This is useless as we need VoteKey address of validator.

~~We can fetch the location and validator information by extracting the VoteKey addresses of all validators. We fetch all VoteKey addresses of each validator first, then use this to fetch the information of each validator. 
**Then hopefully the information of each validator can be linked back to the identity address of each validator.**~~


~~**New things to add once we link things up (VoteKey, Location and Coordinates are all in):**~~
~~[
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
  },~~
