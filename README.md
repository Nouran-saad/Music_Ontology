# Music_Ontology
<img src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/5308ecb5-b32b-4a84-8545-01cc5a8a60fb"  width="30%" height="5%" align="right">


***CSE488 Ontologies and the Semantic Web Project***
## Introduction
Our project is based on a Music Ontology that contains songs, their artists, including the singer
singing, the musician playing the background music, the writer that wrote the lyrics and the
composer. Our ontology also includes the bands and the artists they include, the awards won
by the artist and the instruments played by the musician. We used the Protégé ontology editor
developed by Stanford University to build our Music Ontology. Then we created a java
application and added Jena jar files to be able to create a GUI frame where we will be able to
write a SPARQL query, press execute and see the results of the query displayed in the form of
a table. We also created a JavaScript web application that contains a text field for the queries,
a button to run the query and a table to display the results.
## CLASSES
* Album: To contain the songs.
*	Award: Given to artists.
*	Band: To have artists that play songs together.
*	Instrument: The instruments that the musician will play.
*	Person: Parent class of Artist, for expansion purposes if wanted to add different type of people that are not artists.
*	Artist: Parent class of Composer, Musician, Singer, and Writer, which are all considered artists.
*	Composer: Composes songs.
*	Musician: Plays instrument.
*	Singer: Sings the songs.
*	Writer: Write the song lyrics
*	Song: The actual song class that has a name, language and other properties discussed in the following sections.
<p align="center">
<img src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/4faeb219-8960-4db4-972b-b5e28d6ec0a2"  width="30%" height="5%">
</p>

## OBJECT PROPERTIES
*	Composed: connects Composer to Song. 
*	Contains: connects Album to Song.
*	hasArtists: connects Band to Artist.
*	hasAwards: connects Artist to Award.
*	hasInstruments: connects Song to Instrument.
*	hasWritten: connects Writer to Song.
*	Plays: connects Musician to Instrument. 
*	Sung: connects Band/Singer to Song. 
<p align="center">
  <img width="30%" height="5%" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/d9d132d0-e1a6-4ca8-8741-1357223465dd">
</p>

## RESTRICTIONS
1. Each Album contains at least 1 and at most 15 songs.
2. Each Band has at least 2 Artists.
3. Each Band sung at least 1 song.
4. Each Song has at least 1 instrument.
5. Each Composer composed at least 1 Song.
6. Each Musician Plays at least 1 Instrument.
7. Each Singer sung at least 1 Song.
8. Each Writer has Witten at least 1 Song.
## DATA PROPERTIES
![image](https://github.com/Nouran-saad/Music_Ontology/assets/55962261/d6d9c997-1262-4714-9eef-c210c25bf11b)

## Examples of The Instances
### Instances of the Albums
<p align="center">
  <img width="30%" height="5%" align= "left" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/ba24161e-2100-4c1c-a14d-b686917a91a6">
  <img width="30%" height="5%" align= "right" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/0f2d2eaf-981c-4cbf-8539-bf5e9398f9ec">
  </p>
  <br />
    <br />
      <br />
        <br />
          <br />
            <br />
              <br />
                <br />
                  <br />
                    <br />
                      <br />
                
### Instances of the Songs
<p align="center">
  <img width="30%" height="5%"  align= "left" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/fe82d867-68c3-4954-826d-802014689353">
  <img width="30%" height="5%"  align= "right" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/dcb030d4-36b9-4c66-93af-57ad3d299daf">
    </p>
      <br />
    <br />
      <br />
        <br />
          <br />
            <br />
              <br />
                <br />
                  <br />
                    <br />
                      <br />
                      <br />
                      <br /> 
                    <br />
                      <br />
                      <br />
                      <br /> 
                      
## GUI of the Java Application
* Text field to write the queries in.
* Button to run the query.
* Table to display the result of the query. 
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/822046fa-ef7d-4128-bde4-a4f91873d810">
</p>

## GUI of Java Script Web App
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/5f813a8b-03aa-497c-b2c3-8ef5287d751d">
</p>


## SPARQL Queries and Results
1. List the songs(name, genre, views) sung by Selena Gomez ordered by release data and the album that each song belong to.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/f23fe008-8252-4b98-b385-473aa7a39a66)">
</p>

2. List the awards taken by Selena Gomez with the date and type
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/74450192-8392-41ab-8ac2-f6002f82e9da">
</p>

3. List the songs of the album everyday life or ghost stories with the instrument used in every song.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/70d58285-00ea-4e30-8ac6-74c52175657e)">
</p>

4. List the names and the ages of the members of the band Coldplay and awards if they have.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/d009e09e-f82d-4174-9ba9-688ff329195f">
</p>

5. List the songs of BTS band that exceed million views and their duration.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/b52f0e37-714d-47d1-b0a6-8dfee2fc5b3e">
</p>

6. List the Ids , names , genre and language of BTS songs.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/45bd3e86-e4d0-4744-a9dd-9948c7bbd520">
</p>


7. List the artist names , ages and top hits of the BTS band that sung songs.
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/8d47a6e8-ecb4-406b-99c7-1760e0e16703">
</p>

#### ASK QUERY 1
Ask if there exists a singer whose name is Selena Gomez , and has award. The award has a name, type and date
<p align="center">
<img width="40%" height="10%"  align= "center" src="https://github.com/Nouran-saad/Music_Ontology/assets/55962261/318611b3-7271-4f07-9a7c-684ff6364a32">
</p>

#### ASK QUERY 2
Ask if there exists a singer whose name is Salma , and has award. The award has a name, type and date
<p align="center">
<img width="40%" height="10%"  align= "center" src="![image](https://github.com/Nouran-saad/Music_Ontology/assets/55962261/68186d0f-9026-4a48-8825-d0b841165eae)">
</p>







