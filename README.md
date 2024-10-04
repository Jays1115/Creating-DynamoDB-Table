<h5>Directory</h5> 

<b>[Tech Portfolio Home](https://github.com/Jays1115/Jalen-Smith.git)</b> /
<b>[AWS Projects & Labs](https://github.com/Jays1115/AWS-Projects.git)</b>

# Creating DynamoDB Table

<h2>Description</h2>
Scenario: A local streaming service wants to enhance its product by introducing features like a digital bookmarking to resume watching shows where users left off, using a flexible NoSQL database. The service aims to gather and handle large volumes of metadata on viewing habits for scalability and lightning-fast performance to support continued expansion and feature integration.
<br><br>
Solution: Set up a NoSQL database using Amazon DynamoDB to support a streaming service that requires high scalability and performance. The database will store digital bookmarks and metadata on customer viewing habits.

<h2>Program walk-through:</h2>

<p align="center">
Navigated to the dynamodb page: <br/>
<img src="images/Screenshot 2024-09-20 at 12.18.02 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.18.22 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
A new DynamoDB table has been successfully created. The partition key has been configured as "UserID," and the sort key has been set to "LastDateWatched": <br/>
<img src="images/Screenshot 2024-09-20 at 12.20.35 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.21.21 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.21.39 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.26.04 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
An item has been added to the UserVideoHistory table in DynamoDB, containing essential attributes to enhance user experience tracking: <br/>
- UserID (Partition Key): 12345-abcd-6789 - Uniquely identifies the user. <br/>
- LastDateWatched (Sort Key): 1619156406 - Timestamp of the user's last viewing. <br/>
- VideoID: 9875-djac-1859 - Specifies the video content watched. <br/>
- PreferredLanguage: English - Indicates the user's language preference. <br/>
- SupportedDeviceTypes: Includes devices like Amazon Fire TV and Fire Tablet, showing the platforms used by the viewer. <br/>
These attributes are crucial for personalizing the streaming service, ensuring continuity across sessions, and refining content recommendations: <br/>
<img src="images/Screenshot 2024-09-20 at 12.27.03 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.27.16 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.33.55 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.36.29 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
I expanded the "Scan or Query Items" dropdown menu to perform a search query. Since only one item has been added so far, that is the sole result displayed in the search outcome: <br/>
<img src="images/Screenshot 2024-09-20 at 12.41.07 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.43.12 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

<p align="center">
I expanded the "Scan or Query Items" dropdown menu to initiate a scan. As only one item has been added to the table, it appears as the exclusive result in the search: <br/>
<img src="images/Screenshot 2024-09-20 at 12.44.53 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="images/Screenshot 2024-09-20 at 12.45.01 PM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
</p>

