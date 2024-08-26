

IllumeAiTest
	- Vertices
	- Patients 

- Surgical CDSS
	- Vertices


1. Select Graph URL
2. Under each vertice, see schema
3. Menus are how you can do thing with whatever it is
4. If I wanted to query Medications, select it. It brings up a table
5. If you wanted to add a verticy you can click add
6. if selected csv it has a header, it puts it in the top
7. You have to tell it it's id
8. Upload file to s3

Vertices are superset of whatever you're looking at
If it's medication names, populate verticy with id/label/medname/Name


Gremlin wants to query 

g(V).count()
Practical Gremlin
Correlate (broken)
Recommendation (broken)
Literature search
- Builds a graph off of the publically available databases

The Top two tabs can be only for the database
The rest are independent!!!!
This is great for routing!!!!


Surgical_CDSS -> ML -> define LD Graph Model Type
-> kyran, Node Classification -> Patient -> Surgery -> Vertices -> Medications (get rid of ids) -> Submit