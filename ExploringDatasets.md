# CFDE Cloud Workspace Partnership (CWP) Pilot
## Exploring and Accessing Datasets

---
### Overview of Accessing Data in CAVATICA

There are a variety of data access tiers across different DCCs. These tiers span a range of open access to controlled access, with file management and access mechanisms ranging from DRS, https pointers to data files, to download / copy of actual files (e.g. FTP). We are matching up these existing tiers with different ways that CAVATICA can support a DCC to provision their data into a cloud workspace where a researcher can then begin their analysis.

![image](https://github.com/kids-first/cloud-workspace-partnership-pilot/assets/1084749/27b1f578-8722-48f7-95f5-de743e21aa71)

One of the commonly used methods for cloud data access is the Data Repository Service (DRS) API
- DRS is a set of standardized API calls so data consumers can “an access data in a single, standard way regardless of where it’s stored and how it’s managed”.  
- DRS can be utilized for both controlled access an open access data, but has become a core standard as part of NCPI for controlled access. 


---
### Controlled Access Data for Secondary Use
Users interested in data from DCCs who submit their data to dbGaP for controlled access can use the dbGaP DRS/RAS integration with CAVATICA

[dbGaP - Tips for Preparing a Successful Data Access Request](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/GetPdf.cgi?document_name=GeneralAAInstructions.pdf)

[![dbGaP: Apply for Controlled Access Data](https://img.youtube.com/vi/m0xp_cCO7kA/0.jpg)](https://www.youtube.com/watch?v=m0xp_cCO7kA)

---
### Consortium Controlled Access Data
Leveraging shared private workspaces for DCC hosted data will be the preferred option for prototyping successful analysis during the pilot. Hosting own DRS server will need integration with CAVATICA for authentication/authorization.

---
### Open Access Data
There are a number of options for users to access open data from DCCs
- Open DRS server managed by DCC
- Use CAVATICA DRS services once DCC has indexed their data on CAVATICA DRS server
- Access non-DRS sources such as open access cloud storage (including AWS Open Data)

---
### Bring Your Own Data

You can upload your private data to CAVATICA using any of the following file transfer methods to suit your various requirements and achieve the best upload speed and reliability for the volume and structure of data that you are uploading.

#### Upload from your local storage 

##### Upload directly through CAVATICA's visual interface

The easiest and most intuitive way of uploading files to CAVATICA is to use the integrated upload functionality. This allows you to browse and select files from your local storage and upload them directly, without using additional tools or services. This upload method is most convenient and demonstrates best performance for small-scale uploads.

##### Upload using the Command-line (CLI) Uploader

If you have a larger volume of data on your local machine or cluster and want to upload it to CAVATICA (store it in CAVATICA storage), use the [Command-line (CLI) Uploader](https://docs.cavatica.org/docs/upload-via-the-command-line). The CLI uploader is a fast and secure upload client that has been optimized to efficiently upload files to CAVATICA, taking advantage of parallelization where possible.

If the two recommended methods above are not convenient or suitable for your use case, you can also consider the following alternative upload option to bring data from your local storage to CAVATICA:

##### Upload via the API
If you want to implement your own upload mechanism, you can use the [CAVATICA API](https://docs.cavatica.org/docs/upload-files) as a low-level method of uploading data to CAVATICA that treats a file as an ordered collection of smaller parts, manipulates multipart uploads, and offers more direct control over uploads.

##### Import from cloud storage
If the data you want to bring to CAVATICA is located in a cloud storage service, rather than your local machine, here are the import methods you can use depending on the location of your data.

##### Import from a volume
If the data is already available on a cloud storage service (AWS S3 or Google Cloud Storage) and you want to use it on CAVATICA without transferring it to CAVATICA storage, use the [Connect Cloud Storage](https://docs.sevenbridges.com/docs/connecting-cloud-storage-overview) feature.

##### Upload from an HTTP(S)/FTP server
If the data is available on an FTP or HTTP endpoint and you want to upload it to CAVATICA (store it in CAVATICA storage), use the [HTTP(S)/FTP](https://docs.cavatica.org/docs/upload-from-an-ftp-server) upload option. 
