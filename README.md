[http://www.virtualflybrain.org Virtual Fly Brain] is a hub for integration of Drosophila neuro-anatomical data.  The glue that binds all this data into a query-able whole is an anatomy ontology in the W3C language [OWL2](http://www.w3.org/TR/owl2-primer/). This project uses Webulous (a new, Google spreadsheets-based version of (Populous)[http://www.e-lico.eu/populous.html]) to generate standard collections of spreadsheet templates for annotating with this ontology.  A file of pre-rolled OWL query classes defines the content of spreadsheet columns.  Users can annotate simply by browsing VFB and then copying and pasting term names into the appropriate columns.  Adding a term not defined as legal for the column provokes a warning.  All legal terms are automatically linked to the ID (URI) for the term.

We envisage two different ways to use this annotation: 

(i) Users can dump the content of simple spreadsheets into a SQL database.  Starting from any anatomy term that can be found on VFB, they can then use a simple web service to find all for relevant anatomy (e.g. all substructures and overlapping neurons for a brain region) to pipe into a query of their database. 

(ii)  A set of [http://oppl2.sourceforge.net/ OPPL2] files defines conversion of these spreadsheets into OWL.  The resulting OWL files can be loaded, along with the Drosophila anatomy ontology, into [http://protege.stanford.edu/ Protege 4] within which they can be directly queried and browsed.  We intend that future versions of VFB will allow users to upload their own files OWL files to allow integrated queries of their own data in the context of VFB. 
