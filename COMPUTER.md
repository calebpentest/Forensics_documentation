Computer components communicate through buses.

* **CPU** executes instructions and controls operations.
* **Memory (RAM)** stores instructions and data for fast access.
* **I/O devices** handle input (keyboard, mouse) and output (screen, printer).

They connect through **buses**:

* **Data bus** moves actual data.
* **Address bus** specifies where in memory or I/O to read/write.
* **Control bus** carries signals (read, write, clock, interrupt).

How NTFS deletion and recovery works:

**1. File creation in NTFS**

* Every file has an entry in the **Master File Table (MFT)**.
* The MFT stores metadata: filename, timestamps, permissions, and pointers to data clusters on disk.
* Actual file content is saved in clusters (sectors grouped together).

**2. File deletion**

* When you delete a file in Windows, NTFS does not erase the data immediately.
* The MFT entry is marked as **unused**.
* Clusters holding the file content are flagged as **available**.
* The data remains until overwritten by new files.

**3. Recovery opportunity**

* Since the MFT entry and data clusters may still exist, forensic tools can read them.
* If the clusters are intact, recovery is complete.
* If partially overwritten, recovery is incomplete or corrupted.

**4. Recovery sources in NTFS**

* **MFT records**: list of files, including deleted ones.
* **\$Bitmap file**: tracks free/used clusters, helps identify where deleted data may still reside.
* **\$LogFile (transaction journal)**: contains recent file system changes, can help roll back or reconstruct.
* **Shadow copies/Volume snapshots**: Windows “Previous Versions” feature keeps copies of files.
* **\$Recycle.Bin**: sometimes the file is only moved here, not deleted.

**5. Tools used**

* Autopsy / Sleuth Kit: parse MFT and recover files.
* FTK Imager: create disk images and extract deleted files.
* X-Ways Forensics, EnCase: professional forensic recovery.
* `ntfsundelete` (Linux) for direct recovery.

**Key idea:** In NTFS, “delete” usually just means “mark as free.” The data persists until overwritten, which is why fast imaging of the disk is critical in forensics.

Do you want me to also map this visually with a **diagram of MFT → deletion → recovery** so you can see the process clearly?
