# Comparing `tmp/compasspy-1.2.tar.gz` & `tmp/compasspy-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compasspy-1.2.tar", last modified: Mon Dec 12 01:52:01 2022, max compression
+gzip compressed data, was "compasspy-3.0.tar", last modified: Thu May  2 03:58:14 2024, max compression
```

## Comparing `compasspy-1.2.tar` & `compasspy-3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 01:52:01.895896 compasspy-1.2/
--rw-rw-rw-   0        0        0      200 2022-12-12 01:52:01.894880 compasspy-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-12 01:52:01.885564 compasspy-1.2/compasspy/
--rw-rw-rw-   0        0        0       52 2022-12-12 01:49:48.000000 compasspy-1.2/compasspy/__init__.py
--rw-rw-rw-   0        0        0     3214 2022-12-12 01:48:20.000000 compasspy-1.2/compasspy/client.py
--rw-rw-rw-   0        0        0       90 2022-12-12 01:26:30.000000 compasspy-1.2/compasspy/errors.py
--rw-rw-rw-   0        0        0     7109 2022-12-12 01:26:30.000000 compasspy-1.2/compasspy/models.py
-drwxrwxrwx   0        0        0        0 2022-12-12 01:52:01.893874 compasspy-1.2/compasspy.egg-info/
--rw-rw-rw-   0        0        0      200 2022-12-12 01:52:01.000000 compasspy-1.2/compasspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2022-12-12 01:52:01.000000 compasspy-1.2/compasspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 01:52:01.000000 compasspy-1.2/compasspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-12 01:38:34.000000 compasspy-1.2/compasspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2022-12-12 01:52:01.000000 compasspy-1.2/compasspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 01:52:01.895896 compasspy-1.2/setup.cfg
--rw-rw-rw-   0        0        0      265 2022-12-12 01:49:58.000000 compasspy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:58:14.944824 compasspy-3.0/
+-rw-rw-rw-   0        0        0      200 2024-05-02 03:58:14.943823 compasspy-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-02 03:56:46.000000 compasspy-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 03:58:14.934858 compasspy-3.0/compasspy/
+-rw-rw-rw-   0        0        0       52 2024-05-02 03:56:46.000000 compasspy-3.0/compasspy/__init__.py
+-rw-rw-rw-   0        0        0     9389 2024-05-02 03:56:46.000000 compasspy-3.0/compasspy/client.py
+-rw-rw-rw-   0        0        0      652 2024-05-02 03:56:46.000000 compasspy-3.0/compasspy/errors.py
+-rw-rw-rw-   0        0        0     8730 2024-05-02 03:56:46.000000 compasspy-3.0/compasspy/models.py
+drwxrwxrwx   0        0        0        0 2024-05-02 03:58:14.941824 compasspy-3.0/compasspy.egg-info/
+-rw-rw-rw-   0        0        0      200 2024-05-02 03:58:14.000000 compasspy-3.0/compasspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-02 03:58:14.000000 compasspy-3.0/compasspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 03:58:14.000000 compasspy-3.0/compasspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-02 03:58:14.000000 compasspy-3.0/compasspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2024-05-02 03:58:14.000000 compasspy-3.0/compasspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 03:58:14.944824 compasspy-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      303 2024-05-02 03:56:46.000000 compasspy-3.0/setup.py
```

### Comparing `compasspy-1.2/compasspy/models.py` & `compasspy-3.0/compasspy/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,195 +1,268 @@
 # Artucuno.dev
 
 from pydantic import BaseModel
-from typing import List, Optional
+from typing import List, Optional, Any
 from enum import Enum
 from .errors import *
 
+
 # The following models use data parsed from the public-ish Compass API
 
 # Note: The API that Compass has is very painful, but i have written some 'descriptions' for parts that may not make sense
 # If you know what some of the variables mean, please open an issue on Github or submit a pull request!
 
 class ExtendedStatus(BaseModel):
     __type: Optional[str]
     id: int
     uiStatus: Optional[int]
     shortName: str
-    attendanceGridDisplayMode: Optional[None] # Unsure
-    attendanceGridOrdinal: Optional[None] # Unsure
-    c: Optional[str] # Unsure (Some sort of code)
-    d: Optional[str] # Details (EG: The student is present on school grounds.)
+    attendanceGridDisplayMode: Any  # Unsure
+    attendanceGridOrdinal: Any  # Unsure
+    c: Optional[str]  # Unsure (Some sort of code)
+    d: Optional[str]  # Details (EG: The student is present on school grounds.)
     # def: bool # Unsure - Unable to add because of Python
