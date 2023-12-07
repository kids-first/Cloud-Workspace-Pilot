# CFDE Cloud Workspace Partnership (CWP) Pilot
## Exploring and Accessing Datasets

---
### Overview of Accessing Data in CAVATICA
add content here

---
### Controlled Access Data for Secondary Use
add content here

[dbGaP - Tips for Preparing a Successful Data Access Request](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/GetPdf.cgi?document_name=GeneralAAInstructions.pdf)

[![dbGaP: Apply for Controlled Access Data](https://img.youtube.com/vi/m0xp_cCO7kA/0.jpg)](https://www.youtube.com/watch?v=m0xp_cCO7kA)

---
### Consortium Controlled Access Data
add content here

---
### Open Access Data
add content here

---
### Bring Your Own Data

Suggest Edits
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
