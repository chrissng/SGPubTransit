<b>SGPubTransit</b> is a door-to-door multi-mode public transport mapping and spatiotemporal analysis dataset for esri ArcGIS. It is aware of all bus, MRT and LRT services in Singapore. Combined with ArcGIS Network Analyst extension, this tool does more than just finding shortest routes. Generating O/D travel cost matrices, determining service areas, analysing spatio-temporal accessibility, and solving the travelling salesman problem are just few of the many possible applications offered by this tool.

### How is it built with esri ArcMap ###

Detailed here: http://sgtptr.chrissng.net/appendices/02.pdf

### Applications ###

- Identifying redundancy in Singapore's public transport system: http://sgtptr.chrissng.net/
- Public transit time maps: http://geoseyeview.wordpress.com/2013/10/19/a-visual-update-to-the-public-transit-time-map-from-my-workplace/

### Public transport modes ###

<p align="left">
  <img src="https://s3-ap-southeast-1.amazonaws.com/chrissng/img04_connectivity.png" width="50%"/>
</p>

- All SBS and SMRT Bus services
- North-South MRT Line, East-West MRT Line, North-East MRT Line, Circle MRT Line (and extensions currently U/C)
- Bukit Panjang LRT Line (Svc A, B, and C), Sengkang West LRT Line, Sengkang East LRT Line, Punggol West LRT Line, Punggol East LRT Line
- Sentosa Express
- Future MRT lines (according to media and LTA in 2012): Downtown MRT Line (U/C), Thomson MRT Line (by 2020), Eastern Region Line (by 2020)

### Cost evaluators ###

- Travel time
- Travel distance
- No. of transfers

### Constraints ###

<p align="left">
  <img src="https://s3-ap-southeast-1.amazonaws.com/chrissng/img03_cost.png" width="75%"/>
</p>

- Transfers are approximated as straight line distances, average walking speed of 5kph.
- Transfers allowed only among bus stops, interchanges and train stations within 400m.
- Any transfer to a Bus service incurs a waiting penalty of 12 mins.
- Any transfer to a Train service incurs a waiting penalty of 3 mins.
- Bus travels at an average speed of 20kph on roads and 40kph on expressways.
- Train stopover time at station is 0.2 min.
- Bus stopover time at bus stop is 0.5 min.

### Data sources are correct as at March 2012 ###

- Bus route information: Transitlink
- Bus stops and Train stations:	Land Transport Authority 
- URA Planning areas: Urban Redevelopment Authority
- Road (Linear features): OpenStreetMap (Dec 2011)
