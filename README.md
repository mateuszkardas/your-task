## Code challenge

1. Design data structures to support the following domain:
    - a model of a car (e.g. VW Golf v5), which is represented by the brand (one of BMW, VW or Audi), the model name and the version (which is numerical  and always starts from 1);
    - a car, which is represented by the car model (e.g. VW Golf v5), the manufacturing year (e.g. 2001) and the engine serial number (e.g. "11A-12345");
    - a known defect, which is represented by the car model, the affected years of issue (e.g. 2001, 2002, 2003) and the defect code (e.g. "345F");


2. Add support for the following operations on the car model:
    - get a user-friendly text representation (for UI);
    - get a developer-friendly text representation (for logs);
    - increment the version;


3. Implement a method that accepts a list of cars and returns defects known to be present in them, given that there is a remote service that can be queried for defects of the provided car models;

    Here is how the actual data may look like:

    - First car, VW Golf v5, manufactured in 2003 with engine SN "11A-12345"
    - Second car, VW Golf v5, manufactured in 2008 with engine SN "88Z-88888"
    - A known defect affects all VW Golf v5 manufactured between 2003 and 2005. Thus, it affects the first car, but does not affect the second car, even though they share the same car model (VW     Golf v5);