# Release 2.5.2
- no changes compared to previous update (see Tag 2.5.2-Pre1)

# Release 2.5.2-Pre1
- added OPS and ICD10 codesystems (now available in fhir format)

- change 'validFrom' date to '01.07.2023' for researchDataSubmissionTracking.json

- added 'maxHistory' attribute (value = 10) in DiGA implementation guide

- added missing codes 175 - 178 in valueset author-specialilty

- added mimetype pdf in medical-image implementation guide (C_11241)

# Release 2.5.1-5
- update 'guidelineDefinitions' (including introduction of 'version') for several implementation_guidelines (editorial)

# Release 2.5.1-4
- removed doubled typecode section in ig-dentalrecord.json (remaining typecode section covers PATD and ABRE)

- new validFrom date = 2024-01-01 for ig-referral_v_1_0.json and ig-tele_med_v_1_0.json

- republish ig-DMP_rheuma_V_1.json with new validFrom date = 2023-04-01 to solve ambiguities with formatCode entries in vs-format-code.xml. This is a preliminary date and may be changed according to roadmap decisions!

# Release 2.5.1-3
- updated OIDs of 'Signature Type Codes' and 'Acquisition Modality Codes' with code system OID instead of value set OID (vs-event-code.xml)

- ig-dentalrecord.json with two typecodes and versioning for igs (ig-schema-definition.json)

- removed ig-dmp-rheuma.json - new validFrom date to be clarified (not available yet but not before 1.4.23))

# Release 2.5.1-2
Updated FDV OpenAPI Specification to include PseudomyseMio Operation

# Release 2.5.1-1
- deprecated marker for obsolete codes (vs-practice-setting-code.xml)

- additional optional entry in ig-schema-definition.json to identify implementation-guides of type 'implementationArtifact', first used in ig-medical-image.json

# Release 2.5.1
- changed description regarding proffessionOID source in policies for diga, hcp and insurance

- added new formatCode (dummy / proprietary) in ig for researchDataSubmissionTrackingList

- clarification date-time format for consentValidFrom in researchDataSubmissionTrackingList

- corrected KeyType (removed algorithm attribute) for ContextKey in KeyManagement.xsd

- modified testtreiber_fdv.yaml for researchDataSubmission testing

# Release UPD_20220711
- new example DiGA-Policy in src/samples

- removed doubled code 131001 FA Immunologie from vs-author-speciality.xml

# Release 2.5.1-CC
- changed class- and type code in several IG

- new implementation guide for 'Rheumatoide Arthritis'

- update cs-kdl.xml to 2022 version

- update vs-event-code.xml to latest kdl, ops and icd-10 code systems (C_11108)

- new attribute 'maxDocumentHistory' in ig-schema-definition.json (C_11123)

- Timestamp format in GetAuditEvents and GetSignedAuditEvents (C_11124)

- changed displayName eventCodeList in ig-dmp_cr_V_1.json

- metadata and valueset changes for researchDataTrackingList handling (C_11110)

- new implementation_guide ig-medical-image.json (C_11065)

- removed OKDate in finishKeyChangeResponse (C_11979)

- new element 'schema-version' for researchDataSubmissionTrackingList (C_11131)

- removed keyword format from tokenstructure in I_Authorization_Insurant.yaml (C_11136)

- removed OKDate from PutForReplacement and GetAllDocumentKeys (C_11066)

- maintenance: synchronization src/schema/ext with repo api-telematik/ext (import)

- new structure for DeidentificationDefinition in schema for implementation_guides (C_11158)

- removed documentCategory from all implementation-guides and ig-schema-definition (C_11109)

- added obsolete code for "Tierheilpraktiker" to value set

# Release 2.5.0-3
- corrections in scheme researchDataSubmissionTracking.json and related example document

- guideline_researchDataSubmissionTracking.adoc moved to 'docs' folder

# Release 2.5.0-2
- minor correction for mixed folders (berechtigungskonzept.adoc)  


- correction of "display" and extension "valueString" for some concepts according to SGB V § 341 vs-speciality-oth.xml)  


