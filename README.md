# SW-project
Semantic web project of 2024-01-10

#Text:

Instructions for the submission of the solution
The candidate has to submit two files: (i) one file containing the ontology in Turtle format, with extension
.ttl or .owl; (ii) one file in PDF format, containing the answers to each question starting from Q8. The
solution must be submitted via the Moodle of the course no later than the 11th of January at 8 PM Italian
time. Any file received after that time will not be considered valid for the exam.
Exercise
The fundamental concepts in an application domain related to Medieval and Renaissance manuscripts are: title,
author, date of creation and library. In this domain, we intend a manuscript as the conceptual and immaterial
outcome of an intellectual or creative process (and not a physical object). Some of the facts that characterize
this domain can be stated as follows:
1. Each manuscript has exactly one title (a string) and an author. The manuscript can be a Medieval
manuscript or a Renaissance manuscript.
2. A manuscript is identified by an ID (a string).
3. The manuscript belongs to at least one literary genre.
4. A manuscript has a date of creation.
5. A manuscript is collected in exactly one library. The library can be public or private. The library is
located in exactly one place.
6. A manuscript is included in at least one modern book.
7. The book has a title (a string) and is identified by an ISBN code (a string).
8. A book has exactly one publisher. The publisher is identified by a name (a string) and an ID (a
positive integer).
9. The publisher has a publication agreement with the library in which the manuscript is collected.
10. A publisher publishes more than one book.
11. A book has a price (a positive integer).
12. The publisher sells the books through more than one bookshop.
13. Manuscript, book, author, library, place, literary genre, publisher, and bookshop are pairwise
disjoint concepts.
The candidate should express all the above statements in an OWL 2 DL ontology, using the RDF Turtle
notation. In particular, the ontology must:
Q1. Declare the required classes, providing for each class a textual label and a concise textual description of
the intension of the class, using the appropriate annotation properties from the RDF Schema vocabulary.
Q2. Provide the sub-class axioms defining the class taxonomy.
Q3. Declare the required object properties, providing for each property:
Q.1. a textual label, using the appropriate annotation property from the RDFS vocabulary
Q3.2. a textual description of the intension of the property, using the appropriate annotation property
from the RDFS vocabulary
Q3.3. one axiom defining the domain of the property
Q3.4. one axiom defining the range of the property
Q3.5. one axiom defining the inverse of the property
Q3.6. any additional axioms expressing disjointness of the property with other object properties, and
the property characteristics.
Q4. Provide the sub-property axioms defining the object property taxonomy.
Q5. Declare the required data properties, providing:
Q5.1. a textual label, using the appropriate annotation property from the RDFS vocabulary
Q5.2. a textual description of the intension of the property, using the appropriate annotation property
from the RDFS vocabulary
Q5.3. one axiom defining the domain of the property
Q5.4. one axiom defining the range of the property
Q5.5. any additional axioms expressing disjointness of the property with other data properties, and
whether the property is functional.
Q6. Define the axioms necessary for expressing any statement in 1 to 13 that has not already been 
expressed.
Q7. Populate the ontology with at least one individual for each class, and at least one assertion for each
property.
In addition, the candidate must:
Q8. Identify two different assertions that would make the ontology inconsistent.
Q9. Define the complex role inclusion axiom capturing the fact that if a publisher publishes a book that
includes a manuscript that is collected in a library, then the publisher has a publication agreement
with that library.
Q10. Verify if the created ontology (including the complex role inclusion axiom defined in Q9) satisfies
the global restrictions on the axioms of an OWL 2 DL ontology.
Q11. Write the following queries in SPARQL:
Q11.1. Find the manuscripts created between 1130 and 1250 and for each manuscript the library in
 which it is collected.
Q11.2. Among all books ordered by title alphabetically, find the title of three books starting from the
 second result.
 Q11.3. For each book, find the manuscripts that are published in it, the titles of these manuscripts, and
 the title, ISBN code and the publisher of the book.
 Q11.4. Find the price of each book calculating a discount of 20%.
 Q11.5. Find the title and the author of each manuscript that is not a Renaissance manuscript.
 Q11.6. Retrieve the maximum price of the books grouped by publisher. 
