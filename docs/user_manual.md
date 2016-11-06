# Introduction
# Incident Posture
# Custom Search Commands

### loadincidentresults 
**Usage**: ```<your search> | table _time incident_id | loadincidentresults incident_id``

**Parameters:**

* `incident_id`: ID of the incident per search result (Required)

Returns results of incidents from the KV store given a list of incidents having an `incident_id` field present.

### modifyincidents 

**Usage**:
```<your search> | table _time incident_id | modifyincidents status=<new status> owner=<new owner> urgency=<new urgency> comment=<comment>``

**Parameters:**

* `status`: New status of the incident(s) (Optional)
* `status`: New owner of the incident(s) (Optional)
* `urgency`: New urgency of the incident(s) (Optional)
* `comment`: Text of the comment to add to the change event (Optional)

Updates incident attributes such as status, owner, urgency and adds a comment, if provided. Requires the field `incident_id` in the search results. Use any attribute in combination or by oneself. 

# Reports
# Datamodel
# Troubleshooting