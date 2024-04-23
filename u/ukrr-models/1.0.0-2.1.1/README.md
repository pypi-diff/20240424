# Comparing `tmp/ukrr_models-1.0.0.tar.gz` & `tmp/ukrr_models-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukrr_models-1.0.0.tar", max compression
+gzip compressed data, was "ukrr_models-2.1.1.tar", max compression
```

## Comparing `ukrr_models-1.0.0.tar` & `ukrr_models-2.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1099 2024-03-25 15:29:47.225126 ukrr_models-1.0.0/LICENSE
--rw-r--r--   0        0        0      707 2024-03-25 20:53:07.558975 ukrr_models-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1268 2024-03-25 20:26:41.125198 ukrr_models-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-11-06 15:09:35.217401 ukrr_models-1.0.0/ukrr_models/__init__.py
--rw-r--r--   0        0        0     1730 2024-03-25 15:29:47.274299 ukrr_models-1.0.0/ukrr_models/nhsbt_models.py
--rw-r--r--   0        0        0     2466 2024-03-25 15:29:47.281108 ukrr_models-1.0.0/ukrr_models/rr_models.py
--rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 ukrr_models-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1291 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/README.md
+-rw-r--r--   0        0        0      637 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/__init__.py
+-rw-r--r--   0        0        0     1680 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/nhsbt_models.py
+-rw-r--r--   0        0        0     2386 2024-04-23 23:12:21.036731 ukrr_models-2.1.1/ukrr_models/rr_models.py
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 ukrr_models-2.1.1/PKG-INFO
```

### Comparing `ukrr_models-1.0.0/README.md` & `ukrr_models-2.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-<a name="readme-top"></a>
-
-<div align='center'>
-
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-
-</div>
-<br />
-<h1 align="center">UKRR Models</h1>
-
-## About The Project
-
-A limited set of database models for the RR database
-<br/>
-
-## Usage
-
-```
-poetry add ukrr_models
-```
-
-## Built With
-
-[![SQLAlchemy][SQLAlchemy]][SQLAlchemy-url]
-
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-## Contact
-
-Renal Registry - [@UKKidney](https://twitter.com/@UKKidney) - rrsystems@renalregistry.nhs.uk
-
-Project Link: [https://github.com/renalreg/ukrr_models](https://github.com/renalreg/rr-connection-manager)
-
-<br />
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-[issues-shield]: https://img.shields.io/github/issues/renalreg/ukrr_models.svg?style=for-the-badge
-[issues-url]: https://github.com/renalreg/ukrr_models/issues
-[license-shield]: https://img.shields.io/github/license/renalreg/ukrr_models.svg?style=for-the-badge
-[license-url]: https://github.com/renalreg/ukrr_models/blob/master/LICENSE
-[SQLAlchemy]: https://img.shields.io/badge/sqlalchemy-V1.4-D71F00?style=for-the-badge&logoColor=white
-[SQLAlchemy-url]: https://www.sqlalchemy.org/
+<a name="readme-top"></a>
+
+<div align='center'>
+
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+
+</div>
+<br />
+<h1 align="center">UKRR Models</h1>
+
+## About The Project
+
+A limited set of database models for the RR database
+<br/>
+
+## Usage
+
+```
+poetry add ukrr_models
+```
+
+## Built With
+
+[![SQLAlchemy][SQLAlchemy]][SQLAlchemy-url]
+
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Renal Registry 
+* Website - [The UK Kidney Association](https://ukkidney.org/)
+* X - [@UKKidney](https://twitter.com/@UKKidney)
+* E-mail -  rrsystems@renalregistry.nhs.uk
+
+Project Link - [https://github.com/renalreg/ukrr_models](https://github.com/renalreg/ukrr_models)
+
+<br />
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+[issues-shield]: https://img.shields.io/github/issues/renalreg/ukrr_models.svg?style=for-the-badge
+[issues-url]: https://github.com/renalreg/ukrr_models/issues
+[license-shield]: https://img.shields.io/github/license/renalreg/ukrr_models.svg?style=for-the-badge
+[license-url]: https://github.com/renalreg/ukrr_models/blob/master/LICENSE
+[SQLAlchemy]: https://img.shields.io/badge/sqlalchemy-V1.4-D71F00?style=for-the-badge&logoColor=white
+[SQLAlchemy-url]: https://www.sqlalchemy.org/
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
     [![Issues][issues-shield]][issues-url] [![MIT License][license-shield]]
                                  [license-url]
 
                            ************ UUKKRRRR MMooddeellss ************
 ## About The Project A limited set of database models for the RR database
 ## Usage ``` poetry add ukrr_models ``` ## Built With [![SQLAlchemy]
 [SQLAlchemy]][SQLAlchemy-url] ## License Distributed under the MIT License. See
-`LICENSE` for more information. ## Contact Renal Registry - [@UKKidney](https:/
-/twitter.com/@UKKidney) - rrsystems@renalregistry.nhs.uk Project Link: [https:/
-/github.com/renalreg/ukrr_models](https://github.com/renalreg/rr-connection-
-manager)
+`LICENSE` for more information. ## Contact Renal Registry * Website - [The UK
+Kidney Association](https://ukkidney.org/) * X - [@UKKidney](https://
+twitter.com/@UKKidney) * E-mail - rrsystems@renalregistry.nhs.uk Project Link -
+[https://github.com/renalreg/ukrr_models](https://github.com/renalreg/
+ukrr_models)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [issues-shield]: https://img.shields.io/github/issues/renalreg/
 ukrr_models.svg?style=for-the-badge [issues-url]: https://github.com/renalreg/
 ukrr_models/issues [license-shield]: https://img.shields.io/github/license/
 renalreg/ukrr_models.svg?style=for-the-badge [license-url]: https://github.com/
 renalreg/ukrr_models/blob/master/LICENSE [SQLAlchemy]: https://img.shields.io/
 badge/sqlalchemy-V1.4-D71F00?style=for-the-badge&logoColor=white [SQLAlchemy-
```

### Comparing `ukrr_models-1.0.0/ukrr_models/nhsbt_models.py` & `ukrr_models-2.1.1/ukrr_models/nhsbt_models.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-"""SQLAlchemy models for NHSBT"""
-
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy import Column, Integer, String, DateTime, MetaData, Boolean
-
-metadata = MetaData()
-Base = declarative_base(metadata=metadata)
-
-
-class UKTPatient(Base):
-    __tablename__ = "ukt_patients"
-
-    uktssa_no = Column(Integer, primary_key=True, autoincrement=False)
-    surname = Column(String(50))
-    forename = Column(String(50))
-    sex = Column(String(1))
-    post_code = Column(String(10))
-    new_nhs_no = Column(Integer)
-    chi_no = Column(Integer)
-    hsc_no = Column(Integer)
-    rr_no = Column(Integer)
-    ukt_date_death = Column(DateTime)
-    ukt_date_birth = Column(DateTime)
-
-
-class UKTTransplant(Base):
-    __tablename__ = "ukt_transplants"
-
-    registration_id = Column(String(12), primary_key=True)
-    uktssa_no = Column(Integer)
-    transplant_id = Column(Integer)
-    transplant_type = Column(String(10))
-    transplant_organ = Column(String(50))
-    transplant_unit = Column(String(50))
-    rr_no = Column(Integer)
-    transplant_date = Column(DateTime)
-    ukt_fail_date = Column(DateTime)
-    registration_date = Column(DateTime)
-    registration_date_type = Column(String(12))
-    registration_end_date = Column(DateTime)
-    registration_end_status = Column(String(12))
-    transplant_consideration = Column(String(20))
-    transplant_dialysis = Column(String(12))
-    transplant_relationship = Column(String(20))
-    transplant_sex = Column(String(12))
-    cause_of_failure = Column(String(10))
-    cause_of_failure_text = Column(String(500))
-    cit_mins = Column(String(10))
-    hla_mismatch = Column(String(10))
-    ukt_suspension = Column(Boolean)
+"""SQLAlchemy models for NHSBT"""
+
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import Column, Integer, String, DateTime, MetaData, Boolean
+
+metadata = MetaData()
+Base = declarative_base(metadata=metadata)
+
+
+class UKTPatient(Base):
+    __tablename__ = "ukt_patients"
+
+    uktssa_no = Column(Integer, primary_key=True, autoincrement=False)
+    surname = Column(String(50))
+    forename = Column(String(50))
+    sex = Column(String(1))
+    post_code = Column(String(10))
+    new_nhs_no = Column(Integer)
+    chi_no = Column(Integer)
+    hsc_no = Column(Integer)
+    rr_no = Column(Integer)
+    ukt_date_death = Column(DateTime)
+    ukt_date_birth = Column(DateTime)
+
+
+class UKTTransplant(Base):
+    __tablename__ = "ukt_transplants"
+
+    registration_id = Column(String(12), primary_key=True)
+    uktssa_no = Column(Integer)
+    transplant_id = Column(Integer)
+    transplant_type = Column(String(10))
+    transplant_organ = Column(String(50))
+    transplant_unit = Column(String(50))
+    rr_no = Column(Integer)
+    transplant_date = Column(DateTime)
+    ukt_fail_date = Column(DateTime)
+    registration_date = Column(DateTime)
+    registration_date_type = Column(String(12))
+    registration_end_date = Column(DateTime)
+    registration_end_status = Column(String(12))
+    transplant_consideration = Column(String(20))
+    transplant_dialysis = Column(String(12))
+    transplant_relationship = Column(String(20))
+    transplant_sex = Column(String(12))
+    cause_of_failure = Column(String(10))
+    cause_of_failure_text = Column(String(500))
+    cit_mins = Column(String(10))
+    hla_mismatch = Column(String(10))
+    ukt_suspension = Column(Boolean)
```

### Comparing `ukrr_models-1.0.0/ukrr_models/rr_models.py` & `ukrr_models-2.1.1/ukrr_models/rr_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from sqlalchemy import Column, Date, ForeignKey, Integer, String
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import Mapped, relationship
-
-Base = declarative_base()
-
-
-class UKRRPatient(Base):
-    __tablename__ = "patients"
-
-    # This is (probably) the last centre for which a file was
-    # loaded and not neccesarily the latest/main unit they
-    # attend.
-    hosp_centre = Column(String)
-
-    rr_no = Column(Integer, primary_key=True)
-    surname = Column(String)
-    forename = Column(String)
-    sex = Column(String)
-
-    nhs_no = Column("new_nhs_no", Integer)
-    chi_no = Column(Integer)
-    hsc_no = Column(Integer)
-    uktssa_no = Column(Integer)
-
-    date_birth = Column(Date)
-    date_death = Column(Date)
-
-    ethnicity = Column("ethgr_code", String)
-
-    blood_group = Column(String)
-    blood_rhesus = Column("blood_group_rhesus", String)
-
-    cod_read = Column(String)
-    # TODO: These should be updated to String in the DB.
-    cod_edta1 = Column(Integer)
-    cod_edta2 = Column(Integer)
-    cod_text = Column(String)
-
-    # This is the date the patient was
-    # first loaded into the UKRR database
-    date_registered = Column(Date)
-
-    first_seen_date = Column(Date)
-
-    patient_demographics: Mapped[Integer] = relationship(
-        "Patient_Demographics", backref="patient", lazy="dynamic"
-    )
-
-
-class Patient_Demographics(Base):
-    __tablename__ = "patient_demog"
-
-    rr_no = Column(Integer, ForeignKey("patients.rr_no"), primary_key=True)
-    hosp_centre = Column(String, primary_key=True)
-
-    surname = Column(String)
-    forename = Column(String)
-    birth_name = Column(String)
-    alias_name = Column(String)
-    date_birth = Column(Date)
-    date_death = Column(Date)
-
-    nhs_no = Column("new_nhs_no", Integer)
-    chi_no = Column(Integer)
-    hsc_no = Column(Integer)
-    uktssa_no = Column(Integer)
-    local_hosp_no = Column(String)
-
-    first_seen_date = Column(Date)
-
-
-class UKRR_Deleted_Patient(Base):
-    __tablename__ = "deleted_patients"
-
-    rr_no = Column(Integer, primary_key=True)
-    surname = Column(String)
-    forename = Column(String)
-    sex = Column(String)
-
-    nhs_no = Column("new_nhs_no", Integer)
-    chi_no = Column(Integer)
-    hsc_no = Column(Integer)
-    uktssa_no = Column(Integer)
-
-    local_hosp_no = Column(String)
-
-    date_birth = Column(Date)
-    date_death = Column(Date)
+from sqlalchemy import Column, Date, ForeignKey, Integer, String
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import Mapped, relationship
+
+Base = declarative_base()
+
+
+class UKRRPatient(Base):
+    __tablename__ = "patients"
+
+    # This is (probably) the last centre for which a file was
+    # loaded and not neccesarily the latest/main unit they
+    # attend.
+    hosp_centre = Column(String)
+
+    rr_no = Column(Integer, primary_key=True)
+    surname = Column(String)
+    forename = Column(String)
+    sex = Column(String)
+
+    nhs_no = Column("new_nhs_no", Integer)
+    chi_no = Column(Integer)
+    hsc_no = Column(Integer)
+    uktssa_no = Column(Integer)
+
+    date_birth = Column(Date)
+    date_death = Column(Date)
+
+    ethnicity = Column("ethgr_code", String)
+
+    blood_group = Column(String)
+    blood_rhesus = Column("blood_group_rhesus", String)
+
+    cod_read = Column(String)
+    # TODO: [GIT-18] These should be updated to String in the DB.
+    cod_edta1 = Column(Integer)
+    cod_edta2 = Column(Integer)
+    cod_text = Column(String)
+
+    # This is the date the patient was
+    # first loaded into the UKRR database
+    date_registered = Column(Date)
+
+    first_seen_date = Column(Date)
+
+    patient_demographics: Mapped[Integer] = relationship(
+        "Patient_Demographics", backref="patient", lazy="dynamic"
+    )
+
+
+class Patient_Demographics(Base):
+    __tablename__ = "patient_demog"
+
+    rr_no = Column(Integer, ForeignKey("patients.rr_no"), primary_key=True)
+    hosp_centre = Column(String, primary_key=True)
+
+    surname = Column(String)
+    forename = Column(String)
+    birth_name = Column(String)
+    alias_name = Column(String)
+    date_birth = Column(Date)
+    date_death = Column(Date)
+
+    nhs_no = Column("new_nhs_no", Integer)
+    chi_no = Column(Integer)
+    hsc_no = Column(Integer)
+    uktssa_no = Column(Integer)
+    local_hosp_no = Column(String)
+
+    first_seen_date = Column(Date)
+
+
+class UKRR_Deleted_Patient(Base):
+    __tablename__ = "deleted_patients"
+
+    rr_no = Column(Integer, primary_key=True)
+    surname = Column(String)
+    forename = Column(String)
+    sex = Column(String)
+
+    nhs_no = Column("new_nhs_no", Integer)
+    chi_no = Column(Integer)
+    hsc_no = Column(Integer)
+    uktssa_no = Column(Integer)
+
+    local_hosp_no = Column(String)
+
+    date_birth = Column(Date)
+    date_death = Column(Date)
```

### Comparing `ukrr_models-1.0.0/PKG-INFO` & `ukrr_models-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ukrr-models
-Version: 1.0.0
+Version: 2.1.1
 Summary: Models of the UKRR database
 License: MIT
 Author: UK Renal Registry
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sqlalchemy (==1.4.52)
+Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 <div align='center'>
 
 [![Issues][issues-shield]][issues-url]
@@ -43,17 +43,20 @@
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
 
 ## Contact
 
-Renal Registry - [@UKKidney](https://twitter.com/@UKKidney) - rrsystems@renalregistry.nhs.uk
+Renal Registry 
+* Website - [The UK Kidney Association](https://ukkidney.org/)
+* X - [@UKKidney](https://twitter.com/@UKKidney)
+* E-mail -  rrsystems@renalregistry.nhs.uk
 
-Project Link: [https://github.com/renalreg/ukrr_models](https://github.com/renalreg/rr-connection-manager)
+Project Link - [https://github.com/renalreg/ukrr_models](https://github.com/renalreg/ukrr_models)
 
 <br />
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 [issues-shield]: https://img.shields.io/github/issues/renalreg/ukrr_models.svg?style=for-the-badge
 [issues-url]: https://github.com/renalreg/ukrr_models/issues
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: ukrr-models Version: 1.0.0 Summary: Models of the
+Metadata-Version: 2.1 Name: ukrr-models Version: 2.1.1 Summary: Models of the
 UKRR database License: MIT Author: UK Renal Registry Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: sqlalchemy (==1.4.52) Description-Content-Type: text/markdown
+Dist: sqlalchemy (>=2.0.0,<3.0.0) Description-Content-Type: text/markdown
     [![Issues][issues-shield]][issues-url] [![MIT License][license-shield]]
                                  [license-url]
 
                            ************ UUKKRRRR MMooddeellss ************
 ## About The Project A limited set of database models for the RR database
 ## Usage ``` poetry add ukrr_models ``` ## Built With [![SQLAlchemy]
 [SQLAlchemy]][SQLAlchemy-url] ## License Distributed under the MIT License. See
-`LICENSE` for more information. ## Contact Renal Registry - [@UKKidney](https:/
-/twitter.com/@UKKidney) - rrsystems@renalregistry.nhs.uk Project Link: [https:/
-/github.com/renalreg/ukrr_models](https://github.com/renalreg/rr-connection-
-manager)
+`LICENSE` for more information. ## Contact Renal Registry * Website - [The UK
+Kidney Association](https://ukkidney.org/) * X - [@UKKidney](https://
+twitter.com/@UKKidney) * E-mail - rrsystems@renalregistry.nhs.uk Project Link -
+[https://github.com/renalreg/ukrr_models](https://github.com/renalreg/
+ukrr_models)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [issues-shield]: https://img.shields.io/github/issues/renalreg/
 ukrr_models.svg?style=for-the-badge [issues-url]: https://github.com/renalreg/
 ukrr_models/issues [license-shield]: https://img.shields.io/github/license/
 renalreg/ukrr_models.svg?style=for-the-badge [license-url]: https://github.com/
 renalreg/ukrr_models/blob/master/LICENSE [SQLAlchemy]: https://img.shields.io/
 badge/sqlalchemy-V1.4-D71F00?style=for-the-badge&logoColor=white [SQLAlchemy-
```

