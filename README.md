# SignalScope   
## See how Wi-Fi coverage changes across Times Square throughout the day   
GPS, Sensor, Time     
</div>  
##Idea    
Wi-Fi quality can change from one side of a street to the other. Buildings may block signal, crowded areas have higher demand, and connection amy fall.  
SignalScope turns these changes into a readable map. The prototype uses Wi-Fi modeling in Times Square, letting the user compare expected coverage at different times. The full map is shaded, so strong, weak, and fluctuating areas are clearly, and fully visible.   
##Problem  
Public Wi-Fi maps usually show where hotspots are, but do not explain if the connection is better at one specific area than another, especially in consideration to time. This makes it more difficult for students, remote workers, organizers, teams, etc, to find a dependable location for work.    
##Wildcard Integration   
###GPS: Associates readings with location, so measurements have a map placement    
###Sensor: Represents computer or phone network sensor, recording signal strength and connection   
###Time: Readings are altered throughout the day caused by crowd activity  
##Prototype   
The prototype focuses on reading Wi-Fi coverage around Times Square.   
 -Switch from 8:00 AM to 12:30 PM to 6:00 PM    
 -Functions as a heatmap: green - strong, yellow - variable, red - weak.    
 -Zoom in or out    
 -Open project information panel for explanation    

 The interface is familiar, using a map orientation for users. Controls are simple, so that coverage is effective, and unfamiliar users have an easy experience.    
 ##Model Functionality    
 This model uses a theoretical frequency model instead of accurate measurements. It functions as a realistic demonstration of interpreted data.   
 Signal strength is estimated by:   
 1.) Distance from rooftop access points    
 2.) Path loss as distance increases   
 3.) Attenuation behind large building groups    
 4.) Signal advantage on open streets    
 5.) Time-based adjustment for busy daytimes   
 ##Resultant RSSI values:    
 >=-61dBm: Green
 -62-(-74)dBm: Yellow
 <-74dBm: Red
 This is a demonstration, or simulation, not a live test. A production version would replace assumed access points and estimates with device readings gathered over time.
 ##Prototype to real product
 A complete system could collect measurements of official RSSI, latency, packet loss, and download speed. Samples would pair with GPS coordinates and timestamps.
 Resulting effect:
 -Dependable connections discovered
 -Better work areas
 -Coverage gaps during emergencies
 -Help cities decide on infrastructure demands

 ##Built With:     
 -HTML   
 -CSS    
 -JavaScript   
 -SVG    
 -Heatmap rendering   
 ##Run locally:    
 1.) Download repository    
 2.) Open index.html in browser, or drag index.html file from downloads into browser unopened tab     
 
