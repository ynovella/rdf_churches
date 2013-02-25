rdf_churches
============

Converting the USA megachurches data to RDF.
The original data can be found at http://hirr.hartsem.edu/megachurch/database.html
It is scraped and then converted using python.

to run the conversion script in the same folder as the churches-2.txt file type:
$ python schema.py

to run jena eyeball tool, put all jars on the java classpath and run it from the comman line:
$ java jena.eyeball -assume owl myshema.owl -check triples.xml
where triples.xml is the turtle data converted in xml format by http://www.rdfabout.com/demo/validator/
and mychema.owl is in the eyeball folder along with it
