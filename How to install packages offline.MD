To download a Python package as a file on your phone for later installation on a computer, follow these steps:


1. **Download the Package File:**
   - Open a web browser on your phone.
   - Go to the Python Package Index (PyPI) website: [pypi.org](https://pypi.org/).
   - Search for the package you want to download.
   - On the package page, navigate to the "Download files" section.
   - Choose the appropriate file (usually a `.whl` or `.tar.gz` file) and download it to your phone.


2. **Transfer the File to Your Computer:**
   - **Using a USB Cable:**
     1. Connect your phone to your computer using a USB cable.
     2. Enable file transfer mode on your phone.
     3. Copy the downloaded package file from your phone to your computer.
   - **Using Cloud Storage:**
     1. Upload the file to a cloud storage service (like Google Drive, Dropbox, or OneDrive) from your phone.
     2. Access the cloud storage on your computer and download the file.
   - **Using Email:**
     1. Attach the file to an email and send it to yourself.
     2. Open the email on your computer and download the attachment.


3. **Install the Package on Your Computer:**
   - Open a terminal or command prompt on your computer.
   - Navigate to the directory where you saved the downloaded package file.
   - Use `pip` to install the package. For example:
     ```bash
     pip install package_file.whl
     ```
     or
     ```bash
     pip install package_file.tar.gz
     ```


This process allows you to download Python packages on your phone and later install them on your computer.



#### OR

### On the system that has access to internet

The pip `download` command lets you download packages without installing them:

    pip download -r requirements.txt
    

(In previous versions of pip, this was spelled `pip install --download -r requirements.txt`.)

### On the system that has no access to internet

Then you can use

    pip install --no-index --find-links /path/to/download/dir/ -r requirements.txt
    

to install those downloaded modules, without accessing the network.