# career-vault-api-documentation-240-tutoring
Career Vault's school districts API documentation

## URL Parameters
Parameter | Description
------------ | -------------
page | A cursor for use in pagination. Returns the n-th chunk of perPage objects.
perPage | Returns up to this number of jobs per response. Must be an integer between 1 and 500 (otherwise, it will default to 100). Defaults to 100.
search | Returns jobs where JobTitle includes this string.
zipCode | Returns jobs where the ZipCode matches.
city | Returns jobs where the City matches.
district | Returns jobs where District matches.
state | Returns jobs where State matches.
distance | Sets the distance from the bordering circle around a city. Default is 5 (miles). 


## GET: List Jobs
### HTTP Request

```GET https://api.careervault.io/240tutoring/v1/jobs```

### JSON Response
```
{
  "pagination": {
    "page": 1,
    "perPage": 25,
    "pageCount": 360,
    "totalNumberOfPages": 360,
    "totalCount": 8996,
    "uniqueCompaniesCount": 90,
    "totalNumberOfJobs": 8996,
    "newJobsCount": 25
  },
  "data": [
    {
      "JobID": 26417,
      "JobTitle": "2021/22 Special Education Teacher, Elementary",
      "Location": "Mason Elementary",
      "District": "Leander Independent School District",
      "DistrictID": 5982,
      "City": "Leander,
      "ZipCode": 78646,
      "State": "Texas,
      "Url": "https://www.applitrack.com/leander/onlineapp/_application.aspx?posJobCodes=6224",
      "DatePosted": "2021-10-05T16:24:22.000Z",
      "Description": "<span class=\"normal\"><div style=\"text-align: center;\"> <center> <center> <center style=\"text-align: left;\"><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\"><strong>If hired, the State Board for Educator Certification will require all first time applicants for an initial credential to be fingerprinted as part of a national criminal background check. A cost of up to $49.00 will be charged for fingerprinting.</strong></span></span></center> </center> </center>  <div style=\"text-align: left;\"> </div> </div> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\"><strong>PRIMARY PURPOSE:</strong><br> To provide special education students with learning activities and experiences designed to help them fulfill their potential for intellectual, emotional, physical, and social growth. Develop or modify curricula and prepare lessons and other instructional materials to student ability levels. Work in self-contained, team, departmental, or itinerant capacity as assigned. <strong>This position may be contingent upon funding in whole or in part through state or federal grants.<br> <br> MAJOR RESPONSIBILITIES AND DUTIES</strong></span></span> <ul><li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Collaborate with students, parents, and other members of staff to develop IEP through the ARD Committee process for each student assigned.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Implement an instructional, therapeutic, or skill development program for assigned students and show written evidence of preparation as required.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Plan and use appropriate instructional and learning strategies, activities, materials, and equipment that reflect understanding of the learning styles and needs of students assigned.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Work cooperatively with classroom teachers to modify regular curricula as needed and assist special education students in regular classes with assignments.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Participate in ARD Committee meetings on a regular basis.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Conduct assessment of student learning styles and use results to plan for instructional activities.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Present subject matter according to guidelines established by IEP. Consult with classroom teachers regarding management of student behavior according to IEP.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Employ a variety of instructional techniques and media to meet the needs and capabilities of each student assigned.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Use technology in teaching/learning process.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Conduct ongoing assessments of student achievement through formal and informal testing.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Provide or supervise personal care, medical care, and feeding of students as stated in IEP.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Assume responsibility for extracurricular activities as assigned. Sponsor outside activities approved by campus principal.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Be a positive role model for students; support mission of school district.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Create classroom environment conducive to learning and appropriate for the physical, social, and emotional development of students. Manage student behavior and administer discipline. This includes intervening in crisis situations and physically restraining students as necessary according to IEP.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Consult district and outside resource people regarding education, social, medical, and personal needs of students.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Take all necessary and reasonable precautions to protect students, equipment, materials, and facilities.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Assist in selection of books, equipment, and other instructional materials.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Establish and maintain open communication by conducting conferences with parents, students, principals, and teachers. Maintain a professional relationship with colleagues, students, parents, and community members.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Participate in staff development activities to improve job-related skills.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Keep informed of and comply with federal, state, district, and school regulations and policies for special education teachers.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Compile, maintain, and file all physical and computerized reports, records, and other documents required.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Attend and participate in faculty meetings and serve on staff committees as required.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Demonstrate regular and prompt attendance to ensure a consistent focus on student learning.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Perform other duties as assigned.</span></span></li> </ul> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">  <br> <em><strong>SUPERVISORY RESPONSIBILITIES</strong></em></span></span> <ul><li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Supervise assigned teacher aide(s) and volunteer(s), student teacher(s), intern(s), beginning teacher(s) as needed.</span></span></li> </ul> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">  <br> <strong>GENERAL QUALIFICATION GUIDELINES</strong><br> <strong>Education/Certification/Experience:</strong></span></span> <ul><li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Bachelor’s degree in education or related field.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Valid Texas teaching certificate appropriate to subject and grade level assigned. Bilingual certification required for bilingual positions.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Experience in student teaching, internship, fieldwork, observation and all other placements required by universities or state approved programs for certification.</span></span></li> </ul> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">  <br> <strong>Knowledge/Skills/Abilities:</strong></span></span> <ul><li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Knowledge of special needs of students in assigned area; Admission, Review, and Dismissal (ARD) Committee process and Individual; Education Plan (IEP) goal setting process and implementation; curriculum and instruction.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Ability to present information accurately and clearly; manage multiple priorities and projects; and instruct students and manage their behavior.</span></span></li> </ul> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">  <br> <strong>Mental/Physical/Environmental Demands</strong><br> <em>The essential functions, pursuant to the Americans with Disabilities Act, may include the characteristic duties, responsibilities, knowledge, skills, and abilities noted herein; however, this is not a comprehensive listing of all functions and tasks performed by positions found in this job description.</em></span></span> <ul><li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">May be exposed to outdoor weather conditions during portions of work day.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Needs to move about inside the classroom or campus to monitor students as necessary.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Maintain composure and professionalism at all times.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Frequent standing, stooping, bending, pulling and pushing.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Frequent moving of small stacks of textbooks, media equipment, desks, and other classroom equipment.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Occasional requires lifting up to 25 pounds.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Occasional prolonged and irregular hours.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Ability to understand complex problems and to collaborate and explore alternative solutions.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Ability to organize and prioritize work schedules of others on short-term basis.</span></span></li> <li><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">Ability to make decisions which have significant impact on the immediate work unit and monitor impact outside immediate work unit.</span></span></li> </ul> <span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\">  </span></span>  <div style=\"text-align: center;\"><span style=\"font-size:14px;\"><span style=\"font-family:tahoma,geneva,sans-serif;\"><b>Equal Opportunity Employer</b></span></span></div> </span>",
      "OtherDescription": "",
      "Attachment": "",
      "WebsiteUrl": "http://www.leanderisd.org"
    }
  ]
}
```

### Attributes Descriptions
#### pagination
Attribute | Description
------------- | -------------
page | A cursor for use in pagination. Returns the n-th chunk of perPage objects.
perPage | Number of jobs per response. Must be an integer between 1 and 500 (otherwise, it will default to 100). Defaults to 100.
pageCount | Number of pages 
uniqueDistrictsCount | Number of districts that are hiring
totalNumberOfJobs | Number of unique job postings in the endpoint
#### data
Attribute | Description
------------- | -------------
JobID | Unique ID for each job
JobTitle | Job title
Location | Location as shown on the job posting. Typically states the school or building.
District | School district name
DistrictID | Unique ID for each school district
City | City the school district's main building is located in
ZipCode | Zip code the school district's main building is located in
State | State the school district's main building is located in
Url | Link to the original job posting
DatePosted | Date and time in ISO 8601 format. The time zone is UTC.
Description | Description of the job opening in HTML format
OtherDescription | Description of the job opening in HTML format. 
Attachment | Link to view or download a file attachment to the job. Typically contains the job description and/or application form. 
WebsiteUrl | Link to the school district's website

