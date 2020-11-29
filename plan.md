** Plan **
* Application will have Users
* Users can sign up, sign in, change their details
* Users can create sounds using the Piano.
* When the User presses Record on the Piano, we start a Session.
> A Session will have a sequence of Sounds. The order of the sequence will be as the User is playing. One Sound is analogous to one musical note.
> How do we store the time between two Sounds?
> The SoundSequence in a Session is constantly (how frequently?) updated on the server.
* When the User presses Stop on the Piano, the Session is closed and saved.
* A User can play back a Session (either made by them or shared with them).
* A User can edit or delete any of their Sessions. The name Session is not exposed to the User. User only sees the sounds that they created.

** For later **
* A User can search for other Users by email/username.
* A User can share Sessions with other Users.
* A User can edit Sessions that they are permitted to edit.
-------------------------------
Questions
* How do we store a sound?
> A Sound is stored in the db as binary data (BLOB?)
* If the user asks to download some sounds, how do we write sounds to an MP3 file?