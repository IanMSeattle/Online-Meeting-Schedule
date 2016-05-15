# Online-Meeting-Schedule
A GoogleMaps API enabled Django site using MySQL to create and maintain an online listing of regularly scheduled public events.

The program:
  1. takes input as a csv, excel file, or from a clipboard copied from a web page, 
  2. saves it to a unique table in a MySQL database
  3. uses python code to perform cleaning functions to prepare it for submission to the GoogleMaps GeoCode Api
  4. submits each record and returns the geocoded address to the appended MySQL database
  5. creates an admin page that allows:
      1. display of returned results manual editing of the address, details, and profile of the meeting
      2. revision and update of individual meeting data
      3. creation of new meeting data
      4. deletion or deactivation of meetings
  
  6. exposes the results of a website that:
      a) allows searching for meeting by proximity to the user, area or district membership, or city name
      b) allows screening of the results by characteristic in the meeting profile
      c) allows user to save meeting information as a contact in their mobile device
      d) allows user to secure directions to the meeting using Google Maps
      e) allows user to identify all meetings at a given location
      f) creates the ability to utilize the code within an external host domain invisibly to the end user - the user will see an url     like <www.foo.org>/meetingname/city
 
 7. built on a datamodel for meetings that includes;
      -meeting name
      -meeting frequency (e.g. every Tuesday at 7 pm, Last Tuesday of the month at 8 pm)
      -group name
      -area name
      -location name
      -google location id
      -latitude and longitude
      -comments that allow direction to a specific room or entrance etc
      -profile according to a legend (eg. open, closed, ASL)
      -GSR
      -GSO number
      -last updated and updated by date and time

Additionally:
  1. Creates an administrative structure for meeting organizers at the Area, District, and Group levels, including commitee membership
  2. Allows for creation of more detailed meeting profiles including Group membership and GSR contact information
  3. Allows for mapping of Groups and Meetings to District definitions by city, zip code or geographic shapefiles
  4. Creates an 'app ready' data service for eventual optional integration into a mobile app
  5. Automatically creates necessary tagging and citations to optimize Google Local search
  



      
