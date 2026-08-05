> This is based on the document Shane has presented me with.

1. Load graph into a graph database
2. Explore vertices, edges, and properties in the database
	1. Connections hard coded based on user ID
	2. Create Vertex / Edge or add to Vertex / Edge
		1. Select a CSV file with Headers to create Vertexes
			1. Modifyable Header / Delimiter / Encoding / Comment character
			2. Ability to change the names of the property values after loading the csv
			3. Ability to change the data type
		2. Select a unique name for vertex
		3. Select a column that has unique id's, as it's necessary
	3. Vertices are data, edges are connectionss, and ML Endpoints are the ML models creating using the vertices and edges. Properties associated with vertexes and edges can be viewed. Each property can be used as features in the graph neural network
	4. Can display the count of Vertexes or Edges with the specified labels
	5. Can perform 'sample queries'
	6. Can view properties of vertexes or edges
	7. Can delete vertex / edges
	8. Can filter on Vertex / Edges labels
3. Cohort query visual representation. If the edges connect Subjects to other vertex label types, Subjects should be selected
	1. Results is a force directed graph
4. Creating machine learning graph neural network models from the graph (automated)
	1. Can view already created Graph Neural Network endpoints
		1. Can view properties of export / processing / training / endpoint creation steps
	2. Can modify / delete ML Endpoints
		1. Can create a confusion matrix of the modle and see all the individual predictions of the training and validation datasets
		2. Can transofrm the modle with the same features
		3. Can delete ML endpoints
	3. Might be able to filter on vertex / edge label properties too
	4. Can create ML Endpoint
		1. Unique name
			1. Node Classification / Node Regression / Edge Classification / Edge Regression / Link Prediction
			2. Choose Vertexes or Edges
			3. Choose properties or edges
			4. Choose Features
			5. For each Vertex and edge label, select properties to use as predictive features
		2. Shows Progress Bar with DGL Export / Processing / Training / Creating ML Endpoint
			1. Pending / Running / Success or Fail
5. Misc
	1. User Authentication
	2. Operator dropdown (numeric / date / text)?? It's the header search thing
		1. So basically a filter function

> Planned / nice to have

1. User management (editing via API / frontend)
2. Database connection authentication via configurable databas
