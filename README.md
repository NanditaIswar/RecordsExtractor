# RecordsExtractor

Technology used here is SpringBoot with Maven,Java8
A REST API(/extractRecords) is exposed as GET operation. The input parameter has to be given as RequestParam which needs to have the full path of the required file. 
For example, the endpoint with inputParam will be http://your hostname: port no/extractRecords?inputFile=name of the required file with extension with fullpath
Junit tests are covered individually for Controller,Service and Utility classes.
Code coverage when tested comes to around 70%(Screenshot attached in mail)
The REST API was tested with SOAPUI for different combination of inputs and the screenshots of the output are attached in mail for reference.
The output gives the list of transcationRefNum and description of records whose refrenceNumber are duplicate and whose endBalance are invalid(Failed Records).

Note: The lombok jar has been included to reduce the boilerplate code and the dependency for same has been added in the pom.xml. 
If any issues faced in accessing it, please make sure the jar from .m2 repository is copied into the IDE location and the same has been integrated with IDE to resolve it.
