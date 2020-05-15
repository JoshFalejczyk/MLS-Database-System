# MLS-Database-System

This was a project from Spring 2020 for my CS301 class.  It is a Java implementation of a Multi-Level Security Database, essentially a "SQL Developer"-like platform written from scratch in Java.  The database is set up by reading in three input table text files of varying contents, and the user can then work with the terminal interface to input SQL-style queries to then have results returned that follow MLS rules.  This program does not of course support every type of SQL query out there, but it does cover the essentials.  I had a bit of fun with the language of the terminal interface as well, and I think it keeps things a bit refreshing.

Functionality/Queries Supported: 
1. MLS Levels of 1-4.
2. Queries that only spans a single table (in other words, this program does not support multi-Table queries).
3. Use of the asterisk identifier in "SELECT" clauses to select all attributes from a Table.
4. A query with a "SELECT" and "FROM" clause, like "SELECT A1 FROM T1".
5. A query with a "SELECT", "FROM", and "WHERE" clause like "SELECT A1 FROM T1 WHERE A2=50".

NOTES:
1. Along with multi-Table queries not being supported, this means attribute-matching "WHERE" clauses are not supported either (like "WHERE A1=B1").
2. The input table text files are "T1.txt", "T2.txt", and "T3.txt" and can of course be modified as long as they follow the original structure/format.
3. Please follow the exact format of the example queries, as the parsing is a bit touchy.

To Run (on Bash): 
1. Compile the program using "make build".
2. Run the program using "make run".
3. Exit the program using "CTRL-D".

Credit: 
1. The concept of the project plus the Makefile was written and supplied by my course instructors, Nicholas Cioli and Dr. Susan Vrbsky.
2. NewMain.java and the classes inside it were written by myself.
