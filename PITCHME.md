## Actionable Insights To Increase Lightning Adoption 

##### <span style="font-family:Helvetica Neue; font-weight:bold">A <span style="color:#e49436">Rajasekar Elango </span>Instrumentaion Team</span>
### 

---

## Idea

> Mine instrumentation data to find actionable insights to increase lightning adoption. 

Correlate Lightning Interaction and Lightning Page View events from AILTN log lines to identify most popular users, pages, page flow patterns of Lightning Abandonment. 

---

## What did I do?

1. Imported AILTN logs from Splunk.
2. Used Apache Zeppelin (Apache Spark interactive notebook) , to correlate and aggregate interaction and page views for `switchToAloha` event.
3. Transformed Salesforce User Ids to user email address for Gus and Org62 org.

---

4. Programmatically Exported results to Wave Analytics studio.
5. Created dashboard to identify top users, exit pages and page flow pattern. 
6. Emailed users asking for feedback on why they switched.

---

## Actionable Insights As Promised

---

### Yiming Qi

Support inline editing

>I switch to classic because I want to do inline field editing on work items, as opposed to in lightning I have to click edit first then change the fields

---

### Michael Dinsmore

Cases list view reports Error "Lightning isnt' supported"

> When I go to the "cases" tool in GUS, and then to the case list view, I get an error that says that Lightning isnt' supported. 

---


|User |Action Items / Issues in Lightning |Actual Comments  |
|---  |---  |---  |
|Yiming Qi  |Support inline editing   |I switch to classic because I want to do inline field editing on work items, as opposed to in lightning I have to click edit first then change the fields. |
|Michael Dinsmore |Cases list view reports Error "Lightning isnt' supported"  |When I go to the "cases" tool in GUS, and then to the case list view, I get an error that says that Lightning isnt' supported. |
|Derek Van Dyke |Attachments (e.g. google docs) do not load when linking from within lighting |It doesn't support in-line editing of fields
Attachments (e.g. google docs) do not load when linking from within lighting
Updating tasks is cumbersome and hard to access after loading a story (that's not specific to work-manager, however)  |
|Nick Gardner |when building reports and dashboards 80% of the time the page will not load causing me to refresh or exit lightning all together | |
|Nihar Aleti  |1) No Quick Access Menu
2) Number of Buttons are limited only 10 are allowed which is a show stopper for any Person who is working on a POC
3) Not an easy Page layout link like we have in Classic | |
|Miguel Ulloa |Easier manually format emails in Chatter in Classic than in lightning. |In lightning, within the Chatter section, I have the option to send release email from there. I chose not to because I have to manually remove recipient emails from the body and paste those emails to the above fields, CC and BCC accordingly.  The recipient emails that are in the body should already be pre-populated in the associated BCC and CC fields.  I also have to manually format the body of the text to insert paragraph breaks where needed.   As a result, I find it quicker and easier to simply switch to classic and send the email from there without having to manually add recipient emails and reformat the body. |

---

## How to make this useful beyond Hackathon?

1. Turn this into a Instrumentation Spark Playground where developers can do adhoc correlation/aggregation to explore AILTN. (Just like people do with splunk queries, but spark + wave is much more efficient)

---

2. We can apply idea to correlate other log lines as well. Eg. Correlate `AILTN` and `AUGEN` using request id.

---

3. Use DVA's Spark or Gridforce infrastructure to run pre-defined aggregation continuously and push results to Wave. 


