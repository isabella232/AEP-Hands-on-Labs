Lab 1.1 - Ingestion - Simple CSV Ingestion
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>There are several ways to push up CSV data into AEP.  This lab will walk-through the "simple" approach-- please note though, this creates a schema that is non-standard or conforment to AEP
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br><li>download "simple_csv_example.csv" file</li></td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_identities.png?raw=true" alt="Identities"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left-hand menu, navigate to "Workflows"
2. Select "CSV Import" option
3. Follow workflow instructions

NOTE: This technique is a valid option for Data Science Workspace (DSW) or other ad-hoc manner datasets that don't require connection to unified profile 
<br>
<br>
<br>







Lab 1.2 - Ingestion - CSV to XMD Mapping
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>This lab will show you how to add CSV data to the AEP datasets in a manner that will be usable (or conformed) to either the user Profile or Experience Event schema.
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br><li>download "csv_to_xdm_mapping.csv" file</li>
                            <li>schema in place</li>
                            <li>dataset in place</li>
           </td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_identities.png?raw=true" alt="Identities"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left-hand menu, navigate to "Workflows"
2. Select "Map CSV to XDM schema"
3. The next workflow sequence will be:
   - Add Data
   - Destination
   - Mapping
   - Ingest
4. Select CSV file for upload
5. Select "Student Performance Dataset"
6. This is where mapping is needed, the system will assume certain values...
    Please WAIT HERE as a class - we'll work through this section together
7. Once done, hit submit and wait for ingestion process to complete
 
<br>
<br>
<br>



Lab 2.1 - Dataset - Adding data via JSON
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>Provided if a dataset is already in place, AEP allows for data architects to add/upload either Parquet files or JSON files directly to the dataset.
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br><li>downloaded "ad_hoc_json_upload.json" file</li>
                            <li>schema in place</li>
                            <li>dataset in place</li>
           </td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_identities.png?raw=true" alt="Identities"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left-hand menu, navigate to "Datasets"
2. Select the dataset named "Student Performance Dataset"
3. On the lower right-hand menu, click the "Drag and drop file(s) or Browse" area
```
    WARNING: Once you select the file in this interface, AEP immediates attempts to ingest it--
    there isn't a seperate initiation or confirmation page/button.
```     
4. Upload and processing should begin (I usually click in-and-out of a different batch to have the current batch update its progess -- I believe there's an AJAX call updating in the browser UI)
5. Confirm that the upload was a success by drilling into batch details
 
<br>
<br>
<br>





Lab 7.1 - Segmentation - Profile Attribute Segmentation
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>In this lab, you will learn how to create a segment based on a profile attribute/characteristic that has been mapped within unified profile
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br>none</td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_segments.png?raw=true" alt="Segments"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left navigation, select ‘Attributes’ under ‘Fields’
2. Select ‘XDM Indvidual Profile’ under ‘Browse Attributes’
3. Select ‘Adobeamericaspot 2’ under ‘Attributes’ > ‘XDM Individual Profile’
4. Expand the ‘Student’ object
5. Once the fields display, drag ‘jobTitle’ over to the Segment Canvas.
6. Finish creating the segment where ‘jobTitle’ contains ‘manager’
7. In the Segment properties pane, select the ‘Refresh estimate’ link
8. Please do not save your segment

NOTE: Estimate link may not show results if attribute or selection is statistically small and not recognized across datset scans 
<br>
<br>
<br>


Lab 7.2 - Segmentation - Profile Experience Event Segmentation
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>Similar to the prior lab, in this lab you will build a customer segment based on the unified experience event data (from EE Schemas/Datasets) that are streaming into plartform</td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br>none</td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_segments.png?raw=true" alt="Segments"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left navigation, select ‘Events’ under ‘Fields’
2. Select ‘XDM ExperienceEvent’ under ‘Browse Classes’
3. Select ‘Experience’ under ‘Events > XDM ExperienceEvent’
4. Select ‘Analytics’ under ‘Events > XDMExperienceEvent > Experience’
5. Expand ‘Event 1 to 100’
6. Expand ‘Account Creation: Step 1 (event33)’
7. Drag the field to the Segment Canvas
8. Modify the condition for this field to ‘exists’
9. In the left navigation, click on ‘Event 1 to 11’
10. Click on ‘Account Creation: Step 2 (event34)’
11. Drag the field to the Segment Canvas to the right of the existing event
12. Modify the condition for this field to ‘exists’
13. Expand ‘Event 1 to 100’
14. Click on ‘Accounts Created’
15. Drag the field to the Segment Canvas to the right of the second event
16. Modify the condition for this field to ‘does not exist’
17. In the Segment properties pane, select the ‘Refresh estimate’ link
18. Please do not save you segment


<br>
<br>
<br>



Lab 15.0 - Deep Dive \[Query Serive\] - Setup to Query Service
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>This will guide you through the steps to configure QS either through Terminal (mac) or PowerShell (windows)
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br><li>installed PSQL on your machine</li>
                            <li>perhaps having OS admin rights?</li>
           </td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_queries.png?raw=true" alt="Queries"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Instructions:
-----------------
1. In the left-hand menu, navigate to "Queries"
2. In the upper-mid-menu, navigate to "Credentials"
3. Within the 2nd column on the left (greyed out and with the phrase "PSQL command" above it), locate the 2 overlapped box icon within the embedded text area, and click that to copy this whole PSQL command.

```
NOTE: don't click the "Learn more" exit box that's just above the copy command
```

4. Paste that copied portion into either Terminal or PowerShell

<br>
<br>
<br>


Lab 15.1 - Deep Dive \[Query Serive\] - Simple commands within PSQL
==========
<table style="border-collapse: collapse; border: none;" class="tab" cellspacing="0" cellpadding="0">

<tr style="border: none;">

<div align="left">
<td width="600" style="border: none;">
<table>
<tbody valign="top">
      <tr width="500">
            <td valign="top"><h3>Objective:</h3></td>
            <td valign="top"><br>This will cover a few simple commands within PSQL if you're unfamiliary with the SQL-syntax
            </td>
     </tr>
     <tr width="500">
           <td valign="top"><h3>Prerequisites:</h3></td>
           <td valign="top"><br>none
           </td>
     </tr>
</tbody>
</table>
</td>
</div>

<div align="right">
<td style="border: none;" valign="top">

<table>
<tbody valign="top">
      <tr>
            <td valign="middle" height="70"><b>section</b></td>
            <td valign="middle" height="70"><img src="https://github.com/adobe/AEP-Hands-on-Labs/blob/master/assets/images/left_hand_nav_menu_queries.png?raw=true" alt="Queries"></td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>version</b></td>
            <td valign="middle" height="70">1.0.1</td>
      </tr>
      <tr>
            <td valign="middle" height="70"><b>date</b></td>
            <td valign="middle" height="70">2020-01-06</td>
      </tr>
</tbody>
</table>
</td>
</div>

</tr>
</table>

Quick Command Guide:
-----------------
```\dt``` or ```\d``` listing all dataset tables

```\dt <table_name>``` list details of dataset table

```\a``` toggle from aligned to non-aligned format

```\o``` output format (I'll need to check this out)

```\q``` or ```quit``` exits the commandline



4. Go here to find more: 

<br>
<br>
<br>
