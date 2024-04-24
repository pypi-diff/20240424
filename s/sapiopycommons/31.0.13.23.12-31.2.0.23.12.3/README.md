# Comparing `tmp/sapiopycommons-31.0.13.23.12.tar.gz` & `tmp/sapiopycommons-31.2.0.23.12.3.tar.gz`

## Comparing `sapiopycommons-31.0.13.23.12.tar` & `sapiopycommons-31.2.0.23.12.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/chem/IndigoMolecules.py
--rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/chem/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/chem/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/datatype/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/datatype/attachment_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/eln/__init__.py
--rw-r--r--   0        0        0    44297 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/eln/experiment_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/files/__init__.py
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/files/file_bridge.py
--rw-r--r--   0        0        0    23138 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/files/file_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/__init__.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/aliases.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/custom_report_util.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/exceptions.py
--rw-r--r--   0        0        0    28858 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/popup_util.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/time_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/recordmodel/__init__.py
--rw-r--r--   0        0        0    34307 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/recordmodel/record_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/rules/__init__.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/rules/eln_rule_handler.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/rules/on_save_rule_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/webhook/__init__.py
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/src/sapiopycommons/webhook/webhook_handlers.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/pyproject.toml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 sapiopycommons-31.0.13.23.12/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/__init__.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/__init__.py
+-rw-r--r--   0        0        0    54417 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/__init__.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py
+-rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/aliases.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py
+-rw-r--r--   0        0        0    29150 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/__init__.py
+-rw-r--r--   0        0        0    34338 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/__init__.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/__init__.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/LICENSE
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/pyproject.toml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 sapiopycommons-31.2.0.23.12.3/PKG-INFO
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/chem/IndigoMolecules.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/IndigoMolecules.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 indigo.setOption("aromaticity-model", "generic")
 indigo.setOption("render-coloring", True)
 indigo_inchi = IndigoInchi(indigo);
 
 
 def highlight_mol_substructure(query: IndigoObject, sub_match: IndigoObject):
     """
-    Highlight the bonds and atoms for substructure search result
-    :param sub_match: The substructure search match obtained from indigo.substructureMatcher(mol).match(query)
-    :param query: The query we were running to match the original structure
+    Highlight the bonds and atoms for substructure search result.
+
+    :param sub_match: The substructure search match obtained from indigo.substructureMatcher(mol).match(query).
+    :param query: The query we were running to match the original structure.
     """
     for qatom in query.iterateAtoms():
         atom = sub_match.mapAtom(qatom)
         if atom is None:
             continue
         atom.highlight()
 
@@ -34,15 +35,16 @@
             continue
         bond.highlight()
 
 
 def highlight_reactions(query_reaction_smarts: IndigoObject, reaction_match: IndigoObject):
     """
     Highlight the bonds and atoms for substructure search result of reaction that's in the query and survived the mapping.
+
     :param query_reaction_smarts: The query we ran substructure search on.
-    :param reaction_match: The substructure search match obtained from indigo.substructureMatcher(reaction).match(query)
+    :param reaction_match: The substructure search match obtained from indigo.substructureMatcher(reaction).match(query).
     :return:
     """
     for q_mol in query_reaction_smarts.iterateMolecules():
         matched_mol = reaction_match.mapMolecule(q_mol)
         sub_match = indigo.substructureMatcher(matched_mol).match(q_mol)
         highlight_mol_substructure(q_mol, sub_match)
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/chem/Molecules.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/chem/Molecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,61 +37,65 @@
             atom.UpdatePropertyCache()
     return mol
 
 
 def find_all_possible_stereoisomers(m: Mol, only_unassigned=True, try_embedding=True, unique=True, max_isomers=200) \
         -> list[Mol]:
     """
-    Find all possible candidates of stereoisomers given the current molecule
-    :param m: The molecule to search for
+    Find all possible candidates of stereoisomers given the current molecule.
+
+    :param m: The molecule to search for.
     :param only_unassigned: Whether to only permute on unspecified stereocenter.
     :param try_embedding: if set the process attempts to generate a standard RDKit distance geometry conformation for
     the stereisomer.
-    If this fails, we assume that the stereoisomer is non-physical and don't return it
-    :param unique: whether to remove duplicates by isomer identity
+    If this fails, we assume that the stereoisomer is non-physical and don't return it.
+    :param unique: whether to remove duplicates by isomer identity.
     :param max_isomers: Maximum number of search results to return.
     """
     # noinspection PyBroadException
     try:
         opts = StereoEnumerationOptions(tryEmbedding=try_embedding, unique=unique, onlyUnassigned=only_unassigned,
                                         maxIsomers=max_isomers)
         return list(EnumerateStereoisomers(m, options=opts))
     except:
         return []
 
 
 def has_chiral_centers(m: Mol):
     """
-    Returns true iff the molecule provided has at least 1 chiral centers (when stereochemistry is relevant)
+    Returns true iff the molecule provided has at least 1 chiral centers (when stereochemistry is relevant).
+
     :param m: The molecule to test.
     """
     # noinspection PyBroadException
     try:
         chiral_centers: list = Chem.FindMolChiralCenters(m, force=True, includeUnassigned=True,
                                                          useLegacyImplementation=False)
         return len(chiral_centers) > 0
     except:
         return False
 
 
 def mol_to_img(mol_str: str) -> str:
     """
-    Convert molecule into image
-    :param mol_str: The molecule INCHI
+    Convert molecule into image.
+
+    :param mol_str: The molecule INCHI.
     :return: The SVG image text.
     """
     mol = indigo.loadMolecule(mol_str)
     return renderer.renderToString(mol)
 
 
 
 def mol_to_sapio_partial_pojo(mol: Mol):
     """
     Get the minimum information about molecule to Sapio, just its SMILES, V3000, and image data.
-    :param mol: The molecule to read the simplified data from
+
+    :param mol: The molecule to read the simplified data from.
     """
     Chem.SanitizeMol(mol)
     mol.UpdatePropertyCache()
     smiles = Chem.MolToSmiles(mol)
     molBlock = Chem.MolToMolBlock(mol)
     img = mol_to_img(mol)
     molecule = dict()
@@ -102,15 +106,16 @@
 
 
 def mol_to_sapio_substance(mol: Mol, include_stereoisomers: bool = False,
                            normalize: bool = False, remove_salt: bool = False, make_images: bool = False,
                            salt_def: str | None = None, canonical_tautomer: bool = True):
     """
     Convert a molecule in RDKit to a molecule POJO in Sapio.
-    :param mol: The molecule in RDKit
+
+    :param mol: The molecule in RDKit.
     :param include_stereoisomers: If true, will compute all stereoisomer permutations of this molecule.
     :param normalize If true, will normalize the functional groups and return normalized result.
     :param remove_salt If true, we will remove salts iteratively from the molecule before returning their data.
     We will also populate desaltedList with molecules we deleted.
     :param salt_def: if not none, specifies custom salt to be used during the desalt process.
     :param canonical_tautomer: if True, we will attempt to compute canonical tautomer for the molecule. Slow!
     This is needed for a registry. Note it stops after enumeration of 1000.
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/datatype/attachment_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/datatype/attachment_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class AttachmentUtil:
     @staticmethod
     def get_attachment_bytes(context: SapioWebhookContext, attachment: SapioRecord) -> bytes:
         """
         Get the data bytes for the given attachment record. Makes a webservice call to retrieve the data.
+
         :param context: The current webhook context.
         :param attachment: The attachment record.
         :return: The bytes for the attachment's file data.
         """
         attachment = AliasUtil.to_data_record(attachment)
         with io.BytesIO() as data_sink:
             def consume_data(chunk: bytes):
@@ -30,14 +31,15 @@
         return file_bytes
 
     @staticmethod
     def set_attachment_bytes(context: SapioWebhookContext, attachment: SapioRecord,
                              file_name: str, file_bytes: bytes) -> None:
         """
         Set the attachment data for a given attachment record. Makes a webservice call to set the data.
+
         :param context: The current webhook context.
         :param attachment: The attachment record. Must be an existing data record that is an attachment type.
         :param file_name: The name of the attachment.
         :param file_bytes: The bytes of the attachment data.
         """
         if attachment.record_id < 0:
             raise SapioException("Provided record cannot have its attachment data set, as it does not exist in the "
@@ -48,14 +50,15 @@
 
     @staticmethod
     def create_attachment(context: SapioWebhookContext, file_name: str, file_bytes: bytes,
                           wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Create an attachment data type and initialize its attachment bytes at the same time.
         Makes a webservice call to create the attachment record and a second to set its bytes.
+
         :param context: The current webhook context.
         :param file_name: The name of the attachment.
         :param file_bytes: THe bytes of the attachment data.
         :param wrapper_type: The attachment type to create.
         :return: A record model for the newly created attachment.
         """
         inst_man = RecordModelManager(context.user).instance_manager
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/eln/experiment_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/eln/experiment_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 from sapiopylib.rest.ELNService import ElnManager
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 from sapiopylib.rest.pojo.eln.ElnExperiment import ElnExperiment, TemplateExperimentQueryPojo, ElnTemplate, \
     InitializeNotebookExperimentPojo, ElnExperimentUpdateCriteria
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry
 from sapiopylib.rest.pojo.eln.ExperimentEntryCriteria import AbstractElnEntryUpdateCriteria
-from sapiopylib.rest.pojo.eln.SapioELNEnums import ExperimentEntryStatus, ElnExperimentStatus
+from sapiopylib.rest.pojo.eln.SapioELNEnums import ExperimentEntryStatus, ElnExperimentStatus, ElnEntryType, \
+    ElnBaseDataType
 from sapiopylib.rest.pojo.webhook.WebhookContext import SapioWebhookContext
 from sapiopylib.rest.pojo.webhook.WebhookDirective import ElnExperimentDirective
 from sapiopylib.rest.pojo.webhook.WebhookResult import SapioWebhookResult
 from sapiopylib.rest.utils.Protocols import ElnEntryStep, ElnExperimentProtocol
+from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel
 from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelInstanceManager, RecordModelManager
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedType
 
 from sapiopycommons.general.aliases import AliasUtil, SapioRecord
 from sapiopycommons.general.exceptions import SapioException
 
 Step = str | ElnEntryStep
@@ -68,112 +70,173 @@
     __COMPLETE_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value]
     """The set of statuses that an ELN entry could have and be considered completed/submitted."""
     __LOCKED_STATUSES = [ExperimentEntryStatus.Completed.value, ExperimentEntryStatus.CompletedApproved.value,
                          ExperimentEntryStatus.Disabled.value, ExperimentEntryStatus.LockedAwaitingApproval.value,
                          ExperimentEntryStatus.LockedRejected.value]
     """The set of statuses that an ELN entry could have and be considered locked."""
 
-    def __init__(self, context: SapioWebhookContext):
+    def __init__(self, context: SapioWebhookContext, experiment: ElnExperiment | None = None):
         """
-        Initialization will throw an exception if there is no ELN Experiment in the provided context.
+        Initialization will throw an exception if there is no ELN Experiment in the provided context and no experiment
+        is provided.
+
         :param context: The current webhook context.
+        :param experiment: If an experiment is provided that is separate from the experiment that is in the context,
+            that experiment will be used by this ExperimentHandler instead.
         """
