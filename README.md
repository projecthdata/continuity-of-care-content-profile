hData Continuity of Care Content Profile
========================================

This project contains the hData Content Profile for Continuity of Care. It provides the ability to capture a patient summary in the hData Record Format. This Content Profile was created by examining the [HITSP C83](http://wiki.hitsp.org/docs/C83/C83-1.html). Entry Content Modules were modeled in XML Schema using HITSP Data Element Names for XML element names. For example, the [medication module](http://wiki.hitsp.org/docs/C83/C83-3.html#_Ref232964001) has a corresponding XML schema. Some data elements have restricted value sets, often defined in the [HITSP C80](http://www.hitsp.org/ConstructSet_Details.aspx?&PrefixAlpha=4&PrefixNumeric=80). When these value sets are small (roughly less than 50 possible values), they are defined as enumerations in the XML schemas.

Data Model
----------

This Content Profile was derived from the HITSP C83. Since the C83 is the basis for the [HITSP C32](http://www.hitsp.org/ConstructSet_Details.aspx?&PrefixAlpha=4&PrefixNumeric=32), it should be possible to create hData Records and [CDA](http://www.hl7.org/implement/standards/cda.cfm) documents that conform to the C32 that contain equivalent information. Since the data model of the HITSP C32 derives from the [HL7 CCD](http://wiki.hl7.org/index.php?title=Product_CCD) which is based on the [ASTM CCR](http://www.astm.org/Standards/E2369.htm), it should also be possible to construct equivalent CCDs (since a C32 is a CCD) and CCRs.

While the CCD and CCR standards were created with the goal of expressing a patient summary, a hData Record exposed via the RESTful API can provide a more longitudinal view of the patient. This change in usage may require changes in the data model.

License
-------

Copyright 2011 The MITRE Corporation

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.