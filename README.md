# Group17FinalProject
**Title of Project**
Song Database

**Team Members**
Justin Woo (section 3)
Deo Gracias Ong (section 3)
Lex Lei (section 3)
Gyuwon Lee (section 3)

**Brief Description of Project**
The song database aims to create a platform where songs can be stored according to each user’s preferences (similar to Spotify playlists). Each song has a specific genre to them, which can help users determine which songs they want in their playlists. Users can also determine which songs the general public likes by looking at the rating. Playlists that appeal to several users can ‘follow’ the playlist, increasing its following count. The platform comes with a user interface that allows each user to navigate smoothly to different songs and playlists available to them. 

**Link to UML Diagram**
https://github.com/justintwoo/Group17FinalProject/blob/main/db_design_final_project_UML.pdf

**Description of User Data Model**
The user data model for our database is given the properties, first name, last name, username, password, date of birth, and email address. Each user can create playlists, store songs, and rate other playlists.

**Description of the Two Domain Object Data Models**
‘Playlists’ is the first domain object. It has properties such as ‘title’, ‘followers’, ‘created’, and ‘updated’; each property respectively corresponds to the name given to the playlist, the number of followers the playlist has, the date at which the playlist was created, and the date at which the playlist was most recently updated. ‘Playlists’ is used to store songs that the user has selected. 

‘Songs’ is the second domain object with properties such as title, artist, feature, and length.
The title is the name of a specific song. The artist is the main singer of the song with ‘feature’ as the guests that the singer performs with. Length is the length of the song in seconds. Each property provides the user an avenue for sorting and filtering their choice in music. 

**Description of the User to Domain Object Relationship**
Users and playlists have a one-to-many relationship. Each user can create as many playlists as they would like to. Each playlist can only have one user as its creator. 



**Description of the Domain Object to Domain Object Relationship**
Playlists and songs have a one-to-many relationship. The relationship indicates that a single playlist can have multiple songs within it. 

**Description of the Portable Enumeration**
Song’s enumeration is its genre. There are a limited amount of genres available, such as Rap, R&B, Pop, EDM, etc. This serves as a constraint for the number of songs as well as a medium for users to select which genre of music they would like to listen to. 

**Description of the User Interface Requirements**
The user interface that we plan to implement for our song database will allow for creating, reading, updating, and deleting each of the user models and domain object models. For each user model and domain object, there will be navigation to screens for various purposes:
Users
    Display all users
    Create User
    Edit User
    Delete User
Songs
    Display all songs
    Add Songs
    Delete Songs
Playlists
    Display all playlists
    Create playlist & add songs from song lists
    Edit Playlist
    Delete Playlist
Ratings
    View all ratings for each playlist
    Create rating for a playlist
    Delete rating for a playlist