-    eventsUi: bool # Unsure (Possibly something to do with the events page)
+    eventsUi: bool  # Unsure (Possibly something to do with the events page)
     lastModified: Optional[str]
     lastModifiedUserId: Optional[int]
-    n: Optional[str] # Another Status (EG: Present) (Possibly means name)
+    n: Optional[str]  # Another Status (EG: Present) (Possibly means name)
     note: Optional[str]
-    parentApprovalsUi: bool # Unsure
-    periodCalc_LateParentApproved: bool # If parent has submitted a late notice
+    parentApprovalsUi: bool  # Unsure
+    periodCalc_LateParentApproved: bool  # If parent has submitted a late notice
     periodCalc_LateUnapproved: bool
-    periodCalc_Present: bool # Present
-    periodCalc_NotMarked: bool # Period not marked
+    periodCalc_Present: bool  # Present
+    periodCalc_NotMarked: bool  # Period not marked
+
 
 class TimelinePeriod(BaseModel):
     """Model for a period"""
     __type: Optional[str]
     userId: int
     name: str
     onCampus: bool
     status: Optional[int]
-    statusName: Optional[str] # Timeline Status (If User attended or not)
-    teachingTime: bool # Unsure
-    attendanceOverride: bool # Unsure (Possibly to override if a user attended)
-    exportId: Optional[str] # Unsure
+    statusName: Optional[str]  # Timeline Status (If User attended or not)
+    teachingTime: bool  # Unsure
+    attendanceOverride: bool  # Unsure (Possibly to override if a user attended)
+    exportId: Optional[str]  # Unsure
     extendedStatus: Optional[ExtendedStatus]
     start: Optional[str]
     finish: Optional[str]
 
+
 class User(BaseModel):
     __type: Optional[str]
     id: int
-    sussiId: Optional[str] # Secondary ID
+    sussiId: Optional[str]  # Secondary ID
     userStatus: int
-    n: str # Fullname
-    fn: str # Firstname
-    ln: str # Lastname
+    n: str  # Fullname
+    fn: str  # Firstname
+    ln: str  # Lastname
     namePrefFirst: Optional[str]
-    namePrefLastId: Optional[str] # "Lastname, Firstname (displayCode)"
-    nif: Optional[str] # "Firstname Lastname (displayCode)"
-    ns: str # Fullname with uppercase Lastname
-    campusId: int # Campus they work in
-    baseRole: int # Role in the school
-    ce: Optional[str] # Unsure
-    displayCode: str # Teacher Display code
-    ii: str # Same as displayCode from what I can tell
-    mobileNumber: Optional[str] # No teachers have this (I think)
-    nameFirstPrefLastIdForm: str # Mix of full name and displayCode
+    namePrefLastId: Optional[str]  # "Lastname, Firstname (displayCode)"
+    nif: Optional[str]  # "Firstname Lastname (displayCode)"
+    ns: str  # Fullname with uppercase Lastname
+    campusId: Optional[int]  # Campus they work in
+    baseRole: int  # Role in the school
+    ce: Optional[str]  # Unsure
+    displayCode: str  # Teacher Display code
+    ii: str  # Same as displayCode from what I can tell
+    mobileNumber: Optional[str]  # No teachers have this (I think)
+    nameFirstPrefLastIdForm: str  # Mix of full name and displayCode
     doNotContact: bool
-    f: Optional[str] # Unsure
-    start: Optional[str] # When they started working
-    finish: Optional[str] # When they finish working / resign (?)
-    govtCode1: Optional[str] # Unsure
-    govtCode2: Optional[str] # Unsure
+    f: Optional[str]  # Unsure
+    start: Optional[str]  # When they started working
+    finish: Optional[str]  # When they finish working / resign (?)
+    govtCode1: Optional[str]  # Unsure
+    govtCode2: Optional[str]  # Unsure
     hasRegisteredDevice: bool
 
