# Check If You Are Featured on Mixer With MixItUp
This will give you a command to check. You could put it on a timer or something.

## Setup
1. Create a  new action group and name it something like amifeatured

2. Add a Special Identifier
  - Enter amifeatured in the 1st field
  - Enter No in the 2nd field
  - Make globally Usable active
  
3. Add another Special Identifier
  - Enter myfeaturelevel in the 1st field
  - Enter 0 in the 2nd field
  - Make globally Usable active
  
4. Add a Web Request
  - with your channels query https://mixer.com/api/v1/channels/platypusmuerte
  - Select JSON to Special Identifiers as action
  - put featured in 1st field and amifeatured in 2nd
  - Add another row, and put featureLevel and myfeaturelevel in the boxes
  
5. Add a Chat action, as a whisper to streamer
  - Featured: $amifeatured ($myfeaturelevel)
