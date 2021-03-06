As of Oct. 19\ :sup:`th`, 2015

1) Files under
ftp://ftp.hdfgroup.uiuc.edu/pub/outgoing/HDFCompass/kent-files/

A) Directory /hdf5-handler-fake

+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Files                        | Issues-view                                                                            | Issues -plot                                |
+==============================+========================================================================================+=============================================+
| Comp\_complex.h5             | 1. Datatype cmp1 treats an HDF5 Attributes                                             | Two lines are plotted, which                |
|                              |                                                                                        |                                             |
|                              | 2. No information about compound datatype cmp1, cmp2                                   | doesn’t make sense                          |
|                              |                                                                                        |                                             |
|                              | 3. Attribute of phony\_compound\_var                                                   |                                             |
|                              |                                                                                        |                                             |
|                              | DIMENSION\_LIST Value doesn’t make sense.                                              |                                             |
|                              |                                                                                        |                                             |
|                              | 4. The value of phony\_compound\_var                                                   |                                             |
|                              |                                                                                        |                                             |
|                              | Is not right                                                                           |                                             |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| comp\_scalar.h5              | All right                                                                              | No plot                                     |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| comp\_complex\_scalar.h5     | Only display the first element of the member                                           | No plot                                     |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Compound\_more\_types.h5     | No data is displayed                                                                   | Crash the compass when clicking plot data   |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_compound.h5               | OK                                                                                     | No plot                                     |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_dset\_many.h5             | OK and fast                                                                            | OK                                          |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_link\_hard.h5             | https://github.com/HDFGroup/hdf-compass/issues/90                                      | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_link\_soft.h5             | https://github.com/HDFGroup/hdf-compass/issues/91                                      | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_objref.h5                 | https://github.com/HDFGroup/hdf-compass/issues/92                                      | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| D\_regref.h5                 | https://github.com/HDFGroup/hdf-compass/issues/93                                      | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Grid\_1\_2d.h5               | Ok but the display of HDF5 string dataset is all in one.                               | OK                                          |
|                              |                                                                                        |                                             |
|                              | https://github.com/HDFGroup/hdf-compass/issues/94                                      |                                             |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Grid\_1\_3d\_xyz\_aug.h5     | Object reference issues discovered by others                                           | OK                                          |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Nc4\_group\_atomic.h5        | Object reference issues discovered by others                                           | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Nc4\_group\_comp.h5          | Wait                                                                                   | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Nest\_comp\_scalar.h5        | Wait                                                                                   | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| Ntypes.h5                    | See issues 95-99                                                                       | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| t\_flatten\_name\_clash.h5   | OK                                                                                     | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| t\_link\_comment.h5          | Comment doesn’t show up, no need to report this since comment is deprecated in HDF5.   | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| T\_vl\_string\_cstr.h5       | Covered                                                                                | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| T\_space\_null.h5            | OK                                                                                     | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+
| T\_space\_zero.h5            | OK                                                                                     | N/A                                         |
+------------------------------+----------------------------------------------------------------------------------------+---------------------------------------------+

B) Directory /hdf5-testing-files

+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| Files                                                                                                         | Issues-view                                                                        | Issues -plot   |
+===============================================================================================================+====================================================================================+================+
| Charsets.h5                                                                                                   | ok                                                                                 |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| tldoublebad.h5                                                                                                | Cannot open by h5dump, the file may be corrupted tldouble.h5 is under /testfiles   |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| tldouble.h5                                                                                                   | Cannot open the file                                                               |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| tbigdims.h5                                                                                                   | Crash the testing machine                                                          |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| tfilters.h5                                                                                                   | OK                                                                                 |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+
| This may wrap up the testing for all the fake files.                                                          |                                                                                    |                |
|                                                                                                               |                                                                                    |                |
| STOP testing and wait for the lead to review the testing plan and provide the guidelines for the next step.   |                                                                                    |                |
+---------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------------+----------------+

C) Directory /hdf5-real-files