-        if context.eln_experiment is None:
+        # FR-46495 - Allow the init function of ExperimentHandler to take in an ElnExperiment that is separate from the
+        # context.
+        if context.eln_experiment is None and experiment is None:
             raise SapioException("Cannot initialize ExperimentHandler. No ELN Experiment in the context.")
+        if context.eln_experiment == experiment:
+            experiment = None
         self.__context = context
 
         # Get the basic information about this experiment that already exists in the context and is often used.
-        self.__eln_exp = context.eln_experiment
-        # noinspection PyTypeChecker
-        self.__protocol = context.active_protocol
+        self.__eln_exp = experiment if experiment else context.eln_experiment
+        self.__protocol = ElnExperimentProtocol(experiment, context.user) if experiment else context.active_protocol
         self.__exp_id = self.__protocol.get_id()
 
         # Grab various managers that may be used.
         self.__eln_man = context.eln_manager
         self.__inst_man = RecordModelManager(context.user).instance_manager
 
         # Create empty caches to fill when necessary.
         self.__steps = {}
         self.__step_options = {}
         # CR-46330: Cache any experiment entry information that might already exist in the context.
         self.__queried_all_steps = False
-        if context.experiment_entry is not None:
-            self.__steps.update({context.active_step.get_name(): context.active_step})
-        if context.experiment_entry_list is not None:
-            for entry in context.experiment_entry_list:
-                self.__steps.update({entry.entry_name: ElnEntryStep(self.__protocol, entry)})
+        # We can only trust the entries in the context if no experiment was given as an input parameter.
+        if experiment is None:
+            if context.experiment_entry is not None:
+                self.__steps.update({context.active_step.get_name(): context.active_step})
+            if context.experiment_entry_list is not None:
+                for entry in context.experiment_entry_list:
+                    self.__steps.update({entry.entry_name: ElnEntryStep(self.__protocol, entry)})
 
+    # FR-46495: Split the creation of the experiment in launch_experiment into a create_experiment function.
     @staticmethod
-    def launch_experiment(context: SapioWebhookContext,
+    def create_experiment(context: SapioWebhookContext,
                           template_name: str,
                           experiment_name: str | None = None,
-                          parent_record: SapioRecord | None = None) -> SapioWebhookResult:
+                          parent_record: SapioRecord | None = None, *,
+                          template_version: int | None = None, active_templates_only: bool = True) -> ElnExperiment:
         """
-        Create a SapioWebhookResult that, when returned by a webhook handler, sends the user to a new experiment of the
-        input template name. Queries for all the active templates of the latest version. Throws an exception if a
-        template of the given name is not found.
+        Create an ElnExperiment from the given template name.
+
+        Makes a webservice request to query for all the templates matching the provided criteria. Note that if multiple
+        templates match the same criteria, the first template that is encountered in the query is used. Throws an
+        exception if no template is found. Also makes a webservice request to create the experiment.
+
         :param context: The current webhook context.
         :param template_name: The name of the template to create the experiment from.
         :param experiment_name: The name to give to the experiment after it is created. If not provided, defaults to the
             display name of the template.
         :param parent_record: The parent record to attach this experiment under. This record must be an eligible
             parent type to ELNExperiment. If not provided, the experiment is stored in the aether.
-        :return: A SapioWebhookResult that directs the user to the newly created experiment.
+        :param template_version: The version number of the template to use. If not provided, the latest version of the
+            template is used. NOTICE: Template version numbers aren't necessarily the same between environments, so
+            be careful with using the same webhook across multiple environments if you are searching for a specific
+            version number.
+        :param active_templates_only: Whether only active templates should be queried for.
+        :return: The newly created experiment.
         """
-        template_query = TemplateExperimentQueryPojo(latest_version_only=True, active_templates_only=True)
+        template_query = TemplateExperimentQueryPojo(latest_version_only=(template_version is None),
+                                                     active_templates_only=active_templates_only)
         templates: list[ElnTemplate] = context.eln_manager.get_template_experiment_list(template_query)
         launch_template: ElnTemplate | None = None
         for template in templates:
-            if template.template_name == template_name:
-                launch_template = template
-                break
+            if template.template_name != template_name:
+                continue
+            if template_version is not None and template.template_version != template_version:
+                continue
+            launch_template = template
+            break
         if launch_template is None:
-            raise SapioException(f"No template with the name \"{template_name}\" found.")
+            raise SapioException(f"No template with the name \"{template_name}\"" +
+                                 ("" if template_version is None else f" and the version {template_version}") +
+                                 f" found.")
 
         if experiment_name is None:
             experiment_name: str = launch_template.display_name
         if parent_record is not None:
             parent_record: DataRecord = AliasUtil.to_data_record(parent_record)
         notebook_init = InitializeNotebookExperimentPojo(experiment_name, launch_template.template_id, parent_record)
-        experiment: ElnExperiment = context.eln_manager.create_notebook_experiment(notebook_init)
+        return context.eln_manager.create_notebook_experiment(notebook_init)
+
+    @staticmethod
+    def launch_experiment(context: SapioWebhookContext,
+                          template_name: str,
+                          experiment_name: str | None = None,
+                          parent_record: SapioRecord | None = None, *,
+                          template_version: int | None = None, active_templates_only: bool = True) -> SapioWebhookResult:
+        """
+        Create a SapioWebhookResult that, when returned by a webhook handler, sends the user to a new experiment of the
+        input template name.
+
+        Makes a webservice request to query for all the templates matching the provided criteria. Note that if multiple
+        templates match the same criteria, the first template that is encountered in the query is used. Throws an
+        exception if no template is found. Also makes a webservice request to create the experiment.
+
+        :param context: The current webhook context.
+        :param template_name: The name of the template to create the experiment from.
+        :param experiment_name: The name to give to the experiment after it is created. If not provided, defaults to the
+            display name of the template.
+        :param parent_record: The parent record to attach this experiment under. This record must be an eligible
+            parent type to ELNExperiment. If not provided, the experiment is stored in the aether.
+        :param template_version: The version number of the template to use. If not provided, the latest version of the
+            template is used. NOTICE: Template version numbers aren't necessarily the same between environments, so
+            be careful with using the same webhook across multiple environments if you are searching for a specific
+            version number.
+        :param active_templates_only: Whether only active templates should be queried for.
+        :return: A SapioWebhookResult that directs the user to the newly created experiment.
+        """
+        experiment = ExperimentHandler.create_experiment(context, template_name, experiment_name, parent_record,
+                                                         template_version=template_version,
+                                                         active_templates_only=active_templates_only)
         return SapioWebhookResult(True, directive=ElnExperimentDirective(experiment.notebook_experiment_id))
 
     def get_experiment_template(self, exception_on_none: bool = True) -> ElnTemplate | None:
         """
         Query for the experiment template for the current experiment. The returned template is cached by the
         ExperimentHandler.
+
         :param exception_on_none: If false, returns None if there is no experiment template. If true, raises an exception
             when the experiment template doesn't exist.
         :return: This experiment's template. None if it has no template.
         """
         template_id: int | None = self.__eln_exp.template_id
         if template_id is None:
             if exception_on_none:
                 raise SapioException(f"Experiment with ID {self.__exp_id} has no template ID.")
             return None
 
         if not hasattr(self, "_ExperimentHandler__exp_template"):
-            query = TemplateExperimentQueryPojo(template_id_white_list=[template_id])
+            # PR-46504: Allow inactive and non-latest version templates to be queried.
+            query = TemplateExperimentQueryPojo(template_id_white_list=[template_id],
+                                                active_templates_only=False,
+                                                latest_version_only=False)
             templates: list[ElnTemplate] = self.__eln_man.get_template_experiment_list(query)
-            if len(templates) > 0:
-                self.__exp_template = templates[0]
+            # PR-46504: Set the exp_template to None if there are no results.
+            self.__exp_template = templates[0] if templates else None
         if self.__exp_template is None and exception_on_none:
             raise SapioException(f"Experiment template not found for experiment with ID {self.__exp_id}.")
         return self.__exp_template
 
     # CR-46104: Change get_template_name to behave like NotebookProtocolImpl.getTemplateName (i.e. first see if the
     # experiment template exists, and if not, see if the experiment record exists, instead of only checking the
     # template).
     def get_template_name(self, exception_on_none: bool = True) -> str | None:
         """
         Get the template name for the current experiment.
 
         The template name is determined by either the experiment template or the experiment record, whichever is
         already cached. If neither are cached, queries for the experiment template. If no experiment template exists,
         queries for the experiment record.
+
         :param exception_on_none: If false, returns None if there is no template name. If true, raises an exception
             when the template name doesn't exist.
         :return: The template name of the current experiment. None if it has no template name.
         """
         if not hasattr(self, "_ExperimentHandler__exp_template"):
             self.get_experiment_template(False)
         if self.__exp_template is None and not hasattr(self, "_ExperimentHandler__exp_record"):
@@ -187,44 +250,47 @@
         if name is None and exception_on_none:
             raise SapioException(f"Template name not found for experiment with ID {self.__exp_id}.")
         return name
 
     def get_experiment_record(self, exception_on_none: bool = True) -> DataRecord | None:
         """
         Query for the data record of this experiment. The returned record is cached by the ExperimentHandler.
+
         :param exception_on_none: If false, returns None if there is no experiment record. If true, raises an exception
             when the experiment record doesn't exist.
         :return: The data record for this experiment. None if it has no record.
         """
         if not hasattr(self, "_ExperimentHandler__exp_record"):
             drm = self.__context.data_record_manager
             dt = self.__eln_exp.experiment_data_type_name
             results = drm.query_data_records_by_id(dt, [self.__eln_exp.experiment_record_id]).result_list
