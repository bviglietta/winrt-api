---
-api-id: P:Windows.Storage.ApplicationData.LocalFolder
-api-type: winrt property
---

<!-- Property syntax
public Windows.Storage.StorageFolder LocalFolder { get; }
-->

# Windows.Storage.ApplicationData.LocalFolder

## -description
Gets the root folder in the local app data store. This folder is backed up to the cloud.

## -property-value
The file system folder that contains the files.

## -remarks
You can access files in the local app data store using the "ms-appdata:///local/" protocol. For example:

`<img src="ms-appdata:///local/myFile.png" alt="" />`

To access files in the app package, use [Windows.ApplicationModel.Package.Current.InstalledLocation](../windows.applicationmodel/package_installedlocation.md).

To request that Windows index your app data for search, create a folder named "Indexed" under this folder and store the files that you want indexed there. Windows indexes the file content and metadata (properties) in this "Indexed" folder and all its subfolders.

If the device that runs this app supports app data backup, any content placed on [LocalFolder](applicationdata_localfolder.md) will be eligible to be backed up to the cloud. Therefore if you want to persist data and keep it local to the device you should consider using [LocalCacheFolder](applicationdata_localcachefolder.md).

## -examples

## -see-also
[Quickstart: Local application data (JavaScript)](http://msdn.microsoft.com/library/87dfe8e5-2d01-45cf-bcb1-25f54219a439), [Store and retrieve settings and other app data](http://msdn.microsoft.com/library/41676a02-325a-455e-8565-c9ec0bc3a8fe), [Store and retrieve settings and other app data](http://msdn.microsoft.com/library/41676a02-325a-455e-8565-c9ec0bc3a8fe)