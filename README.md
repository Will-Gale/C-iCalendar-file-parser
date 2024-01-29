# C-iCalendar-file-parser



# /*missing CalendarParser.c file is available upon request for future employers*/



The iCal File Parser is a robust C-based application designed to parse, manipulate, and generate .ics (iCalendar) files. It emphasizes not only functionality but also memory safety and efficiency, ensuring proper memory allocation, deallocation, and leak prevention using tools such as Valgrind. It effectively handles the complexities of the iCalendar format by providing a robust set of functionalities that include parsing iCalendar files into structured data, validating the integrity of the data against the iCalendar specification, and writing the structured data back into compliant .ics files.



Modules

The project is divided into two primary modules:

1. LinkedListAPI
   
   - Handles all operations related to the doubly linked list data structure, offering functionalities for node creation, insertion, deletion, and utility operations.

2. CalendarParser

   - Manages parsing, validating, and writing iCalendar files. It operates on structured data representing iCalendar components like events, alarms, and properties.

Data Structures

1. Linked List (LinkedListAPI)
   
   - Node: A structure representing a node in a doubly linked list.

   - List: A structure representing the list metadata, containing pointers to the head and tail nodes, the length of the list, and function pointers for operations on list data.

   - ListIterator: A structure for iterating through the list.

2. iCalendar Components (CalendarParser)
   
   - DateTime: Represents date-time information in the iCalendar format.

   - Property: Represents a generic iCalendar property.

   - Alarm: Represents an alarm component within an iCalendar event.

   - Event: Represents an iCalendar event component, containing a UID, creation date-time, start date-time, properties, and alarms.

   - Calendar: Represents an iCalendar object, encapsulating the iCalendar version, product ID, events, and additional properties.

Core Functionalities

3. LinkedListAPI
   
   - Node and List Initialization: Functions for initializing nodes and the list.

   - Insertion and Deletion: Functions for inserting nodes at the front, back, or sorted order, and for deleting nodes.

   - Utility Functions: Functions for getting nodes from the front or back, converting the list to a string, and other list-related operations.

5. CalendarParser
   
   - createCalendar: Parses an iCalendar file and creates a Calendar object.

   - deleteCalendar: Frees all memory associated with a Calendar object.
   
   - printCalendar: Generates a human-readable string representing the content of a Calendar object.
   
   - printError: Converts an error code into a human-readable string.

   - writeCalendar: Writes a Calendar object into a file in iCalendar format.

   - validateCalendar: Validates a Calendar object according to the iCalendar standard.

Utility Functions

   - Functions for managing and comparing Event, Alarm, Property, and DateTime objects, including memory management and string representation functions.

JSON Conversion Functions

   - Functions for converting DateTime, Event, Calendar, and their lists to and from JSON strings, and for adding events to an existing Calendar object.

File Structure

   - LinkedListAPI.h/c: Contains definitions and implementations of the linked list functionalities.

   - CalendarParser.h/c: Contains definitions and implementations of the iCalendar parsing, validation, and writing functionalities.

Usage

   - Parsing: Use createCalendar to parse .ics files into Calendar objects.
   
   - Manipulating: Utilize the LinkedListAPI and CalendarParser functions to manipulate calendar data.
   
   - Validating: Use validateCalendar to ensure the calendar data meets the iCalendar specifications.
   
   - Writing: Use writeCalendar to write the Calendar object back into an .ics file.
   
   - Converting: Use JSON conversion functions for web or network-based applications.