-            if len(results) > 0:
-                self.__exp_record = results[0]
+            # PR-46504: Set the exp_record to None if there are no results.
+            self.__exp_record = results[0] if results else None
         if self.__exp_record is None and exception_on_none:
             raise SapioException(f"Experiment record not found for experiment with ID {self.__exp_id}.")
         return self.__exp_record
 
     def get_experiment_model(self, wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Query for the data record of this experiment and wrap it as a record model with the given wrapper.
         The returned record is cached by the ExperimentHandler.
+
         :param wrapper_type: The record model wrapper to use.
         :return: The record model for this experiment.
         """
         return self.__inst_man.add_existing_record_of_type(self.get_experiment_record(), wrapper_type)
 
     def update_experiment(self,
                           experiment_name: str | None = None,
                           experiment_status: ElnExperimentStatus | None = None,
                           experiment_option_map: dict[str, str] | None = None) -> None:
         """
         Make a webservice call to update the experiment for this ExperimentHandler.  If any parameter is not provided,
         then no change is made to it.
+
         :param experiment_name: The new name of the experiment.
         :param experiment_status: The new status of this experiment.
         :param experiment_option_map:
             The new map of options for this experiment. Completely overwrites the existing options map.
             Any changes to the experiment options will update this ExperimentHandler's cache of the experiment options.
             If you wish to add options to the existing map of options that an experiment has, use the
             add_experiment_options method.
@@ -245,88 +311,95 @@
     def get_experiment_option(self, option: str) -> str:
         """
         Get the value of a specific experiment option.
 
         Getting the experiment options requires a webservice query, which is made the first time any experiment option
         method is called by this ExperimentHandler. The experiment options are cached so that subsequent calls of this
         method don't make a webservice call.
+
         :param option: The experiment option to search for.
         :return: The value of the input experiment options.
         """
         return self.get_experiment_options().get(option)
 
     def get_experiment_options(self) -> dict[str, str]:
         """
         Get the entire map of options for this experiment.
 
         Getting the experiment options requires a webservice query, which is made the first time any experiment option
         method is called by this ExperimentHandler. The experiment options are cached so that subsequent calls of this
         method don't make a webservice call.
+
         :return: The map of options for this experiment.
         """
         return self.__get_experiment_options()
 
     def add_experiment_options(self, mapping: Mapping[str, str]) -> None:
         """
         Add to the existing map of options for this experiment. Makes a webservice call to update the experiment. Also
         updates the cache of the experiment options.
 
         Getting the experiment options requires a webservice query, which is made the first time any experiment option
         method is called by this ExperimentHandler. The experiment options are cached so that subsequent calls of this
         method don't make a webservice call.
+
         :param mapping: The new options and values to add to the existing experiment options, provided as some Mapping
             (e.g. a Dict). If an option key already exists and is provided in the mapping, overwrites the existing value
             for that key.
         """
         options: dict[str, str] = self.get_experiment_options()
         options.update(mapping)
         self.update_experiment(experiment_option_map=options)
 
     def step_exists(self, step_name: str) -> bool:
         """
         Determine if a step by the given name exists in the experiment.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step_name: The name of the step to search for.
         :return: True if the step exists, false otherwise.
         """
         return self.get_step(step_name, False) is not None
 
     def steps_exist(self, step_names: Iterable[str]) -> bool:
         """
         Determine if all the steps by the given names exist in the experiment.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step_names: The names of the steps to search for.
         :return: True if every step exists, false if at least one does not exist.
         """
         return all([x is not None for x in self.get_steps(step_names, False)])
 
     def get_step(self, step_name: str, exception_on_none: bool = True) -> ElnEntryStep | None:
         """
         Get the step of the given name from the experiment.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step_name: The name for the step to return.
         :param exception_on_none: If false, returns None if the entry can't be found. If true, raises an exception
             when the named entry doesn't exist in the experiment.
         :return: An ElnEntrySteps matching the provided name. If there is no match and no exception is to be thrown,
             returns None.
         """
         return self.get_steps([step_name], exception_on_none)[0]
 
     def get_steps(self, step_names: Iterable[str], exception_on_none: bool = True) -> list[ElnEntryStep | None]:
         """
         Get a list of steps of the given names from the experiment, sorted in the same order as the names are provided.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step_names: A list of names for the entries to return and the order to return them in.
         :param exception_on_none: If false, returns None for entries that can't be found. If true, raises an exception
             when the named entry doesn't exist in the experiment.
         :return: A list of ElnEntrySteps matching the provided names in the order they were provided in. If there is no
             match for a given step and no exception is to be thrown, returns None for that step.
         """
         ret_list: list[ElnEntryStep | None] = []
@@ -346,14 +419,15 @@
 
     def get_step_records(self, step: Step) -> list[DataRecord]:
         """
         Query for the data records for the given step. The returned records are not cached by the ExperimentHandler.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to get the data records for.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: The data records for the given step.
         """
         return self.__to_eln_step(step).get_records()
@@ -361,46 +435,51 @@
     def get_step_models(self, step: Step, wrapper_type: type[WrappedType]) -> list[WrappedType]:
         """
         Query for the data records for the given step and wrap them as record models with the given type. The returned
         records are not cached by the ExperimentHandler.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to get the data records for.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param wrapper_type: The record model wrapper to use.
         :return: The record models for the given step.
         """
         return self.__inst_man.add_existing_records_of_type(self.get_step_records(step), wrapper_type)
 
     def add_step_records(self, step: Step, records: Iterable[SapioRecord]) -> None:
         """
-        Make a webservice call to add a list of records to a step.
+        Make a webservice call to add a list of records to a step. Only functions for global data type table entries.
+        For adding to an ELN data type table entry, see add_eln_rows.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to add the records to.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param records:
             A list of records to add to the given step.
             The records may be provided as either DataRecords, PyRecordModels, or WrappedRecordModels.
         """
         step = self.__to_eln_step(step)
         step.add_records(AliasUtil.to_data_records(records))
 
     def remove_step_records(self, step: Step, records: Iterable[SapioRecord]) -> None:
         """
-        Make a webservice call to remove a list of records from a step.
+        Make a webservice call to remove a list of records from a step. Only functions for global data type table
+        entries. For removing from an ELN data type table entry, see remove_eln_rows.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param records:
             A list of records to remove from the given step.
             The records may be provided as either DataRecords, PyRecordModels, or WrappedRecordModels.
         """
@@ -410,26 +489,120 @@
     def set_step_records(self, step: Step, records: Iterable[SapioRecord]) -> None:
         """
         Sets the records in the given step to be equal to the input list of records. If a record is already on the step,
         it remains. If a record is missing from the step, it gets added. If a record is on the step but not in the
         provided record list, it gets removed. Makes one webservice call to get what is currently on the step and
         one additional webservice call for each of either adding or removing, if necessary.
 
+        Functions for table, form, and attachment entries. For form and attachment entries, only a single record should
+        be provided.
+
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param records:
-            A list of records to remove from the given step,
+            A list of records to set for the given step,
             The records may be provided as either DataRecords, PyRecordModels, or WrappedRecordModels.
         """
         step = self.__to_eln_step(step)
         step.set_records(AliasUtil.to_data_records(records))
 
+    # FR-46496 - Provide alias of set_step_records for use with form entries.
+    # TODO: Provide a similar aliased function for attachment entries once sapiopylib allows setting multiple
+    #  attachments to an attachment step.
+    def set_form_record(self, step: Step, record: SapioRecord) -> None:
+        """
+        Sets the record for a form entry.
+
+        If no step functions have been called before and a step is being searched for by name, queries for the
+        list of steps in the experiment and caches them.
+
+        :param step:
+            The step may be provided as either a string for the name of the step or an ElnEntryStep.
+            If given a name, throws an exception if no step of the given name exists in the experiment.
+        :param record:
+            A record to set for the given step,
+            The record may be provided as either a DataRecord, PyRecordModel, or WrappedRecordModel.
+        """
+        self.set_step_records(step, [record])
+
+    # FR-46496 - Provide functions for adding and removing rows from an ELN data type entry.
+    def add_eln_rows(self, step: Step, count: int) -> list[PyRecordModel]:
+        """
+        Add rows to an ELNExperimentDetail or ELNSampleDetail table entry. The rows will not appear in the system
+        until a record manager store and commit has occurred.
+
+        If no step functions have been called before and a step is being searched for by name, queries for the
+        list of steps in the experiment and caches them.
+
+        :param step:
+            The step may be provided as either a string for the name of the step or an ElnEntryStep.
+            If given a name, throws an exception if no step of the given name exists in the experiment.
+        :param count: The number of new rows to add to the entry.
+        :return: A list of the newly created rows.
+        """
+        step = self.__to_eln_step(step)
+        if step.eln_entry.entry_type != ElnEntryType.Table:
+            raise SapioException("The provided step is not a table entry.")
+        dt: str = step.get_data_type_names()[0]
+        if not self.__is_eln_type(dt):
+            raise SapioException("The provided step is not an ELN data type entry.")
+        return self.__inst_man.add_new_records(dt, count)
+
+    def remove_eln_rows(self, step: Step, records: list[SapioRecord]) -> None:
+        """
+        Remove rows from an ELNExperimentDetail or ELNSampleDetail table entry. ELN data type table entries display all
+        records in the system that match the entry's data type. This means that removing rows from an ELN data type
+        table entry is equivalent to deleting the records for the rows.
+
+        The rows will not be deleted in the system until a record manager store and commit has occurred.
+
+        If no step functions have been called before and a step is being searched for by name, queries for the
+        list of steps in the experiment and caches them.
+
+        :param step:
+            The step may be provided as either a string for the name of the step or an ElnEntryStep.
+            If given a name, throws an exception if no step of the given name exists in the experiment.
+        :param records:
+            A list of records to remove from the given step.
+            The records may be provided as either DataRecords, PyRecordModels, or WrappedRecordModels.
+        """
+        step = self.__to_eln_step(step)
+        dt: str = step.get_data_type_names()[0]
+        if not self.__is_eln_type(dt):
+            raise SapioException("The provided step is not an ELN data type entry.")
+        if any([x.data_type_name != dt for x in records]):
+            raise SapioException("Not all of the provided records match the data type of the step.")
+        # If any rows were provided as data records, turn them into record models before deleting them, as otherwise
+        # this function would need to make a webservice call to do the deletion.
+        data_records: list[DataRecord] = []
+        for record in records:
+            if isinstance(record, DataRecord):
+                data_records.append(record)
+            else:
+                record.delete()
+        if data_records:
+            record_models: list[PyRecordModel] = self.__inst_man.add_existing_records(data_records)
+            for record in record_models:
+                record.delete()
+
+    # TODO: Remove and use the function of the same name in ElnBaseDataType in the future. Currently this function is
+    #  bugged in sapiopylib and is comparing against base_type.name instead of base_type.value.
+    @staticmethod
+    def __is_eln_type(data_type: str):
+        if data_type is None or not data_type:
+            return False
+        for base_type in ElnBaseDataType:
+            if data_type.lower().startswith(base_type.value.lower()):
+                return True
+        return False
+
     def update_step(self, step: Step,
                     entry_name: str | None = None,
                     related_entry_set: Iterable[int] | None = None,
                     dependency_set: Iterable[int] | None = None,
                     entry_status: ExperimentEntryStatus | None = None,
                     order: int | None = None,
                     description: str | None = None,
@@ -451,14 +624,15 @@
                     entry_options_map: dict[str, str] | None = None) -> None:
         """
         Make a webservice call to update an abstract step. If any parameter is not provided, then no change is made
         to it. All changes will be reflected by the ExperimentEntry of the Step that is being updated.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The entry step to update.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param entry_name: The new name of this entry.
         :param related_entry_set: The new set of entry IDs for the entries that are related (implicitly dependent) to
             this entry. Completely overwrites the existing related entries.
@@ -522,17 +696,20 @@
         criteria.is_shown_in_template = is_shown_in_template
         criteria.template_item_fulfilled_timestamp = template_item_fulfilled_timestamp
         criteria.clear_template_item_fulfilled_timestamp = clear_template_item_fulfilled_timestamp
         criteria.entry_options_map = entry_options_map
 
         self.__eln_man.update_experiment_entry(self.__exp_id, step.get_id(), criteria)
 
+        # Update the cached information for this entry in case it's needed by the caller after updating.
         entry: ExperimentEntry = step.eln_entry
         if entry_name is not None:
-            self.__steps.pop(entry.entry_name)
+            # PR-46477 - Ensure that the previous name of the updated entry already existed in the cache.
+            if entry.entry_name in self.__steps:
+                self.__steps.pop(entry.entry_name)
             entry.entry_name = entry_name
             self.__steps.update({entry_name: step})
         if related_entry_set is not None:
             entry.related_entry_id_set = related_entry_set
         if dependency_set is not None:
             entry.dependency_set = dependency_set
         if entry_status is not None:
@@ -583,14 +760,15 @@
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
 
         Getting the step options requires a webservice query, which is made the first time any step option
         method is called for a specific step. The step options are cached so that subsequent calls of this
         method for that step don't make a webservice call.
+
         :param step:
             The step to check the options of.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param option: The entry option to search for.
         :return: The value of the input entry option for the input step.
         """
@@ -602,14 +780,15 @@
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
 
         Getting the step options requires a webservice query, which is made the first time any step option
         method is called for a specific step. The step options are cached so that subsequent calls of this
         method for that step don't make a webservice call.
+
         :param step:
             The step to get the options of.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: The map of options for the input step.
         """
         return self.__get_step_options(step)
@@ -621,14 +800,15 @@
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
 
         Getting the step options requires a webservice query, which is made the first time any step option
         method is called for a specific step. The step options are cached so that subsequent calls of this
         method for that step don't make a webservice call.
+
         :param step:
             The step to update the options of.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :param mapping: The new options and values to add to the existing step options, provided as some Mapping
             (e.g. a Dict). If an option key already exists and is provided in the mapping, overwrites the existing value
             for that key.
@@ -640,14 +820,15 @@
     def initialize_step(self, step: Step) -> None:
         """
         Initialize the input step by setting its template item fulfilled timestamp to now. Makes a webservice call to
         update the step. Checks if the step already has a timestamp, and does nothing if so.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to initialize.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         # Avoid unnecessary calls if the step is already initialized.
         step: ElnEntryStep = self.__to_eln_step(step)
@@ -657,14 +838,15 @@
     def uninitialize_step(self, step: Step) -> None:
         """
         Uninitialize the input step by clearing its template item fulfilled timestamp to now. Makes a webservice call to
         update the step. Checks if the step already doesn't have a timestamp, and does nothing if so.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to uninitialize.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         # Avoid unnecessary calls if the step is already uninitialized.
         step: ElnEntryStep = self.__to_eln_step(step)
@@ -674,14 +856,15 @@
     def complete_step(self, step: Step) -> None:
         """
         Submit the input step. Makes a webservice call to update the step. Checks if the step is already completed, and
         does nothing if so.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to complete.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
         if step.eln_entry.entry_status not in self.__COMPLETE_STATUSES:
@@ -694,14 +877,15 @@
     def unlock_step(self, step: Step) -> None:
         """
         Set the status of the input step to UnlockedChangesRequired. Makes a webservice call to update the step. Checks
         if the step is already unlocked, and does nothing if so.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to unlock.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         """
         step = self.__to_eln_step(step)
         if step.eln_entry.entry_status in self.__LOCKED_STATUSES:
@@ -713,59 +897,64 @@
 
     def step_is_submitted(self, step: Step) -> bool:
         """
         Determine if the input step has already been submitted.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to check.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: True if the step's status is Completed or CompletedApproved. False otherwise.
         """
         return self.__to_eln_step(step).eln_entry.entry_status in self.__COMPLETE_STATUSES
 
     def step_is_locked(self, step: Step) -> bool:
         """
         Determine if the input step has been locked in any way.
 
         If no step functions have been called before and a step is being searched for by name, queries for the
         list of steps in the experiment and caches them.
+
         :param step:
             The step to check.
             The step may be provided as either a string for the name of the step or an ElnEntryStep.
             If given a name, throws an exception if no step of the given name exists in the experiment.
         :return: True if the step's status is Completed, CompletedApproved, Disabled, LockedAwaitingApproval,
             or LockedRejected. False otherwise.
         """
         return self.__to_eln_step(step).eln_entry.entry_status in self.__LOCKED_STATUSES
 
     def __to_eln_step(self, step: Step) -> ElnEntryStep:
         """
         Convert a variable that could be either a string or an ElnEntryStep to just an ElnEntryStep.
         This will query and cache the steps for the experiment if the input step is a name and the steps have not been
         cached before.
+
         :return: The input step as an ElnEntryStep.
         """
         return self.get_step(step) if isinstance(step, str) else step
 
     def __get_experiment_options(self) -> dict[str, str]:
         """
         Cache the experiment options if they haven't been cached yet.
+
         :return: The options for this experiment.
         """
         if hasattr(self, "_ExperimentHandler__exp_options"):
             return self.__exp_options
         self.__exp_options = self.__eln_man.get_notebook_experiment_options(self.__exp_id)
         return self.__exp_options
 
     def __get_step_options(self, step: Step) -> dict[str, str]:
         """
         Cache the options for the input step if they haven't been cached yet.
+
         :return: The entry options for the input step.
         """
         step = self.__to_eln_step(step)
         if step in self.__step_options:
             return self.__step_options.get(step)
         options: dict[str, str] = step.get_options()
         self.__step_options.update({step: options})
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/files/file_bridge.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class FileBridge:
     @staticmethod
     def read_file(context: SapioWebhookContext, bridge_name: str, file_path: str, base64_decode: bool = True) -> bytes:
         """
         Read a file from FileBridge.
+
         :param context: The current webhook context.
         :param bridge_name: The name of the bridge to use.
         :param file_path: The path to read the file from.
         :param base64_decode: If true, base64 decode the file. Files are by default base64 encoded when retrieved from
             FileBridge.
         :return: The bytes of the file.
         """
@@ -31,14 +32,15 @@
             ret_val = base64.b64decode(response.content)
         return ret_val
 
     @staticmethod
     def write_file(context: SapioWebhookContext, bridge_name: str, file_path: str, file_data: bytes | str) -> None:
         """
         Write a file to FileBridge.
+
         :param context: The current webhook context.
         :param bridge_name: The name of the bridge to use.
         :param file_path: The path to write the file to. If a file already exists at the given path then the file is
             overwritten.
         :param file_data: A string or bytes of the file to be written.
         """
         sub_path = '/ext/filebridge/writeFile'
@@ -50,14 +52,15 @@
             response = context.user.post_data_stream(sub_path, params=params, data_stream=data_stream)
         context.user.raise_for_status(response)
 
     @staticmethod
     def list_directory(context: SapioWebhookContext, bridge_name: str, file_path: str | None = "") -> list[str]:
         """
         List the contents of a FileBridge directory.
+
         :param context: The current webhook context.
         :param bridge_name: The name of the bridge to use.
         :param file_path: The path to read the directory from.
         :return: A list of name of files and folders in the directory.
         """
         sub_path = '/ext/filebridge/listDirectory'
         params = {
@@ -70,14 +73,15 @@
         path_length = len(f"bridge://{bridge_name}/")
         return [urllib.parse.unquote(value[path_length:]) for value in response_body]
 
     @staticmethod
     def create_directory(context: SapioWebhookContext, bridge_name: str, file_path: str) -> None:
         """
         Create a new directory in FileBridge.
+
         :param context: The current webhook context.
         :param bridge_name: The name of the bridge to use.
         :param file_path: The path to create the directory at. If a directory already exists at the given path then an
             exception is raised.
         """
         sub_path = '/ext/filebridge/createDirectory'
         params = {
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/files/file_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/files/file_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,30 @@
     # FR-46097 - Add write file request shorthand functions to FileUtil.
     @staticmethod
     def write_file(file_name: str, file_bytes: bytes, *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Send a file to the client.
 
         The calling webhook must catch the WriteFileResult that the client will send back.
+
         :param file_name: The name of the file.
         :param file_bytes: The bytes of the file.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the write request as its client callback request.
         """
         return SapioWebhookResult(True, client_callback_request=WriteFileRequest(file_bytes, file_name,
                                                                                  request_context))
 
     @staticmethod
     def write_files(files: dict[str, bytes], *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Send a collection of files to the client.
 
         The calling webhook must catch the MultiFileResult that the client will send back.
+
         :param files: A dictionary of files names to file bytes.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the write request as its client callback request.
         """
         return SapioWebhookResult(True, client_callback_request=MultiFileRequest(files, request_context))
 
     @staticmethod
@@ -52,22 +54,23 @@
         """
         Request a single file from the user. This function handles the entire client callback interaction for the
         requesting of the file, including if the user cancels the file upload prompt.
 
         The first time this method is called in the course of an interaction with the client, it will return a webhook
         result containing the client callback to request the file. The second time it is called, it will return the
         file name and bytes from the callback result.
+
         :param context: The current webhook context.
         :param title: The title of the file prompt dialog.
         :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
             exception if an incorrect file extension is provided.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A tuple with the following elements.
             0 - A webhook result that contains a file prompt if this is the first interaction with this request.
-                May also contain a result that will terminate the client interaction if the user canceled the prompt.
+            May also contain a result that will terminate the client interaction if the user canceled the prompt.
             1 - The file name of the requested file if the user provided one.
             2 - The file bytes of the requested file if the user provided one.
         """
         client_callback = context.client_callback_result
         result_context: str | None = client_callback.callback_context_data if client_callback else None
         # If the user cancels, terminate the interaction.
         if client_callback is not None and client_callback.user_cancelled:
@@ -102,22 +105,23 @@
         """
         Request multiple files from the user. This function handles the entire client callback interaction for the
         requesting of the files, including if the user cancels the file upload prompt.
 
         The first time this method is called in the course of an interaction with the client, it will return a webhook
         result containing the client callback to request the files. The second time it is called, it will return each
         file name and bytes from the callback result.
+
         :param context: The current webhook context.
         :param title: The title of the file prompt dialog.
         :param exts: The allowable file extensions of the uploaded file. If blank, any file can be uploaded. Throws an
             exception if an incorrect file extension is provided.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A tuple with the following elements.
             0 - A webhook result that contains a file prompt if this is the first interaction with this request.
-                May also contain a result that will terminate the client interaction if the user canceled the prompt.
+            May also contain a result that will terminate the client interaction if the user canceled the prompt.
             1 - A dictionary that maps the file names to the file bytes for each provided file.
         """
         client_callback = context.client_callback_result
         result_context: str | None = client_callback.callback_context_data if client_callback else None
         # If the user cancels, terminate the interaction.
         if client_callback is not None and client_callback.user_cancelled:
             return SapioWebhookResult(True), None
@@ -144,14 +148,15 @@
         return None, result.files
 
     @staticmethod
     def __verify_file(file_path: str, file_bytes: bytes, allowed_extensions: list[str]):
         """
         Verify that the provided file was read (i.e. the file path and file bytes aren't None or empty) and that it
         has the correct file extension. Raises a user error exception if something about the file is incorrect.
+
         :param file_path: The name of the file to verify.
         :param file_bytes: The bytes of the file to verify.
         :param allowed_extensions: The file extensions that the file path is allowed to have.
         """
         if file_path is None or len(file_path) == 0 or file_bytes is None or len(file_bytes) == 0:
             raise SapioUserErrorException("Empty file provided or file unable to be read.")
         if len(allowed_extensions) != 0:
@@ -166,14 +171,15 @@
 
     @staticmethod
     def tokenize_csv(file_bytes: bytes, required_headers: list[str] | None = None, header_row_index: int | None = 0) \
             -> tuple[list[dict[str, str]], list[list[str]]]:
         """
         Tokenize a CSV file. The provided file must be uniform. That is, if row 1 has 10 cells, all the rows in the file
         must have 10 cells. Otherwise, the Pandas parser throws a tokenizer exception.
+
         :param file_bytes: The bytes of the CSV to be parsed.
         :param required_headers: The headers that must be present in the file. If a provided header is missing, raises
             a user error exception.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
@@ -191,14 +197,15 @@
         return rows, metadata
 
     @staticmethod
     def tokenize_xlsx(file_bytes: bytes, required_headers: list[str] | None = None, header_row_index: int | None = 0) \
             -> tuple[list[dict[str, str]], list[list[str]]]:
         """
         Tokenize an XLSX file row by row.
+
         :param file_bytes: The bytes of the XLSX to be parsed.
         :param required_headers: The headers that must be present in the file. If a provided header is missing, raises
             a user error exception.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
@@ -217,14 +224,15 @@
 
     @staticmethod
     def csv_to_data_frames(file_bytes: bytes, header_row_index: int | None = 0) \
             -> tuple[DataFrame, DataFrame | None]:
         """
         Parse the file bytes for a CSV into DataFrames. The provided file must be uniform. That is, if row 1 has 10
         cells, all the rows in the file must have 10 cells. Otherwise, the Pandas parser throws a tokenizer exception.
+
         :param file_bytes: The bytes of the CSV to be parsed.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
         :return: A tuple of two DataFrames. The first is the frame for the CSV table body, while the second is for the
             metadata from above the header row, or None if there is no metadata.
@@ -248,14 +256,15 @@
         return file_body, file_metadata
 
     @staticmethod
     def xlsx_to_data_frames(file_bytes: bytes, header_row_index: int | None = 0) \
             -> tuple[DataFrame, DataFrame | None]:
         """
         Parse the file bytes for an XLSX into DataFrames.
+
         :param file_bytes: The bytes of the XLSX to be parsed.
         :param header_row_index: The row index in the file that the headers are located at. Everything above the header
             row is returned in the metadata list. If input is None, then no row is considered to be the header row,
             meaning that required headers are also ignored if any are provided. By default, the first row (0th index)
             is assumed to be the header row.
         :return: A tuple of two DataFrames. The first is the frame for the XLSX table body, while the second is for the
             metadata from above the header row, or None if there is no metadata.
@@ -276,14 +285,15 @@
         return file_body, file_metadata
 
     @staticmethod
     def data_frame_to_lists(data_frame: DataFrame) -> list[list[str]]:
         """
         Parse a Pandas DataFrame to a list of lists. Each outer list is a row, while each inner list is the cells
         for that row.
+
         :param data_frame: The DataFrame to be parsed.
         :return: The input DataFrame parsed into a row-wise list of lists.
         """
         if data_frame is None:
             return []
         # DataFrames are oriented column-wise instead of row-wise. Read down each column before moving to the next.
         rows: list[list[str]] = []
@@ -306,14 +316,15 @@
                             required_headers: list[str] = None,
                             header_row_index: int | None = 0) -> list[dict[str, str]]:
         """
         Parse a Pandas DataFrame to a list of dicts. Each list is a row, while each dict is the cells from that row
         keyed by the column header that the cell is under. Capable of requiring that certain headers are present.
 
         The names of the data_frame.columns values are expected to be the header names.
+
         :param data_frame: The DataFrame to be parsed.
         :param required_headers: The headers that must be present in the DataFrame. If a header is missing, raises an
             exception. If no headers are provided, doesn't do any enforcement.
         :param header_row_index: The row index in the file that the headers are located at. Only used ot tell the
             user where the headers are expected to be if a required header is not found, given that the input DataFrame
             was created from a parsed file.
         :return: The input DataFrame parsed into a row-wise list of dicts.
@@ -347,14 +358,15 @@
 
         return rows
 
     @staticmethod
     def csv_to_xlsx(file_data: bytes | str) -> bytes:
         """
         Convert a CSV file into an XLSX file.
+
         :param file_data: The CSV file to be converted.
         :return: The bytes of the CSV file converted to an XLSX file.
         """
         with (io.BytesIO(file_data) if isinstance(file_data, bytes) else io.StringIO(file_data)) as csv:
             # Setting header to false makes pandas read the CSV as-is.
             data_frame = pandas.read_csv(csv, sep=",", header=None)
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/aliases.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from collections.abc import Iterable
 from typing import Any
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedRecordModel, WrappedType
 
-# Different forms that a record model could take.
 RecordModel = PyRecordModel | WrappedRecordModel | WrappedType
-# A record could be provided as either a DataRecord, PyRecordModel, or WrappedRecordModel (WrappedType).
+"""Different forms that a record model could take."""
 SapioRecord = DataRecord | RecordModel
+"""A record could be provided as either a DataRecord, PyRecordModel, or WrappedRecordModel (WrappedType)."""
+RecordIdentifier = SapioRecord | int
+"""A RecordIdentifier is either a record type or an integer for the record's record ID."""
 
 
 # FR-46064 - Initial port of PyWebhookUtils to sapiopycommons.
 class AliasUtil:
     @staticmethod
     def to_data_record(record: SapioRecord) -> DataRecord:
         """
-        Convert a single DataRecord, PyRecordModel, or WrappedRecordModel to just a DataRecord
+        Convert a single DataRecord, PyRecordModel, or WrappedRecordModel to just a DataRecord.
+
         :return: The DataRecord of the input SapioRecord.
         """
         return record if isinstance(record, DataRecord) else record.get_data_record()
 
     @staticmethod
     def to_data_records(records: Iterable[SapioRecord]) -> list[DataRecord]:
         """
         Convert a list of variables that could either be DataRecords, PyRecordModels,
         or WrappedRecordModels to just DataRecords.
+
         :return: A list of DataRecords for the input records.
         """
         return [(x if isinstance(x, DataRecord) else x.get_data_record()) for x in records]
 
     @staticmethod
-    def to_record_ids(records: Iterable[int | SapioRecord]) -> list[int]:
+    def to_record_ids(records: Iterable[RecordIdentifier]) -> list[int]:
         """
         Convert a list of variables that could either be integers, DataRecords, PyRecordModels,
         or WrappedRecordModels to just integers (taking the record ID from the records).
+
         :return: A list of record IDs for the input records.
         """
         return [(x if isinstance(x, int) else x.record_id) for x in records]
 
     @staticmethod
     def to_field_map_lists(records: Iterable[SapioRecord]) -> list[dict[str, Any]]:
         """
         Convert a list of variables that could either be DataRecords, PyRecordModels,
         or WrappedRecordModels to a list of their field maps.
+
         :return: A list of field maps for the input records.
         """
         field_map_list: list[dict[str, Any]] = []
         for record in records:
             if isinstance(record, DataRecord):
                 field_map_list.append(record.get_fields())
             else:
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/custom_report_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/custom_report_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def run_system_report(context: SapioWebhookContext,
                           report_name: str,
                           filters: dict[str, Iterable[Any]] | None = None,
                           page_limit: int | None = None) -> list[dict[str, Any]]:
         """
         Run a system report and return the results of that report as a list of dictionaries for the values of each
         column in each row.
+
         :param context: The current webhook context.
         :param report_name: The name of the system report to run.
         :param filters: If provided, filter the results of the report using the given mapping of headers to values to
             filter on. Only those headers that both the filters and the custom report share will take effect. That is,
             any filters that have a header name that isn't in the custom report will be ignored.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The results of the report listed row by row, mapping each cell to the header it is under. The header
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/exceptions.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/popup_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/popup_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,27 @@
                    column_positions: dict[str, tuple[int, int]] = None, data_type: str = "Default",
                    *, display_name: str | None = None, plural_display_name: str | None = None,
                    request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a basic form entry dialog.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display at the top of the form.
         :param fields: The definitions of the fields to display in the form. Fields will be displayed in the order they
             are provided in this list.
         :param values: Sets the default values of the fields.
         :param column_positions: If a tuple is provided for a field name, alters that field's column position and column
             span. (Field order is still determined by the fields list.)
         :param data_type: The data type name for the temporary data type that will be created for this form.
         :param display_name: The display name for the temporary data type. If not provided, defaults to the data type
             name.
         :param plural_display_name: The plural display name for the temporary data type. If not provided, defaults to
-            the plural display name + "s".
+            the display name + "s".
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         if display_name is None:
             display_name = data_type
         if plural_display_name is None:
             plural_display_name = display_name + "s"
@@ -73,14 +74,15 @@
                           column_positions: dict[str, tuple[int, int]] = None, editable: bool | None = True,
                           *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a basic form dialog for a record with displayed fields from the record data type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
+
         :param context: The current webhook context
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param fields: The data field names of the fields from the record to display in the form. Fields will be
             displayed in the order they are provided in this list.
         :param record: The record to display the values of.
         :param column_positions: If a tuple is provided for a field name, alters that field's column position and column
@@ -117,128 +119,135 @@
             builder.add_field(field_def, column, span)
         temp_type_def = builder.get_temporary_data_type()
         callback = FormEntryDialogRequest(title, msg, temp_type_def,
                                           callback_context_data=request_context)
         return SapioWebhookResult(True, client_callback_request=callback)
 
     @staticmethod
-    def string_field_popup(title: str, msg: str, field_name: str, default_value: str | None,
+    def string_field_popup(title: str, msg: str, field_name: str, default_value: str | None = None,
                            max_length: int | None = None, editable: bool = True, data_type: str = "Default",
                            *, display_name: str | None = None, plural_display_name: str | None = None,
                            request_context: str | None = None, **kwargs) -> SapioWebhookResult:
         """
         Create a form dialog with a single string field. May take additional parameters to be passed to the string field
         definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param field_name: The name and display name of the string field.
         :param default_value: The default value to place into the string field, if any.
         :param max_length: The max length of the string value. If not provided, uses the length of the default value.
             If neither this or a default value are not provided, defaults to 100 characters.
         :param editable: Whether the user may edit the contents of the string field.
         :param data_type: The data type name for the temporary data type that will be created for this form.
         :param display_name: The display name for the temporary data type. If not provided, defaults to the data type
             name.
         :param plural_display_name: The plural display name for the temporary data type. If not provided, defaults to
-            the plural display name + "s".
+            the display name + "s".
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         if max_length is None:
             max_length = len(default_value) if default_value else 100
         string_field = VeloxStringFieldDefinition(data_type, field_name, field_name, default_value=default_value,
                                                   max_length=max_length, editable=editable, **kwargs)
         return PopupUtil.form_popup(title, msg, [string_field], data_type=data_type, display_name=display_name,
                                     plural_display_name=plural_display_name, request_context=request_context)
 
     @staticmethod
     def integer_field_popup(title: str, msg: str, field_name: str, default_value: int = None, min_value: int = -10000,
-                            max_value: int = 10000, data_type: str = "Default",
+                            max_value: int = 10000, data_type: str = "Default", editable: bool = True,
                             *, display_name: str | None = None, plural_display_name: str | None = None,
                             request_context: str | None = None, **kwargs) -> SapioWebhookResult:
         """
         Create a form dialog with a single integer field. May take additional parameters to be passed to the integer
         field definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param field_name: The name and display name of the integer field.
         :param default_value: The default value to place into the integer field. If not provided, defaults to the 0 or
             the minimum value, whichever is higher.
         :param min_value: The minimum allowed value of the input.
         :param max_value: The maximum allowed value of the input.
         :param data_type: The data type name for the temporary data type that will be created for this form.
+        :param editable: Whether the user may edit the contents of the integer field.
         :param display_name: The display name for the temporary data type. If not provided, defaults to the data type
             name.
         :param plural_display_name: The plural display name for the temporary data type. If not provided, defaults to
-            the plural display name + "s".
+            the display name + "s".
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         if default_value is None:
             default_value = max(0, min_value)
         integer_field = VeloxIntegerFieldDefinition(data_type, field_name, field_name, default_value=default_value,
-                                                    min_value=min_value, max_value=max_value, **kwargs)
+                                                    min_value=min_value, max_value=max_value, editable=editable,
+                                                    **kwargs)
         return PopupUtil.form_popup(title, msg, [integer_field], data_type=data_type, display_name=display_name,
                                     plural_display_name=plural_display_name, request_context=request_context)
 
     @staticmethod
     def double_field_popup(title: str, msg: str, field_name: str, default_value: float = None,
                            min_value: float = -10000000, max_value: float = 100000000,
-                           data_type: str = "Default", *, display_name: str | None = None,
+                           data_type: str = "Default", editable: bool = True, *, display_name: str | None = None,
                            plural_display_name: str | None = None, request_context: str | None = None, **kwargs) \
             -> SapioWebhookResult:
         """
         Create a form dialog with a single double field. May take additional parameters to be passed to the double
         field definition.
 
         The calling webhook must catch the FormEntryDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param field_name: The name and display name of the double field.
         :param default_value: The default value to place into the double field. If not provided, defaults to the 0 or
             the minimum value, whichever is higher.
         :param min_value: The minimum allowed value of the input.
         :param max_value: The maximum allowed value of the input.
         :param data_type: The data type name for the temporary data type that will be created for this form.
+        :param editable: Whether the user may edit the contents of the double field.
         :param display_name: The display name for the temporary data type. If not provided, defaults to the data type
             name.
         :param plural_display_name: The plural display name for the temporary data type. If not provided, defaults to
-            the plural display name + "s".
+            the display name + "s".
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         if default_value is None:
             default_value = min_value
         double_field = VeloxDoubleFieldDefinition(data_type, field_name, field_name, default_value=default_value,
-                                                  min_value=min_value, max_value=max_value, **kwargs)
+                                                  min_value=min_value, max_value=max_value, editable=editable, **kwargs)
         return PopupUtil.form_popup(title, msg, [double_field], data_type=data_type, display_name=display_name,
                                     plural_display_name=plural_display_name, request_context=request_context)
 
     @staticmethod
     def table_popup(title: str, msg: str, fields: list[AbstractVeloxFieldDefinition], values: list[dict[str, Any]],
                     *, data_type: str = "Default", display_name: str | None = None,
                     plural_display_name: str | None = None, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a basic table entry dialog.
 
-        The calling webhook must catch the FormEntryDialogResult that the client will send back.
+        The calling webhook must catch the TableEntryDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display at the top of the form.
         :param fields: The definitions of the fields to display as table columns. Fields will be displayed in the order
             they are provided in this list.
         :param values: The values to set for each row of the table.
         :param data_type: The data type name for the temporary data type that will be created for this table.
         :param display_name: The display name for the temporary data type. If not provided, defaults to the data type
             name.
         :param plural_display_name: The plural display name for the temporary data type. If not provided, defaults to
-            the plural display name + "s".
+            the display name + "s".
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         if display_name is None:
             display_name = data_type
         if plural_display_name is None:
             plural_display_name = display_name + "s"
@@ -255,14 +264,15 @@
                            title: str, msg: str, fields: list[str], records: list[SapioRecord],
                            editable: bool | None = True, *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a table dialog for a list of record where the columns are specific fields from the record data type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the TableEntryDialogResult that the client will send back.
+
         :param context: The current webhook context
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param records: The records to display as rows in the table.
         :param fields: The names of the fields to display as columns in the table. Fields will be displayed in the order
             they are provided in this list.
         :param editable: If true, all fields are displayed as editable. If false, all fields are displayed as
@@ -306,14 +316,15 @@
                                *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a record selection dialog for a list of record where the columns are specific fields from the record data
         type.
 
         Makes webservice calls to get the data field and type definitions of the given data type.
         The calling webhook must catch the DataRecordSelectionResult that the client will send back.
+
         :param context: The current webhook context
         :param msg: The message to display in the dialog.
         :param records: The records to display as rows in the table.
         :param fields: The names of the fields to display as columns in the table. Fields will be displayed in the order
             they are provided in this list.
         :param multi_select: Whether the user is able to select multiple records from the list.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
@@ -350,14 +361,15 @@
     @staticmethod
     def list_popup(title: str, options: list[str], multi_select: bool = False,
                    *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create a list dialog with the given options for the user to choose from.
 
         The calling webhook must catch the ListDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param options: The list options that the user has to choose from.
         :param multi_select: Whether the user is able to select multiple options from the list.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
         """
         callback = ListDialogRequest(title, multi_select, options,
@@ -367,14 +379,15 @@
     @staticmethod
     def option_popup(title: str, msg: str, options: list[str], default_option: int = 0, user_can_cancel: bool = False,
                      *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create an option dialog with the given options for the user to choose from.
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param options: The button options that the user has to choose from.
         :param default_option: The index of the option in the options list that defaults as the first choice.
         :param user_can_cancel: True if the user is able to click the X to close the dialog, returning
             user_cancelled = True in the client callback result. False if the user cannot close the dialog without
             selecting an option.
@@ -388,14 +401,15 @@
     @staticmethod
     def ok_popup(title: str, msg: str, user_can_cancel: bool = False, *, request_context: str | None = None) \
             -> SapioWebhookResult:
         """
         Create an option dialog where the only option is "OK".
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param user_can_cancel: True if the user is able to click the X to close the dialog, returning
             user_cancelled = True in the client callback result. False if the user cannot close the dialog without
             selecting an option.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
         :return: A SapioWebhookResult with the popup as its client callback request.
@@ -405,14 +419,15 @@
     @staticmethod
     def yes_no_popup(title: str, msg: str, default_yes: bool = True, user_can_cancel: bool = False,
                      *, request_context: str | None = None) -> SapioWebhookResult:
         """
         Create an option dialog where the only options are "Yes" and "No".
 
         The calling webhook must catch the OptionDialogResult that the client will send back.
+
         :param title: The title of the dialog.
         :param msg: The message to display in the dialog.
         :param default_yes: If true, "Yes" is the default choice. Otherwise, the default choice is "No".
         :param user_can_cancel: True if the user is able to click the X to close the dialog, returning
             user_cancelled = True in the client callback result. False if the user cannot close the dialog without
             selecting an option.
         :param request_context: Context that will be returned to the webhook server in the client callback result.
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/general/time_util.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/general/time_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,36 +31,43 @@
         global __timezone
         return __timezone
 
     @staticmethod
     def set_default_timezone(new_timezone: str | int) -> None:
         """
         Set the timezone used by TimeUtil to something new.
+
         :param new_timezone: The timezone to set the default to. A list of valid timezones can be found at
             https://en.wikipedia.org/wiki/List_of_tz_database_time_zones. May also accept a UTC offset in seconds.
         """
         global __timezone
         __timezone = TimeUtil.__to_tz(new_timezone)
 
     @staticmethod
     def __to_tz(timezone: str | int = None):
         """
         :param timezone: Either the name of a timezone, a UTC offset in seconds, or None if the default should be used.
         :return: The timezone object to use for the given input. If the input is None, uses the default timezone.
         """
         if isinstance(timezone, str):
-            return pytz.timezone(timezone)
-        elif isinstance(timezone, int):
+            # PR-46571: Convert timezones to a UTC offset and then use that offset as the timezone. This is necessary
+            # because pytz may return timezones from strings in Local Mean Time instead of a timezone with a UTC offset.
+            # LMT may be a few minutes off of the actual time in that timezone right now.
+            # https://stackoverflow.com/questions/35462876
+            offset: int = int(datetime.now(pytz.timezone(timezone)).utcoffset().total_seconds() / 60)
+            return pytz.FixedOffset(offset)
+        if isinstance(timezone, int):
             return pytz.FixedOffset(timezone // 60)
         return TimeUtil.get_default_timezone()
 
     @staticmethod
     def current_time(timezone: str | int = None) -> datetime:
         """
         The current time as a datetime object.
+
         :param timezone: The timezone to initialize the current time with. If no timezone is provided, uses the global
             timezone variable set by the TimeUtil. A list of valid timezones can be found at
             https://en.wikipedia.org/wiki/List_of_tz_database_time_zones. May also accept a UTC offset in seconds.
         """
         tz = TimeUtil.__to_tz(timezone)
         return datetime.now(tz)
 
@@ -71,40 +78,43 @@
         """
         return round(time.time() * 1000)
 
     @staticmethod
     def now_in_format(time_format: str, timezone: str | int = None) -> str:
         """
         The current time in some date format.
+
         :param time_format: The format to display the current time in. Documentation for how the time formatting works
             can be found at https://docs.python.org/3.10/library/datetime.html#strftime-and-strptime-behavior
         :param timezone: The timezone to initialize the current time with. If no timezone is provided, uses the global
             timezone variable set by the TimeUtil. A list of valid timezones can be found at
             https://en.wikipedia.org/wiki/List_of_tz_database_time_zones. May also accept a UTC offset in seconds.
         """
         return TimeUtil.current_time(timezone).strftime(time_format)
 
     @staticmethod
     def millis_to_format(millis: int, time_format: str, timezone: str | int = None) -> str:
         """
         Convert the input time in milliseconds to the provided format.
+
         :param millis: The time in milliseconds to convert from.
         :param time_format: The format to display the input time in. Documentation for how the time formatting works
             can be found at https://docs.python.org/3.10/library/datetime.html#strftime-and-strptime-behavior
         :param timezone: The timezone to initialize the current time with. If no timezone is provided, uses the global
             timezone variable set by the TimeUtil. A list of valid timezones can be found at
             https://en.wikipedia.org/wiki/List_of_tz_database_time_zones. May also accept a UTC offset in seconds.
         """
         tz = TimeUtil.__to_tz(timezone)
         return datetime.fromtimestamp(millis / 1000, tz).strftime(time_format)
 
     @staticmethod
     def format_to_millis(time_point: str, time_format: str, timezone: str | int = None) -> int:
         """
         Convert the input time from the provided format to milliseconds.
+
         :param time_point: The time in some date/time format to convert from.
         :param time_format: The format that the time_point is in. Documentation for how the time formatting works
             can be found at https://docs.python.org/3.10/library/datetime.html#strftime-and-strptime-behavior
         :param timezone: The timezone to initialize the current time with. If no timezone is provided, uses the global
             timezone variable set by the TimeUtil. A list of valid timezones can be found at
             https://en.wikipedia.org/wiki/List_of_tz_database_time_zones. May also accept a UTC offset in seconds.
         """
@@ -112,14 +122,15 @@
         return int(datetime.strptime(time_point, time_format).replace(tzinfo=tz).timestamp() * 1000)
 
     # FR-46154: Create a function that determines if a string matches a time format.
     @staticmethod
     def str_matches_format(time_point: str, time_format: str) -> bool:
         """
         Determine if the given string is recognized as a valid time in the given format.
+
         :param time_point: The time in some date/time format to check.
         :param time_format: The format that the time_point should be in. Documentation for how the time formatting works
             can be found at https://docs.python.org/3.10/library/datetime.html#strftime-and-strptime-behavior
         """
         try:
             # If this function successfully runs, then the time_point matches the time_format.
             TimeUtil.format_to_millis(time_point, time_format, "UTC")
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/recordmodel/record_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/recordmodel/record_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,34 +36,37 @@
         self.rec_man = RecordModelManager(context.user)
         self.inst_man = self.rec_man.instance_manager
         self.rel_man = self.rec_man.relationship_manager
 
     def wrap_model(self, record: DataRecord, wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Shorthand for adding a single data record as a record model.
+
         :param record: The data record to wrap.
         :param wrapper_type: The record model wrapper to use.
         :return: The record model for the input.
         """
         return self.inst_man.add_existing_record_of_type(record, wrapper_type)
 
     def wrap_models(self, records: Iterable[DataRecord], wrapper_type: type[WrappedType]) -> list[WrappedType]:
         """
         Shorthand for adding a list of data records as record models.
+
         :param records: The data records to wrap.
         :param wrapper_type: The record model wrapper to use.
         :return: The record models for the input.
         """
         return self.inst_man.add_existing_records_of_type(list(records), wrapper_type)
 
     def query_models(self, wrapper_type: type[WrappedType], field: str, value_list: Iterable[Any],
                      page_limit: int | None = None) -> list[WrappedType]:
         """
         Shorthand for using the data record manager to query for a list of data records by field value
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param field: The field to query on.
         :param value_list: The values of the field to query on.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The record models for the queried records.
         """
         return self.query_models_with_criteria(wrapper_type, field, value_list, None, page_limit)[0]
@@ -71,14 +74,15 @@
     def query_models_with_criteria(self, wrapper_type: type[WrappedType], field: str, value_list: Iterable[Any],
                                    paging_criteria: DataRecordPojoPageCriteria | None = None,
                                    page_limit: int | None = None) \
             -> tuple[list[WrappedType], DataRecordPojoPageCriteria]:
         """
         Shorthand for using the data record manager to query for a list of data records by field value
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param field: The field to query on.
         :param value_list: The values of the field to query on.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
@@ -88,28 +92,30 @@
         return self.wrap_models(records, wrapper_type), paging_criteria
 
     def query_models_by_id(self, wrapper_type: type[WrappedType], ids: Iterable[int],
                            page_limit: int | None = None) -> list[WrappedType]:
         """
         Shorthand for using the data record manager to query for a list of data records by record ID
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param ids: The list of record IDs to query.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The record models for the queried records.
         """
         return self.query_models_by_id_with_criteria(wrapper_type, ids, None, page_limit)[0]
 
     def query_models_by_id_with_criteria(self, wrapper_type: type[WrappedType], ids: Iterable[int],
                                          paging_criteria: DataRecordPojoPageCriteria | None = None,
                                          page_limit: int | None = None) \
             -> tuple[list[WrappedType], DataRecordPojoPageCriteria]:
         """
         Shorthand for using the data record manager to query for a list of data records by record ID
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param ids: The list of record IDs to query.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
         """
@@ -117,27 +123,29 @@
         records, paging_criteria = self.__exhaust_query_id_pages(dt, list(ids), paging_criteria, page_limit)
         return self.wrap_models(records, wrapper_type), paging_criteria
 
     def query_all_models(self, wrapper_type: type[WrappedType], page_limit: int | None = None) -> list[WrappedType]:
         """
         Shorthand for using the data record manager to query for all data records of a given type
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The record models for the queried records.
         """
         return self.query_all_models_with_criteria(wrapper_type, None, page_limit)[0]
 
     def query_all_models_with_criteria(self, wrapper_type: type[WrappedType],
                                        paging_criteria: DataRecordPojoPageCriteria | None = None,
                                        page_limit: int | None = None) \
             -> tuple[list[WrappedType], DataRecordPojoPageCriteria]:
         """
         Shorthand for using the data record manager to query for all data records of a given type
         and then converting the results into a list of record models.
+
         :param wrapper_type: The record model wrapper to use.
         :param paging_criteria: The paging criteria to start the query with.
         :param page_limit: The maximum number of pages to query from the starting criteria. If None, exhausts all
             possible pages.
         :return: The record models for the queried records and the final paging criteria.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
@@ -149,14 +157,15 @@
                                filters: dict[str, Iterable[Any]] | None = None,
                                page_limit: int | None = None) -> list[WrappedType]:
         """
         Run a system report that contains a RecordId column and query for the records with those IDs.
         First runs the custom report, then runs a data record manager query on the results of the custom report.
 
         Will throw an exception if the given system report does not have a RecordId column.
+
         :param wrapper_type: The record model wrapper to use.
         :param report_name: The name of the system report to run.
         :param filters: If provided, filter the results of the report using the given mapping of headers to values to
             filter on. This filtering is done before the records are queried.
         :param page_limit: The maximum number of pages to query. If None, exhausts all possible pages.
         :return: The record models for the queried records.
         """
@@ -164,32 +173,35 @@
         # Using the bracket operators because we want to throw an exception if RecordId doesn't exist in the report.
         ids: list[int] = [row["RecordId"] for row in results]
         return self.query_models_by_id(wrapper_type, ids)
 
     def add_model(self, wrapper_type: type[WrappedType]) -> WrappedType:
         """
         Shorthand for using the instance manager to add a new record model of the given type.
+
         :param wrapper_type: The record model wrapper to use.
         :return: The newly added record model.
         """
         return self.inst_man.add_new_record_of_type(wrapper_type)
 
     def add_models(self, wrapper_type: type[WrappedType], num: int) -> list[WrappedType]:
         """
         Shorthand for using the instance manager to add new record models of the given type.
+
         :param wrapper_type: The record model wrapper to use.
         :param num: The number of models to create.
         :return: The newly added record models.
         """
         return self.inst_man.add_new_records_of_type(num, wrapper_type)
 
     def add_models_with_data(self, wrapper_type: type[WrappedType], fields: list[dict[str, Any]]) -> list[WrappedType]:
         """
         Shorthand for using the instance manager to add new models of the given type, and then initializing all those
         models with the given fields.
+
         :param wrapper_type: The record model wrapper to use.
         :param fields: A list of field maps to initialize the record models with.
         :return: The newly added record models with the provided fields set. The records will be in the same order as
             the fields in the fields list.
         """
         models: list[WrappedType] = self.add_models(wrapper_type, len(fields))
         for model, field in zip(models, fields):
@@ -198,14 +210,15 @@
 
     def create_models(self, wrapper_type: type[WrappedType], num: int) -> list[WrappedType]:
         """
         Shorthand for creating new records via the data record manager and then returning them as wrapped
         record models. Useful in cases where your record model needs to have a valid record ID.
 
         Makes a webservice call to create the data records.
+
         :param wrapper_type: The record model wrapper to use.
         :param num: The number of new records to create.
         :return: The newly created record models.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.wrap_models(self.dr_man.add_data_records(dt, num), wrapper_type)
 
@@ -213,14 +226,15 @@
             -> list[WrappedType]:
         """
         Shorthand for creating new records via the data record manager with field data to initialize the records with
         and then returning them as wrapped record models. Useful in cases where your record model needs to have a valid
         record ID.
 
         Makes a webservice call to create the data records.
+
         :param wrapper_type: The record model wrapper to use.
         :param fields: The field map list to initialize the new data records with.
         :return: The newly created record models.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.wrap_models(self.dr_man.add_data_records_with_data(dt, fields), wrapper_type)
 
@@ -232,14 +246,15 @@
         throws an exception.
 
         The record is searched for using the primary identifier field name and value. If multiple records are returned
         by the query on this primary identifier, then the secondary identifiers are used to filter the results.
 
         Makes a webservice call to query for the existing record. Makes an additional webservice call if the record
         needs to be created.
+
         :param wrapper_type: The record model wrapper to use.
         :param primary_identifier: The data field name of the field to search on.
         :param id_value: The value of the identifying field to search for.
         :param secondary_identifiers: Optional fields used to filter the records that are returned after searching on
             the primary identifier.
         :return: The record model with the identifying field value, either pulled from the system or newly created.
         """
@@ -276,28 +291,30 @@
         secondary_identifiers.update({primary_identifier: id_value})
         return self.create_models_with_data(wrapper_type, [secondary_identifiers])[0]
 
     @staticmethod
     def map_to_parent(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
         """
         Map a list of record models to a single parent of a given type. The parents must already be loaded.
+
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parent.
         :return: A dict[ModelType, ParentType]. If an input model doesn't have a parent of the given parent type, then
             it will map to None.
         """
         return_dict: dict[RecordModel, WrappedType] = {}
         for model in models:
             return_dict[model] = model.get_parent_of_type(parent_type)
         return return_dict
 
     @staticmethod
     def map_to_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
         """
         Map a list of record models to a list parents of a given type. The parents must already be loaded.
+
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parents.
         :return: A dict[ModelType, list[ParentType]]. If an input model doesn't have a parent of the given parent type,
             then it will map to an empty list.
         """
         return_dict: dict[RecordModel, list[WrappedType]] = {}
         for model in models:
@@ -305,14 +322,15 @@
         return return_dict
 
     @staticmethod
     def map_by_parents(models: Iterable[RecordModel], parent_type: type[WrappedType]) -> dict:
         """
         Take a list of record models and map them by their parents. Essentially an inversion of map_to_parents. Input
         models that share a parent will end up in the same list. The parents must already be loaded.
+
         :param models: A list of record models.
         :param parent_type: The record model wrapper of the parents.
         :return: A dict[ParentType, list[ModelType]]. If an input model doesn't have a parent of the given parent type,
             then it will not be in the resulting dictionary.
         """
         to_parents: dict[RecordModel, list[WrappedType]] = RecordHandler.map_to_parents(models, parent_type)
         by_parents: dict[WrappedType, list[RecordModel]] = {}
@@ -321,28 +339,30 @@
                 by_parents.setdefault(parent, []).append(record)
         return by_parents
 
     @staticmethod
     def map_to_child(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
         """
         Map a list of record models to a single child of a given type. The children must already be loaded.
+
         :param models: A list of record models.
         :param child_type: The record model wrapper of the child.
         :return: A dict[ModelType, ChildType]. If an input model doesn't have a child of the given child type, then
             it will map to None.
         """
         return_dict: dict[RecordModel, WrappedType] = {}
         for model in models:
             return_dict[model] = model.get_child_of_type(child_type)
         return return_dict
 
     @staticmethod
     def map_to_children(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
         """
         Map a list of record models to a list children of a given type. The children must already be loaded.
+
         :param models: A list of record models.
         :param child_type: The record model wrapper of the children.
         :return: A dict[ModelType, list[ChildType]]. If an input model doesn't have children of the given child type,
             then it will map to an empty list.
         """
         return_dict: dict[RecordModel, list[WrappedType]] = {}
         for model in models:
@@ -350,14 +370,15 @@
         return return_dict
 
     @staticmethod
     def map_by_children(models: Iterable[RecordModel], child_type: type[WrappedType]) -> dict:
         """
         Take a list of record models and map them by their children. Essentially an inversion of map_to_children. Input
         models that share a child will end up in the same list. The children must already be loaded.
+
         :param models: A list of record models.
         :param child_type: The record model wrapper of the children.
         :return: A dict[ParentType, list[ModelType]]. If an input model doesn't have children of the given child type,
             then it will not be in the resulting dictionary.
         """
         to_children: dict[RecordModel, list[WrappedType]] = RecordHandler.map_to_children(models, child_type)
         by_children: dict[WrappedType, list[RecordModel]] = {}
@@ -366,27 +387,29 @@
                 by_children.setdefault(child, []).append(record)
         return by_children
 
     @staticmethod
     def map_by_id(models: Iterable[SapioRecord]) -> dict[int, SapioRecord]:
         """
         Map the given records their record IDs.
+
         :param models: The records to map.
         :return: A dict mapping the record ID to each record.
         """
         ret_dict: dict[int, SapioRecord] = {}
         for model in models:
             ret_dict.update({model.record_id: model})
         return ret_dict
 
     @staticmethod
     def map_by_field(models: Iterable[SapioRecord], field_name: str) -> dict[Any, list[SapioRecord]]:
         """
         Map the given records by one of their fields. If any two records share the same field value, they'll appear in
         the same value list.
+
         :param models: The records to map.
         :param field_name: The field name to map against.
         :return: A dict mapping field values to the records with that value.
         """
         ret_dict: dict[Any, list[SapioRecord]] = {}
         for model in models:
             val: Any = model.get_field_value(field_name)
@@ -394,14 +417,15 @@
         return ret_dict
 
     @staticmethod
     def map_by_unique_field(models: Iterable[SapioRecord], field_name: str) -> dict[Any, SapioRecord]:
         """
         Uniquely map the given records by one of their fields. If any two records share the same field value, throws
         an exception.
+
         :param models: The records to map.
         :param field_name: The field name to map against.
         :return: A dict mapping field values to the record with that value.
         """
         ret_dict: dict[Any, SapioRecord] = {}
         for model in models:
             val: Any = model.get_field_value(field_name)
@@ -411,52 +435,56 @@
         return ret_dict
 
     @staticmethod
     def sum_of_field(models: Iterable[SapioRecord], field_name: str) -> float:
         """
         Sum up the numeric value of a given field across all input models. Excepts that all given models have a value.
         If the field is an integer field, the value will be converted to a float.
+
         :param models: The models to calculate the sum of.
         :param field_name: The name of the numeric field to sum.
         :return: The sum of the field values for the collection of models.
         """
         field_sum: float = 0
         for model in models:
             field_sum += float(model.get_field_value(field_name))
         return field_sum
 
     @staticmethod
     def mean_of_field(models: Iterable[SapioRecord], field_name: str) -> float:
         """
         Calculate the mean of the numeric value of a given field across all input models. Excepts that all given models
         have a value. If the field is an integer field, the value will be converted to a float.
+
         :param models: The models to calculate the mean of.
         :param field_name: The name of the numeric field to mean.
         :return: The mean of the field values for the collection of models.
         """
         return RecordHandler.sum_of_field(models, field_name) / len(list(models))
 
     @staticmethod
     def get_newest_record(records: Iterable[SapioRecord]) -> SapioRecord:
         """
         Get the newest record from a list of records.
+
         :param records: The list of records.
         :return: The input record with the highest record ID. None if the input list is empty.
         """
         newest: SapioRecord | None = None
         for record in records:
             if newest is None or record.record_id > newest.record_id:
                 newest = record
         return newest
 
     @staticmethod
     def values_to_field_maps(field_name: str, values: Iterable[Any], existing_fields: list[dict[str, Any]] | None = None) \
             -> list[dict[str, Any]]:
         """
         Add a list of values for a specific field to a list of dictionaries pairing each value to that field name.
+
         :param field_name: The name of the field that the values are from.
         :param values: A list of field values.
         :param existing_fields: An optional existing fields map list to add the new values to. Values are added in the
           list in the same order that they appear. If no existing fields are provided, returns a new fields map list.
         :return: A fields map list that contains the given values mapped by the given field name.
         """
         # Update the existing fields map list if one is given.
@@ -475,14 +503,15 @@
     # output can be wrapped instead of requiring the user to wrap the output.
     def get_linear_path(self, models: Iterable[RecordModel], path: RelationshipPath, wrapper_type: type[WrappedType]) \
             -> dict[RecordModel, WrappedType | None]:
         """
         Given a relationship path, travel the path starting from the input models. Returns the record at the end of the
         path, if any. The hierarchy must be linear (1:1 relationship between data types at every step) and the
         relationship path must already be loaded.
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the record at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to None.
         """
         ret_dict: dict[RecordModel, WrappedType | None] = {}
@@ -501,14 +530,15 @@
 
     def get_branching_path(self, models: Iterable[RecordModel], path: RelationshipPath,
                            wrapper_type: type[WrappedType]) -> dict[RecordModel, list[WrappedType]]:
         """
         Given a relationship path, travel the path starting from the input models. Returns the record at the end of the
         path, if any. The hierarchy may be non-linear (1:Many relationships between data types are allowed) and the
         relationship path must already be loaded.
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the records at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to an empty list.
         """
         ret_dict: dict[RecordModel, list[WrappedType]] = {}
@@ -538,14 +568,15 @@
         Given a relationship path, travel the path starting from the input models. Returns the record at the end of the
         path, if any. The hierarchy may be non-linear (1:Many relationships between data types are allowed) and the
         relationship path must already be loaded.
 
         The path is "flattened" by only following the first record at each step. Useful for traversing 1-to-Many-to-1
         relationships (e.g. a sample with is aliquoted to a number of samples, then those aliquots are pooled back
         together into a single sample).
+
         :param models: A list of record models.
         :param path: The relationship path to follow.
         :param wrapper_type: The record model wrapper to use.
         :return: Each record model mapped to the record at the end of the path starting from itself. If the end of the
             path couldn't be reached, the record will map to None.
         """
         ret_dict: dict[RecordModel, WrappedType | None] = {}
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/rules/eln_rule_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/eln_rule_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,27 +69,29 @@
             self.__entry_to_records.update({entry: entry_dict})
 
     def get_records(self, data_type: str, entry: str | None = None) -> list[DataRecord]:
         """
         Get records from the cached context with the given data type. Capable of being filtered to searching within
         the context of an entry name. If the given data type or entry does not exist in the context,
         returns an empty list.
+
         :param data_type: The data type of the records to return.
         :param entry: The name of the entry to grab the records from. If None, returns the records that match the data
             type from every entry. If an entry is provided, but it does not exist in the context, returns an empty list.
         :return: The records from the context that match the input parameters.
         """
         records: dict[str, set[DataRecord]] = self.__entry_to_records.get(entry, {}) if entry else self.__records
         return list(records.get(data_type, []))
 
     def get_models(self, wrapper_type: type[WrappedType], entry: str | None = None) -> list[WrappedType]:
         """
         Get record models from the cached context with the given data type. Capable of being filtered to searching
         within the context of an entry name. If the given data type or entry does not exist in the context,
         returns an empty list.
+
         :param wrapper_type: The record model wrapper to use.
         :param entry: The name of the entry to grab the records from. If None, returns the records that match the data
             type from every entry. If an entry is provided, but it does not exist in the context, returns an empty list.
         :return: The record models from the context that match the input parameters.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.__inst_man.add_existing_records_of_type(self.get_records(dt, entry), wrapper_type)
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/rules/on_save_rule_handler.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/rules/on_save_rule_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,27 +69,29 @@
             self.__base_id_to_records.update({record_id: id_dict})
 
     def get_records(self, data_type: str, record_id: int | None = None) -> list[DataRecord]:
         """
         Get records from the cached context with the given data type. Capable of being filtered to searching within
         the context of a record ID. If the given data type or record ID does not exist in the context,
         returns an empty list.
+
         :param data_type: The data type of the records to return.
         :param record_id: The record ID of the base record to search from. If None, returns the records that match the
             data type from ID. If an ID is provided, but it does not exist in the context, returns an empty list.
         :return: The records from the context that match the input parameters.
         """
         records: dict[str, set[DataRecord]] = self.__base_id_to_records.get(record_id, {}) if record_id else self.__records
         return list(records.get(data_type, []))
 
     def get_models(self, wrapper_type: type[WrappedType], record_id: int | None = None) -> list[WrappedType]:
         """
         Get records from the cached context with the given data type. Capable of being filtered to searching within
         the context of a record ID. If the given data type or record ID does not exist in the context,
         returns an empty list.
+
         :param wrapper_type: The record model wrapper to use.
         :param record_id: The record ID of the base record to search from. If None, returns the records that match the
             data type from ID. If an ID is provided, but it does not exist in the context, returns an empty list.
         :return: The record models from the context that match the input parameters.
         """
         dt: str = wrapper_type.get_wrapper_data_type_name()
         return self.__inst_man.add_existing_records_of_type(self.get_records(dt, record_id), wrapper_type)
```

### Comparing `sapiopycommons-31.0.13.23.12/src/sapiopycommons/webhook/webhook_handlers.py` & `sapiopycommons-31.2.0.23.12.3/src/sapiopycommons/webhook/webhook_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,56 +70,60 @@
     # CR-46153: Make CommonsWebhookHandler exception handling more easily overridable by splitting them out of
     # the run method and into their own functions.
     def handle_exception_callback(self) -> SapioWebhookResult | None:
         """
         Handle any client callbacks made as the result of exceptions. Whether a result is from an exception is
         determined by reading the callback context data. Context data for exceptions should be something unique that
         no programmer would use in practice so that we don't accidentally handle callbacks we shouldn't.
+
         :return: A SapioWebhookResult for any handled exceptions. None if nothing was handled.
         """
         # Catch any SapioCriticalErrorException results.
         result = self.context.client_callback_result
         if result is not None:
             result_context = result.callback_context_data
             if isinstance(result, FormEntryDialogResult) and result_context == "SapioCriticalErrorException":
                 return SapioWebhookResult(False)
         return None
 
     def handle_user_error_exception(self, e: SapioUserErrorException) -> SapioWebhookResult:
         """
         Handle a SapioUserErrorException. Default behavior returns the error message as display text in a webhook
         result.
+
         :param e: The exception that was raised.
         :return: A SapioWebhookResult reporting the exception to the user.
         """
         result: SapioWebhookResult | None = self.handle_any_exception(e)
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
         return SapioWebhookResult(False, display_text=e.args[0])
 
     def handle_critical_error_exception(self, e: SapioCriticalErrorException) -> SapioWebhookResult:
         """
         Handle a SapioCriticalErrorException. Default behavior returns a FormEntryDialogRequest with an uneditable
         text entry containing the error message. This client callback for this request is handled by
         handle_exception_callback.
+
         :param e: The exception that was raised.
         :return: A SapioWebhookResult reporting the exception to the user.
         """
         result: SapioWebhookResult | None = self.handle_any_exception(e)
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
         return PopupUtil.string_field_popup("Error", "", "Reason", e.args[0],
                                             request_context="SapioCriticalErrorException", num_lines=10)
 
     def handle_unexpected_exception(self, e: Exception) -> SapioWebhookResult:
         """
         Handle a generic exception which isn't a SapioUserErrorException or SapioCriticalErrorException. Default
         behavior returns a generic error message as display text informing the user to contact Sapio support.
+
         :param e: The exception that was raised.
         :return: A SapioWebhookResult reporting the exception to the user.
         """
         result: SapioWebhookResult | None = self.handle_any_exception(e)
         if result is not None:
             return result
         self.log_error(traceback.format_exc())
@@ -127,14 +131,15 @@
                                                       "Please contact Sapio support.")
 
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
     def handle_any_exception(self, e: Exception) -> SapioWebhookResult | None:
         """
         An exception handler which runs regardless of the type of exception that was raised. Can be used to "rollback"
         the client if an error occurs. Default behavior does nothing and returns None.
+
         :param e: The exception that was raised.
         :return: An optional SapioWebhookResult. May return a custom message to the client that wouldn't have been
             sent by one of the normal exception handlers, or may return None if no result needs returned.
         """
         return None
 
     def log_info(self, msg: str) -> None:
```