+    @property
+    def name(self):
+        return self.n
+
+    @property
+    def firstname(self):
+        return self.fn
+
+    @property
+    def lastname(self):
+        return self.ln
+
+
+class UserBasic(BaseModel):
+    __type: Optional[str]
+    id: int
+    ii: Optional[str]
+    n: Optional[str]
+    nameFirstPrefLastIdForm: Optional[str]
+    namePrefLastId: Optional[str]
+    p: Optional[str]
+    pv: Optional[str]
+    lastName: Optional[str]
+    checkInMarkingMode: int
+    compassPersonId: Optional[str]
+    displayCode: Optional[str]
+    f: Optional[str]
+    isPrimaryAccountHolder: bool
+    userStatus: Optional[int]
+    y: Optional[int]
+
+
 class UserDetailsBlob(BaseModel):
     __type: Optional[str]
-    userId: int # Internal Student ID
+    userId: int  # Internal Student ID
     chroniclePinnedCount: Optional[int]
-    userDisplayCode: str # Student ID
-    userSussiID: Optional[str] # Secondary Student ID
-    userDetails: str # Time since Date of Birth
+    userDisplayCode: str  # Student ID
+    userSussiID: Optional[str]  # Secondary Student ID
+    userDetails: Optional[str]  # Time since Date of Birth
     userEmail: str
     userFirstName: str
     userLastName: str
-    userYearLevel: str # Year Level String
-    userYearLevelId: int # Year Level Number
+    userYearLevel: Optional[str]  # Year Level String
+    userYearLevelId: Optional[int]  # Year Level Number
     userPreferredName: Optional[str]
     userPreferredLastName: Optional[str]
     userFullName: str
-    userRole: int # Unsure yet (Possibly to tell between staff / student)
-    userStatus: int # Unsure yet (Possibly to show if student is at school)
-    userPhotoPath: Optional[str] # Location of user profile picture
-    userSquarePhotoPath: Optional[str] # Square Photo
-    userHouse: Optional[str] # User House Group
-    userGenderPronouns: Optional[str] # Not implemented at my school
-    userFormGroup: str # Year / House
+    userRole: int  # Unsure yet (Possibly to tell between staff / student)
+    userStatus: int  # Unsure yet (Possibly to show if student is at school)
+    userPhotoPath: Optional[str]  # Location of user profile picture
+    userSquarePhotoPath: Optional[str]  # Square Photo
+    userHouse: Optional[str]  # User House Group
+    userGenderPronouns: Optional[str]  # Not implemented at my school
+    userFormGroup: Optional[str]  # Year / House
     userSchoolURL: Optional[str]
     userSchoolId: Optional[str]
     userTimeLinePeriods: List[TimelinePeriod]
 
+
 class StandardClass(BaseModel):
     __type: Optional[str]
     id: int
-    subjectId: int # Different to id
+    subjectId: int  # Different to id
     name: str
     subjectLongName: str
     facultyName: Optional[str]
     description: Optional[str]
     importIdentifier: Optional[str]
     subjectImportIdentifier: Optional[str]
-    importTeachers: bool # Unsure
-    layerAllowsImport: bool # Unsure
-    layerId: int # Unsure
+    importTeachers: bool  # Unsure
+    layerAllowsImport: bool  # Unsure
+    layerId: int  # Unsure
     locationId: Optional[int]
-    managerId: int # Possibly Teacher ID
-    managerImportIdentifier: str # Manager identifier
-    attendanceModeDefault: int # Unsure
+    managerId: int  # Possibly Teacher ID
+    managerImportIdentifier: str  # Manager identifier
+    attendanceModeDefault: int  # Unsure
     campusId: Optional[int]
-    checkInEnabledDefault: int # Unsure
-    customLocation: Optional[str] # Unsure
-    extendedStatusId: int # Unsure
-    start: Optional[str] # Date the subject starts
-    finish: Optional[str] # Date the subject finishes
-    haparaSyncEnabled: bool # Unsure
+    checkInEnabledDefault: int  # Unsure
+    customLocation: Optional[str]  # Unsure
+    extendedStatusId: int  # Unsure
+    start: Optional[str]  # Date the subject starts
+    finish: Optional[str]  # Date the subject finishes
+    haparaSyncEnabled: bool  # Unsure
     yearLevelShortName: Optional[str]
 
+
 class DataExtGridDataContainer(BaseModel):
     __type: Optional[str]
     data: List[StandardClass]
     total: int
 
+
 class Location(BaseModel):
     __type: Optional[str]
     id: int
     roomName: str
-    n: Optional[str] # Same as roomName
+    n: Optional[str]  # Same as roomName
     longName: str
     building: Optional[str]
     archived: bool
 
+
 class AlertItem(BaseModel):
     __type: Optional[str]
