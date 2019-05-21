## UgandaEMR 2.1.0 Release Notes
Currently work in progress 

### New Features

1. Patient Flags - these allow highlighting information on the patient dashboard following the traffic light coloring, green (good), orange (take note), red (take action). The summary of flags by color codes are:
   * Green - Upcoming Appointment, Due for First Viral Load, Due for Routine Viral Load, Due for 1st DNA PCR, Due for 2nd DNA PCR, Due for Rapid Test
   * Orange - Missed Appointment
   * Red - Overdue for First Viral Load, Overdue for Routine Viral Load, Lost, Lost to Followup, Overdue for 1st DNA PCR, Overdue for 2nd DNA PCR, Overdue for Rapid Test, Has Detectable Viral Load
   
2. Ability to disable some of the patient flags to improve performance 

2. Differentiated Service Model
   * All patients enrolled in HIV care are placed in the FBIM model 
   * During the data capture for an ART Encounter the model can be changed 
   * Only stable patients can be moved to community models 
   * The history of the patient's models is displayed on the patient's dashboard 
   * A report showing the current model for all patients has been added 

3. Patient Dashboard- added the following sections 
   * Summary from Last Visit - selected data elements from the last ART encounter 
   * Viral Load History - shows a history of viral load results  
   * Directions to address 
4. DTG regimens have been added to the ART Summary and Encounter pages  
5. Data tools 
   * Intensive Adherence Counselling (IAC) form 
   * ART Encounter Page - duration on ART and duration on current regimen are automatically computed
   
6. Reports
   * New Facility Reports - Due for Viral Load, Overdue for Viral Load, Transfer In, Transfer Out, Lost Clients, Lost to Followup, Active Clinets in Care, Non-Suppressed Viral Load, Patient Stability Assessment Report, and Patient DSDM Model Report 
   * New MER Indicator Reports - TX_CURR (for 30 days and 90 days), TX_NEW, TB STAT, TB ART, TX_TB, PMTCT STAT 
   * Early Warning Indicators - Lost to Follow-up, Pill Pickup and Viral Load Suppression 
   * Integration Data Exports - Family Connect EMTCT Module
   * Registers - HIV Exposed Infants Register
   * All reports can be exported as CSV
   
7. Updated address hierarchy on the patient registration page to match the current version in DHIS2 as of April 2019 

8. Improved performance by:
   * Removed chart search, Atlas modules 
   * Data Entry Statistics and FHIR modules are not started by default  

### Bug Fixes

1. Data quality violations were not removed when cleared 
2. ART Summary page would not save with date validations for Transfer In 
3. Added addresses to all patient level reports 
4. Corrected reports which had errors running 

### Links to download files

This release is a drop in WAR file upgrade for UgandaEMR 2.0.0, however upgrades from 1.x require the use of the upgrade installer due to changes in the Java version required from Java 7 to Java 8 

#### WAR File 

Link

#### New Installation

For new machines with no UgandaEMR installed

1. 32 bit installer (TBD) - 
2. 64 bit installer (TBD) -  

#### Upgrade Installer 

For existing versions of UgandaEMR 1.x 

1. 32 bit upgrade installer (TBD) - 
2. 64 bit upgrade installer (TBD) -  

### Noteable contributions 

We would like to recognize the noteable contribution of the following partners, and facilities in this release

1. Baylor and Rwenzori Region health facilties - feedback on facility level reports and field testing of DSDM modules 
2. MUJHU through Mulago and Kawempe Hospital facilities - ANC and Maternity data collection and reporting tools, especially the need to export reports as CSV format for further analysis 
3. Alive Medical Services and ISS Clinic Mulago - stress testing and continuous improvements to the patient clinician facing dashboard page 
