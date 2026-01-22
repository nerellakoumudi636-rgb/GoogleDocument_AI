 Automated Document Processing using Google Document AI

 Problem Statement

Organizations receive many documents such as Aadhaar cards, PAN cards, driving licenses, invoices, and employment forms. Manually reading and entering data from these documents is slow, time-consuming, and costly.

To solve this problem, Google Cloud Platform (GCP) **Document AI** is used. Document AI uses machine learning to automatically understand and extract information from documents.



 Overview of Google Document AI

Google Document AI helps automate document understanding by:

Reading text using OCR (Optical Character Recognition)
Detecting document structure
Extracting required fields automatically



 Steps to Use Document AI

1.Go to Google Cloud Console
2. In the search bar, type Document AI
3. Open Document AI and go to Processors
4. Create different processors based on document type

   * Aadhaar
   * PAN Card
   * Driving License
   * Invoice
   * Forms



1.Aadhaar Card Processing

 Processor Creation

 Create a Custom Extractor processor for Aadhaar
 Upload sample Aadhaar card documents

 Required Fields

Name
Date of Birth
Gender
Aadhaar Number

Training Process

 Manually label the required fields in sample documents
 After labeling, start the training process
 The model learns from the provided examples
 After training, the processor is automatically saved

 Extraction

Upload a new Aadhaar card
OCR reads the text
Trained processor identifies fields
Required data is extracted automatically



2. PAN Card Processing

 Processor Creation

Create a custom PAN Card Processor in Document AI
Upload sample PAN card images

Required Fields

 Name
 Father’s Name
 Date of Birth
PAN Number

Training and Usage

 Label all required fields manually
 Train the processor
 After training, the processor is saved automatically
 Upload a new PAN card
 PAN details are extracted accurately


3.Driving License Processing

Processor Creation

 Create a Driving License custom processor
 Upload sample driving license documents

Training Steps

 Label required fields during training
 Train the processor
 Processor is saved automatically after training

 Extraction

 Upload a new driving license
All required details are extracted automatically



4.Form Parser

 What is Form Parser?

Form Parser is used to extract data from structured forms where fields and layouts are mostly consistent.

 Example

Employment application form

Working

Upload the form into the Form Parser
Document AI automatically performs OCR
Detects text and form structure
Extracts field names and values



Automatic Detection

After uploading a document:

Document AI automatically performs OCR
Detects text, tables, and form structure



 Boundary Box Detection

 What are Boundary Boxes?

Boundary boxes are drawn around detected text
They show where each field is located in the document

Features

 Identifies fields and values
 Draws boxes around detected text
 Helps locate information like:

   Name
   Phone number
   Address
   Position field



 Field Mapping
 Text inside boundary boxes is mapped to predefined fields
 Ensures correct association between text and field names



Training and Learning

 During training, we manually confirm correct fields
 Over time, the processor learns automatically
 Accuracy improves with more samples



 Final Outcome

 No further manual work is required
 Upload documents directly
 Data is extracted automatically
 Processors are ready for real-time use