-    Type: int # Unsure
+    Type: int  # Unsure
     AlertItemId: int
-    Body: Optional[str] # Alert Item Body (HTML)
+    Body: Optional[str]  # Alert Item Body (HTML)
     Dismissible: bool
     ImageSourceUrl: Optional[str]
     IsWarning: bool
     LinkText: Optional[str]
     LinkUrl: Optional[str]
     Title: Optional[str]
 
+
 class TaskCategory(BaseModel):
     __type: Optional[str]
     categoryId: int
-    categoryName: Optional[str] # Name (EG: Homework, Assignment, etc)
-    categoryColour: Optional[str] # Hex code
+    categoryName: Optional[str]  # Name (EG: Homework, Assignment, etc)
+    categoryColour: Optional[str]  # Hex code
+
 
 class CalendarTransport(BaseModel):
     __type: Optional[str]
     activityId: int
     activityType: int
     instanceId: Optional[str]
     topTitleLine: Optional[str]
     bottomTitleLine: Optional[str]
     topAndBottomLine: Optional[str]
     allDay: bool
     start: Optional[str]
     finish: Optional[str]
     rollMarked: bool
     runningStatus: int
-    attendanceMode: int # Unsure
-    backgroundColor: str # Unsure
+    attendanceMode: int  # Unsure
+    backgroundColor: str  # Unsure
+
 
 class GenericMobileResponse(BaseModel):
     __type: Optional[str]
     data: List[CalendarTransport]
 
-def getType(tp: str): # Converts __type to a class model
+
+class Task(BaseModel):
+    __type: Optional[str]
+    id: int
+    taskName: Optional[str]
+    status: bool
+    dueDate: Optional[str]
+
+
+class Account(BaseModel):
+    __type: Optional[str]
+    userId: int
+    firstName: str
+    lastName: str
+    name: str
+    accountId: Optional[str]
+    compassPersonId: Optional[str]
+    yearLevelId: Optional[int]
+    username: Optional[str]
+    userStatus: Optional[int]
+    schoolId: Optional[str]
+    paymentMethods: Optional[list]
+    isWalletEnabled: bool
+    balance: Optional[int]
+    imageUrl: Optional[str]
+    freeMeals: Any
+
+
+def getType(tp: str):  # Converts __type to a class model
     p = {
-    "UserDetailsBlob": UserDetailsBlob,
-    "User:http://jdlf.com.au/ns/data/users": User,
-    "TimelinePeriod:http://jdlf.com.au/ns/data/attendance/v2": TimelinePeriod,
-    "Es:http://jdlf.com.au/ns/business/attendance/transport": ExtendedStatus,
-    "DataExtGridDataContainer:http://jdlf.com.au/ns/business/transport": DataExtGridDataContainer,
-    "StandardClass:http://jdlf.com.au/ns/business/curriculum": StandardClass,
-    "LC": Location,
-    "AlertItem:http://jdlf.com.au/ns/data/newsfeed": AlertItem,
-    "GenericMobileResponse:http://jdlf.com.au/ns/data/mobile/": GenericMobileResponse,
-    "CalendarTransport:http://jdlf.com.au/ns/data/mobile": CalendarTransport
+        "UserDetailsBlob": UserDetailsBlob,
+        "User:http://jdlf.com.au/ns/data/users": User,
+        "UserBasic:http://jdlf.com.au/ns/data/users": UserBasic,
+        "TimelinePeriod:http://jdlf.com.au/ns/data/attendance/v2": TimelinePeriod,
+        "Es:http://jdlf.com.au/ns/business/attendance/transport": ExtendedStatus,
+        "DataExtGridDataContainer:http://jdlf.com.au/ns/business/transport": DataExtGridDataContainer,
+        "StandardClass:http://jdlf.com.au/ns/business/curriculum": StandardClass,
+        "LC": Location,
+        "AlertItem:http://jdlf.com.au/ns/data/newsfeed": AlertItem,
+        "GenericMobileResponse:http://jdlf.com.au/ns/data/mobile/": GenericMobileResponse,
+        "CalendarTransport:http://jdlf.com.au/ns/data/mobile": CalendarTransport,
+        "Task:http://jdlf.com.au/ns/data/tasks": Task,
+        "Account:http://jdlf.com.au/ns/data/accounts": Account
     }
     if tp in p:
         return p[tp]
     raise UnknownType(f"{tp}")
```

