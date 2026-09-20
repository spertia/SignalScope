# SignalScope

## See how Wi-Fi coverage changes across Times Square throughout the day

**GPS, Sensor, Time**

## Inspiration

Reliable Wi-Fi can frequently change depending on location, and time of day. I've experienced this in my personal life, as simply going across a building can cause your signal to disappear, which has been a conflict, in our modern, technological world. This is especially noticeable in large public spaces, such as schools, libraries, events, and more. I wanted to make these changes visible instead of relying on a wifi-speed test for one specific location.

## What it does

SignalScope uses repeated network measurements to create a coverage map. Users can compare performance, weak readings, and fluctuations of wifi throughout the day.

### Coverage Levels:

- Green: Strong, stable connection
- Yellow: Moderate connection
- Red: Weak, unstable connection

This can help schools, centers, event organizers, and technicians identify areas needing further signal testing or methods for improving Wi-Fi coverage.

### Problem:

Public Wi-Fi maps usually show where hotspots are, but do not explain if the connection is better at one specific area than another, especially in consideration to time. This makes it more difficult for students, remote workers, organizers, teams, etc, to find a dependable location for work.

### Wildcard Integration:

- **GPS:** Associates readings with location, so measurements have a map placement
- **Sensor:** Represents computer or phone network sensor, recording signal strength and connection
- **Time:** Readings are altered throughout the day caused by crowd activity

## How we built it

I created a web prototype using HTML, CSS, JavaScript, and SVG. The interface uses Times Square as a demonstration area, with interactive time, filters, GPS support, controls, live simulation, etc. The current Wi-Fi measurements are simulated, since standard browsers do not have access to Wi-Fi signal strength. The prototype demonstrates a full standard experience. A production version may implement Android applications for RSSI, latency, packet-loss, GPS, and more.

### Prototype:

- Switch from 8:00 AM to 12:30 PM to 6:00 PM
- Functions as a heatmap: green - strong, yellow - variable, red - weak
- Zoom in or out
- Open project information panel for explanation

The interface is familiar, using a map orientation for users. Controls are simple, so that coverage is effective, and unfamiliar users have an easy experience.

### Model Functionality:

This model uses a theoretical frequency model instead of accurate measurements. It functions as a realistic demonstration of interpreted data.

Signal strength is estimated by:

1. Distance from rooftop access points
2. Path loss as distance increases
3. Attenuation behind large building groups
4. Signal advantage on open streets
5. Time-based adjustment for busy daytimes

### Resultant RSSI values:

- −61dBm: Green
- −62--(−74)dBm: Yellow
- <−74dBm: Red

> This is a demonstration, or simulation, not a live test. A production version would replace assumed access points and estimates with device readings gathered over time.

### Built With:

- HTML
- CSS
- JavaScript
- SVG
- Heatmap rendering

### Run locally:

1. Download repository
2. Open index.html in browser, or drag index.html file from downloads into browser unopened tab

## Challenges we ran into

The largest challenge was presenting the various types of information without map reading conflicts for the user. I replaced measurement markers with heat zones, creating red, yellow, and green coverage areas for more effective recognition. Another challenge was signal strength and connection quality being difficult to seperate, since strong Wi-Fi may not always have a reliable connection. I also had to use browser privacy, so real connection cannot be achieved, but simulated data with GPS coordinates still effectively completes the goal.

## Accomplishments that we're proud of

I'm proud of combining simple words into a practical product. My product has the capability to assist many people in their day to day lives. A responsive prototype visualizing Wi-Fi performance changes with easy readability may be implemented in the future to assist citizens. I'm also proud of the limits extended by this product, creating more than a network speed test, and demonstrating a more fleshed out, complex, problem solving mechanism than traditional standards allow for.

## What we learned

I learned that location alone is not reliable for network details. Measurements are much more useful when compared over time and paired with latency and stability readings. I also learned that effective visualization can help with decision making. SignalScope is designed to show additional testing, adjustment, improvement or alteration demanding locations.

## What's next for SignalScope

The next step is to connect the interface to an Android data collector, to read real Wi-Fi signal. Secure local storage, community feedback, confidence scores, floor-plan differentiation, and more may improve the effectiveness of the product.

## Words Chosen

The selected words were GPS, Sensor, and Time
