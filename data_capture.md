##Data Capture Templates

The tables we use for data capture each have standardized column headings. It is not necessary to fill in all of the columns for each record you enter, though more data will give a more complete visualization.

####General Rules
Uncertain dates: All of the date related fields include a "raw" column, like "BirthDateRaw". These fields are text string fields, meaning that you can include punctuation, question marks, etc. Use this column to capture the actual date information, even if it is uncertain, such as "late 1763" or "March? 1753" or "1734-35". The day/month/year columns cannot include anything other than number. No dashes or date ranges. If the month is uncertain, you can either pick a month or leave it blank. The preferred approach is to leave the field blank rather than guessing. We will reveal the "raw" field in the visualization for reference.

Uncertain places: As with dates, we have a "raw" field for all places. Use this field to capture location as recorded, including street addresses, building names, etc. The City/Province/Country fields should only include proper names - no punctuation, question marks, etc. If it is not known, leave it blank. 

People and Organizations: Enter multiple authors or recipients in the same field separated by two colons with no spaces "::". We attempt to match correspondents against our existing database when the correspondence spreadsheet is uploaded to our system. You'll be able to download a "person" spreadsheet that will indicate successful and unsuccessful matches. At that point you can correct mismatches and add biographical details to enrich the person list.



###Archive 
If the correspondence data is a direct export from an existing digitized archive, add a record here. 

###Collection
If the data has been collected by an individual for inclusion in our database, add a record under Collection.

###Biographical Data Schema   

RawName = Name as it comes to us, constructed by taking a correspondence selection and isolating unique authors and recipients to create a single list of unique correspondent-- this field is temporary and we will be getting rid of it down the road, but you'll need to keep it as the starting point for each Biographical Data spreadsheet  --> this is the column that will match together the biographical information with correspondence data.

Full Name =  Should match name in the correspondence list-- needs to match author/recipient in Correspondence Data, Shortest version of a recognizable name for the individual, name will appear as a label in visualizations, Voltaire is the Full Name not F.M.A. etc (sometimes this will be the person's title)

Alias = often more than one Alias, for more than one value separate with "::" with no spaces, include variations on the same (variations in spelling), pen names, etc.  Variations on the name will allow the database to find the person by searching with any number of variations on the name

Title = can be repetative with Alias, this allows us to capture a more refined version of alias in some cases, we may formalize this more later
Gender = 
BirthYear = (follow same date format described in Correspondence Data Schema)

BirthMonth =

BIrthDay =

DeathYear =

DeathMonth =

DeathDay = 

BirthCity = (follow same place format as is Correspondence Schema)

BirthCourntry =

DeathCity =

DeathCountry = 


###Letter_Events Schema   

SourceArchive = If you are using more than one source archive, put the name here. This should match the name entered in the Archive spreadsheet. If you only have one source, you can leave this blank and the name will be taken from the single entry in the Archive spreadsheet.

InventoryNumber = If there is a unique identifier from your source, make note of this in the collection annotation and use this field to record that unique number.

Author = Enter the commonly used name for this person. Separate multiple authors with two colons.  ::

Recipient = Enter the commonly used name for this person. Separate multiple authors with two colons.  ::

DateRaw = Enter the date just as it is in your source, warts and all

DateYear =  YYYY Numbers only. No dashes. Leave blank if unknown

DateMonth = MM.  Numbers only. No dashes. Leave blank if unknown

DateDay = DD  Numbers only. No dashes. Leave blank if unknown

URI = If there is a unique URL for this letter in an online archive, enter it here. If not, leave it blank.

SourceRaw = Enter address just as it was recorded. Any language. Any format.

SourceCity = Enter City in English. Modern city names are preferable, when available. This field is used for LatLon lookup. The historical location name appears in SourceRaw.

SourceProvince = Enter Province in English if known. Use this field for US states, Italian republics, etc.

SourceCountry = Enter country in English. Modern country boundaries are preferable. This field is used for LatLon lookup.

DestinationRaw = Enter address just as it was recorded. Any language. Any format.

 DestinationCity = Enter City in English. Modern city names are preferable, when available. This field is used for LatLon lookup. The historical location name appears in DestinationRaw.

DestinationProvince = Enter Province in English if known. Use this field for US states, Italian republics, etc.

DestinationCountry = Enter country in English. Modern country boundaries are preferable. This field is used for LatLon lookup.

 DestinationLatLon = If you would like to record a specific street address, add coordinates here.
 
 

###Group/Institution Schema

GroupName = The full official name of the group, default to English spelling

ShortName = Shortest legible version to appear in a visualization

Alias = Alternative spellings or constructions of the group's name. For more than one value separate with "::" with no spaces.

Location = (can be multiple values) Places associated with this group. Place name comma geonamesid or lat/lon. For more than one value separate with "::" with no spaces.

### Connection Events Schema 

*Connections may not include a location. If, for example, entities are in different locations, we use the chronology or biographical data to infer location.*

Entity1 = 

Entity2 = 

StartDate = 

EndDate =

PlaceRaw = Place name

PlaceID = Internal unique identifier

Geonames = Geonames ID

EventDescription = (controlled vocabulary) Marriage, Death, Meeting, Divorce, Mentioned

EventNotes = (string) Keep it simple, but you can add any relevant notes here.





### Travel Events

**Travel events are recorded by person.**


Person (Full Name) = Should match biographical data.

PersonID =  Will be generated once this collection is complete

StartDateRaw = This is start time as taken directly from the text (could also be understood as descriptive)

EndDateRaw = This is start time as taken directly from the text (could also be understood as descriptive)



 
 
 