- correction of ig-files, considering the changes in vs-speciality-oth (implementation_guides)  


# Release 2.5.0-1
- clarification and explanation of folder visibility (berechtigungskonzept.adoc)  


- reintroduced outdated ig-prescription for reference  (ig-prescription.json)  


- several updates to value sets, including new codes for DMP, Telemonitoring and Referral (C_11058, C_11082) (vocabulary)  


- removed attribute 'unique' in all existing implementaion-guides (implementation_guides)  


- new ig for referral (care) and telemonitoring (implementation_guides)  


- moved sample for tracking list (example_TrackingList.json)  


- reduced DMP format codes to major/minor version only (vs-format-code.xml))  


- removed leading space in name elements of ig (ANFEPA_1944))(implementation_guides)  


- new example message for getAuthorizationState (samples: ePA 2 Beispielnachrichten PS - Konnektor)  


# Release 2.5.0
- added de-identification property for documents in implementation-guideline-scheme (ig-schema-definition.json)  


- introduced referencedIdList meta data for research data tracking list  (ig-researchDataSubmissionTracking.json)  


- several updates to value sets (vocabulary)  


- new code system DMP (KBV_CS_SFHIR_KBV_DMP_V1.05.xml  


- changed tracking of research data (removed submissionDocumentIdSet) (scheme researchDataSubmissionTrackingLIst.json)  


- corrected regex for UserAgents (AuthorizationService.xsd)  


- added several ig for DMP (implementation_guides)  


- corrected policy (C_11003) (hcp-policy-definition.xml)  


# Release 2.5.0-Pre1
- correction regex for UserAgents (missing escape character for '.') (AuthorizationService.xsd)  


# Release 2.5.0-CC
- Feature: Verarbeitung von Daten der ePA zu Forschungszwecken  


- Feature:  Anbindung digitaler Gesundheitsanwendungen an die ePA 


- (latest 2.1.1 changes) regex pattern for UserAgentType (AuthorizationService.xsd)  (C_11027)  


- (latest 2.1.1 changes) static folders on allow- or deny-lists (hcp-policy-definition.xml)  (C_11003)  


# Release 2.1.1-Pre1
- corrected AuthorizedIdList (KeyManagementService.xsd)  (C_10977)  


- corrected cardinality for Key in KeListType (KeyManagementService.xsd)  (C_10976)  


- corrected MIO versions in vs-foramt-code.xml 


- corrected SOAP-Action for consistence with specification (KeyManagementService.wsdl)  (C_11029)  


- added LastTimeStamp in getAuditEvenets and getSignedAuditEvents (AuthenticaionService.xsd, AuthorizationService.xsd, AccountManagementService.xsd) (C_11019) 


# Release MIO_20220216
- removed implementation guides for outdated mio version (prescription) 


- added format codes for eVerordnung (prescription 1.0.2) 


# Release MIO_20220211
- added implementation guides for new mio versions 


- changed json schema for implementation guides 


- updated implementation guides regarding to new schema 


- added new mios and "validfrom" date to value sets section 


# Release 2.1.0
- new samples for ePA 2 Request Facility Authorization  

- withdrawal of doubled folder association for parental notice (childsrecord and patientdoc) (C_10981) 


# Release 2.1.0-Pre1
- enable 'Paging' for GetSignedAuditEvents in AuthorizationService, AuthenticationService and AccountManagemnetService (C_10962)  


- add <AuditMessages> to healthcare-security-audit.xsd for validation improvement on export packages (Proto291.xml) (C_10890) 


# Release 2.0.6-Pre2
- introduce a fhir-ressource based on 'dummy' values. Shall be used as Practitioner (KBV_PR_MIO_CMR_Practitioner) in parental notices of a childs medical record V1.0.0 (C_10907) ' 


# Release 2.0.6-Pre1
- update 'Berechtigungskonzept' 

- added OID-based identifier (vocabulary) 

- explanation on colons (hcp-policy-dedfinition.xml) 

- new operation GetauthorizationState (AuthorizationService) 

- additional parameter 'AllMandators' in CheckRecordExists (AuthorizationService.xsd) 


# Release 2.0.5-2
- new folder "ePA 2 Beispielnachrichten PS - Konnektor" 


- sample messages ePA 2 


# Release 2.0.5-1
- changes from C_10932 (hcp-policy-definition.xml and hcp-policy-2.xml) 


- new folder "vocabulary" for code systems and value sets. 


- initial provision of code systems and value sets (draft) used with epa. 


- major update "berechtigungskonzept". Detailed clarifications on ePA1 to ePA2 migration issues 


# Release 2.0.5
- Bugfix SoapAction GetSignedAuditEvents (AccountManagementService.wsdl) 
- Bugfix parametertype in finishKeyChange (AuthorizationService.xsd) 
- Removed typeCode (C_10831) (ig-nfd.json)

# Release 2.0.4-3X
2.0.4-3X is an update to 2.0.4-3 without any change, except for the removal of 'as-wechsel'

# Release 2.0.4-3
changes since 2.0.4-2 
- Integrated SOAP-Interface PHR from api-telematik to api-epa 
- Moved reference implementation as-wechsel to separate repository ref-ePA_HealthRecordMigration 
- Corrections and clarifications (berechtigungskonzept.adoc)

# Release 2.0.4-2
changes since 2.0.4-1
- update berechtigungskonzept.adoc (add some informations to collections)
- update ig-prescription (delete folder description link to vaccination documentation)

# Release 2.0.4-1
changes since 2.0.4
 - correction in formatCode. Is now "Arbeitsunfaehigkeitsbescheinigung" (ig-eau.json)
 - correction in version. Is now 1.0.2 (device_management)

# Release 2.0.4
changes since 2.0.4-pre3 - fixed erroneous DTO for Remove permissionHcpo (testtreiber_fdv.yaml)
 - moved deviceID parameter to header, added new error reponse 412 (DeviceUnknown), removed not used error responses(device_management.yaml)
 - added pagination for protocol, removed in findObjects (testtreiber_fdv.yaml)
 - update comments (hcp-policy-definition.xml)
 - update categjory "psychotherapy" (C_10787, hcp-poliy-2.xml)
 - several fixes (testtreiber_fdv.yaml)

# Release 2.0.4-pre3
- update and bugfix(testtreiber_fdv.yaml)
 - clarifications Dokumentenspezifische Autorisierung (C_10773, berechtigungskonzept.adoc)
 - update reference implementation "Aktensystem Wechsel", now with Docker (as_wechsel)
 - additional comment for deleteDevice (device_management.yaml)

# Release 2.0.4-pre2
- correction DeviceNameType minLength (device_management.yaml)
 - corrections in delta-export-time description (readme in as-wechsel)

# Release 2.0.4-pre1
- replaced "mothersrecord" with "childsrecord" in collection "mixed"
 - added reference implementation "Aktensystem Wechsel"
 - C_10778: modified access rights for midwife refering DVPMG\ - C_10773 - created metadata definitions for structured documents (renamed folder mio to implementation_guides)
 - updated structure for supporting generic documents (not solely mios)

# Release 2.0.3-4
- MIO: Mio Versions updated
 - PS: update implementation guide for PS
 - API: bugfix type AuthenticationAssertion (device_management.yaml)

# Release 2.0.3-3
- API: fixed syntax bugs, added missing parameters to paths, renamed path parameters (device_management.yaml)
 - API: corrections in comments and version history (device_management.yaml)
 - SAMPLES: C_10750 - permit access to very restricted documents added on a whitelist
 - MIO: correction of document cardinality (mr-mio-definition.json)

# Release 2.0.3-2
- new MIO definitions
 - moved testdriver to api-ePA
 - namespace corrections for policies
 - editorial changes

# Release 2.0.3-1
 - Changes - minor changes in HCP policy definition and sample HCP policies (i.e. HL7 namespace fixed)

# Release 2.0.3
 - ePA 2.0.3 - Release Notes Changes - description for access management and policy definitions added - upgrade notes added - device management API added

# Release 1.1.3
 - ePA 1.1.3 - Release Notes Changes - sample IHE messages added - implemention notes added
 