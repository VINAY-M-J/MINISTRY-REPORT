
# Government Officials Contact Information Analysis

This Power BI project involves collecting and analyzing comprehensive information about key government officials from various departments across the 29 states in India. The primary goal is to gather data on the current ministers, principal/additional secretaries, secretaries, and commissioners for several sectors, including school education, higher education, medical education, social welfare, tribal department, skill development, rural department, and zilla panchayat.

# Distribution of Social-Media Handles Of Ministers / Bureaucrat Across India

### Dashboard Link : https://app.powerbi.com/links/s91Hazp1aI?ctid=191dd60d-090a-4459-a071-b03c80f3ac3b&pbi_source=linkShare

## Problem Statement

This dashboard helps in addressing the critical need for transparency and accessibility of government officials' contact information across India's 29 states. By meticulously collecting data on ministers, principal/additional secretaries, secretaries, and commissioners spanning diverse departments such as school education, higher education, medical education, social welfare, tribal affairs, skill development, rural development, and zilla panchayats, this Power BI project offers a comprehensive overview of the administrative landscape. Moreover, it goes beyond merely listing officials by incorporating their contact details, including email IDs, phone numbers, and various social media profiles such as Instagram, Facebook, Twitter, and YouTube. This holistic approach not only provides stakeholders with a centralized repository of vital information but also promotes accountability and facilitates direct engagement with key decision-makers at different levels of governance.

Through intuitive visualizations, including matrices, maps, and clustered column charts, this dashboard illuminates the extent to which government officials embrace digital communication platforms. It quantifies the presence of contact information among officials, offering insights into the accessibility of channels such as email, phone, and social media. By delineating the proportion of officials within each category who have furnished contact details, this analysis informs strategies for enhancing transparency and fostering efficient communication channels between citizens and government representatives. Ultimately, this Power BI project serves as a catalyst for promoting digital governance and citizen participation, paving the way for more informed, inclusive, and responsive public administration across India's diverse administrative landscape.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : It was observed that in Facebook, Twitter, Intsagram, YouTube, Email ID and Contact Number there were empty values. All these columns were filled with "Null" in Power Query Editor.
- Step 3: Created a new column to store the count for Facebook, Twitter, Intsagram, YouTube, Email ID and Contact Number using  DAX Queries, it will assign 0 if the cell is null/empty and it will assign 1 if there is value in the cell.

The following DAX Queries was added:

(a) TwitterCount = IF(ISBLANK([Twitter]), 0, 1)

(b) FacebookCount = IF(ISBLANK([Facebook]), 0, 1)

(c) InstagramCount = IF(ISBLANK([Instagram]), 0, 1)

(d) YoutubeCount = IF(ISBLANK([Youtube]), 0, 1)

(e) MailCount = IF(ISBLANK([Email ID]), 0, 1)

(f) contactCount = IF(ISBLANK([Contact Number ]), 0, 1)

- Step 4 : For calculating unique number of ministers, secretary, commissioners, principal / additional secretary, We removed duplicates from "Name" column in Power Query Editor.
- Step 5 : A clustered column chart was added to the canva to show Unique number of Ministers / Bureaucrat. 
- Step 6 :  A clustered column chart was added to the canva to show social media counts (Facebook, Twitter, Intsagram, YouTube, Email ID and Contact Number).
- Step 7 : Visual filters (Matrix) were added to canva for Ministers / Bureaucrat field and values named TwitterCount, FacebookCount, InstagramCount, YoutubeCount, MailCount, contactCount .
- Step 8 : One Geographical visual was added to the canvas, which gives the state wise data / information.
           
           Although, by default, while selecting each state the numbers used to change in matrix as well as stacked column charts.

  (1) Andhra Pradesh

  (2) Arunachal Pradesh

  (3) Assam

  (4) Bihar

  (5) Chhattisgarh

  (6) Delhi

  (7) Goa

  (8) Gujarat

  (9) Haryana

  (10) Himachal Pradesh

  (11) Jharkhand

  (12) Karnataka

  (13) Kerala

  (14) Madhya Pradesh

  (15) Maharashtra

  (16) Manipur

  (17) Meghalaya

  (18) Mizoram

  (19) Nagaland

  (20) Odisha

  (21) Punjab

  (22) Rajasthan

  (23) Sikkim

  (24) Tamil Nadu

  (25) Telangana

  (26) Tripura

  (27) Uttar Pradesh

  (28) Uttarakhand

  (29) West Bengal

- Step 9 : In the report view, under the insert tab, one text box was added to the canvas, the title of the project is mentioned in the box.

# Snapshot of Dashboard (Power BI DESKTOP)

![MINISTRY DASHBOARD](https://github.com/VINAY-M-J/MINISTRY-REPORT/assets/170668374/ac13129e-bfa0-47df-96bd-de424c632860)


