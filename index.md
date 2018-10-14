## Welcome to GitHub Pages

##appendix
\textbf{Four queries of DBpedia}\\
Q1: SELECT	?s1	?s2	?s3	?s4	?s5	?s6	where \{ \\
	?s2	<http://www.w3.org/1999/02/22-rdf-syntax-ns\#type>	?s1	.\\
	?s3	<http://www.w3.org/1999/02/22-rdf-syntax-ns\#type>	?s5	.\\
	?s4	<http://www.w3.org/1999/02/22-rdf-syntax-ns\#type>	?s6	.\\
	?s2	<http://dbpedia.org/ontology/careerStation>	?s3	.\\
	?s2	<http://dbpedia.org/ontology/managerClub>	?s4	.\\
	?s3	<http://dbpedia.org/ontology/team>	?s4	.
\} \\
Q2: SELECT	?s1	?o1	?o2	?o3	
where	\{ \\
	?s1	<http://www.w3.org/1999/02/22-rdf-syntax-ns\#type>	?o1	.\\
	?s1	<http://dbpedia.org/ontology/team>	?o2	.\\
	?o3	<http://dbpedia.org/property/publisher>	?o2	.
\} \\
Q3: SELECT	?s1	?o1	?o2	
where	\{ \\
	?s1	<http://dbpedia.org/ontology/team>	?o1	.\\
	?s1	<http://www.w3.org/1999/02/22-rdf-syntax-ns\#type>	?o2	.
\} \\
Q4: SELECT	?s1	?o1	?o2	
where	\{ \\
	?s1	<http://www.w3.org/2000/01/rdf-schema\#seeAlso>	?o1	.\\
	?s1	<http://dbpedia.org/ontology/successor>	?o2	.
\} 

\textbf{Seven queries of YAGO}\\
Q1: select	?s1	?s2	?s3	?o1	?o2	?o3 where \{ \\
	?s1	<type>	?o1	.\\
	?s2	<type>	?o2	.\\
	?s3	<type>	?o3	.\\
	?s1	<graduatedFrom>	?s2	.\\
	?s1	<livesIn>	?s3	.\\
	?s2	<isLocatedIn>	?s3	.
\}\\
Q2: select	?s1	?s2	?s3	?o1	?o2	?o3
where	
\{\\
	?s1	<type>	?o1	.\\
	?s2	<type>	?o2	.\\
	?s3	<type>	?o3	.\\
	?s1	<wasBornIn>	?s2	.\\
	?s1	<isCitizenOf>	?s3	.\\
	?s2	<isLocatedIn>	?s3	.
\}\\
Q3: select	?s1	?o1	?o2	?o3	?o4	?o5	?o6	?o7	?o8	
where	
\{\\
	?s1	<diedIn>	?o1	.\\
	?s1	<created>	?o2	.\\
	?s1	<hasGender>	?o3	.\\
	?s1	<type>	?o4	.\\
	?s1	<actedIn>	?o5	.\\
	?o1	<wasCreatedOnDate>	?o6	.\\
	?o1	<hasWebsite>	?o7	.\\
	?o1	<isLocatedIn>	?o8	.
\}\\
Q4: select	?s1	?o1	?o2	?o3 ?o4
where	
\{\\
	?s1	<actedIn>	?o1	.\\
	?s1	<hasChild>	?o4	.\\
	?s1	<hasWikipediaAnchorText>	?o2	.\\
	?o3	<hasCitationTitle>	?o2	.
\}\\
Q5: select	?s1	?o2	?o3	?o4	?o5
where	
\{\\
	?s1	<created>	?o2	.\\
	?o2	<isLocatedIn>	?o3	.\\
	?o3	<hasOfficialLanguage>	?o4	.\\
	?o4	<hasWikipediaAnchorText>	?o5	.
\}\\
Q6: select	?s1	?o1	?o3	?o4	?o5	?o6	?o8
where	
\{\\
	?s1	<hasGender>	?o1	.\\
	?s1	<wasBornOnDate>	?o3	.\\
	?s1	<hasCitationTitle>	?o4	.\\
	?s1	<diedOnDate>	?o5	.\\
	?s1	<wasBornIn>	?o6	.\\
	?s1	<type>	?o8	.
\}\\
Q7: select	?s1	?o1	?o2	?o4	?o6	?o8
where	
\{\\
	?s1	<hasGender>	?o1	.\\
	?s1	<diedIn>	?o2	.\\
	?s1	<hasWikipediaAnchorText>	?o4	.\\
	?s1	<wasBornIn>	?o6	.\\
	?s1	<type>	?o8	.
\}\\
