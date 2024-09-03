# Regulation by Topic GET API

Write me a "GET" API that grab the government regulation data based on topic and publish date.
Two key value needed: 
1. topic (string)
2. publication_date (string)
The response would be array of regulation data.

The regulation data object is
1. abstract (string)
2. agencies (array of agency)
3. document_number (string)
4. excerpts (string)
5. html_url (string)
6. pdf_url (string)
7. public_inspection_pdf_url (string)
8. publication_date (string)
9. title (string)
10. type (string)

In order to get the data:
1. You need to hit this government regulation provider which is 
=> https://www.federalregister.gov/api/v1/documents/?conditions[topics]=xxxxx&format=json (GET) 
2. Pass the topic from your API into the "conditions[topics]".
3. When you are successfully getting the response, need to return only matched required publication_date. There is a parameter to search range of publication date but this test would like to see how you solve it.

Sample of topic:
1. air-pollution-control
2. agricultural-commodities
3. food-additives
4. chemicals
   
