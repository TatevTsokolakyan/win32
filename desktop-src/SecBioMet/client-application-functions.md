---
title: Client Application Functions
description: Functions supported for client application development by the Windows Biometric Framework API.
ms.assetid: 57c9378d-b170-4ba8-8eee-8078531540d5
keywords:
- Windows Biometric Framework API Windows Biometric Framework API , client application functions
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Client Application Functions

The following functions are supported for client application development by the Windows Biometric Framework API.

## In this section



| Topic                                                                                       | Description                                                                                                                                                                                                                              |
|---------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**WinBioAcquireFocus**](/windows/desktop/api/Winbio/nf-winbio-winbioacquirefocus)<br/>                                 | Acquires window focus.<br/>                                                                                                                                                                                                        |
| [**WinBioAsyncEnumBiometricUnits**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncenumbiometricunits)<br/>           | Asynchronously enumerates all attached biometric units that match the input factor type.<br/>                                                                                                                                      |
| [**WinBioAsyncEnumDatabases**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncenumdatabases)<br/>                     | Asynchronously enumerates all registered databases that match a specified type.<br/>                                                                                                                                               |
| [**WinBioAsyncEnumServiceProviders**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncenumserviceproviders)<br/>       | Asynchronously returns information about installed biometric service providers. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                  |
| [**WinBioAsyncMonitorFrameworkChanges**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncmonitorframeworkchanges)<br/> | Starts an asynchronous monitor of changes to the biometric framework.<br/>                                                                                                                                                         |
| [**WinBioAsyncOpenFramework**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncopenframework)<br/>                     | Opens a handle to the biometric framework. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                                       |
| [**WinBioAsyncOpenSession**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncopensession)<br/>                         | Asynchronously connects to a biometric service provider and one or more biometric units. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                         |
| [**WinBioCancel**](/windows/desktop/api/Winbio/nf-winbio-winbiocancel)<br/>                                             | Cancels all pending biometric operations for a specified session. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                |
| [**WinBioCaptureSample**](/windows/desktop/api/Winbio/nf-winbio-winbiocapturesample)<br/>                               | Captures a biometric sample and fills a biometric information record (BIR) with the raw or processed data.<br/>                                                                                                                    |
| [**WinBioCaptureSampleWithCallback**](/windows/desktop/api/Winbio/nf-winbio-winbiocapturesamplewithcallback)<br/>       | Captures a biometric sample asynchronously and returns the raw or processed data in a biometric information record (BIR).<br/>                                                                                                     |
| [**WinBioCloseFramework**](/windows/desktop/api/Winbio/nf-winbio-winbiocloseframework)<br/>                             | Closes a framework handle previously opened with [**WinBioAsyncOpenFramework**](/windows/desktop/api/Winbio/nf-winbio-winbioasyncopenframework). Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                   |
| [**WinBioCloseSession**](/windows/desktop/api/Winbio/nf-winbio-winbioclosesession)<br/>                                 | Closes a biometric session and releases associated resources. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                    |
| [**WinBioControlUnit**](/windows/desktop/api/Winbio/nf-winbio-winbiocontrolunit)<br/>                                   | Allows the caller to perform vendor-defined control operations on a biometric unit. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                              |
| [**WinBioControlUnitPrivileged**](/windows/desktop/api/Winbio/nf-winbio-winbiocontrolunitprivileged)<br/>               | Allows the caller to perform privileged vendor-defined control operations on a biometric unit. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                   |
| [**WinBioDeleteTemplate**](/windows/desktop/api/Winbio/nf-winbio-winbiodeletetemplate)<br/>                             | Deletes a biometric template from the template store. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                            |
| [**WinBioEnrollBegin**](/windows/desktop/api/Winbio/nf-winbio-winbioenrollbegin)<br/>                                   | Initiates a biometric enrollment sequence and creates an empty biometric template. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                               |
| [**WinBioEnrollCapture**](/windows/desktop/api/Winbio/nf-winbio-winbioenrollcapture)<br/>                               | Captures a biometric sample and adds it to a template. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                           |
| [**WinBioEnrollCaptureWithCallback**](/windows/desktop/api/Winbio/nf-winbio-winbioenrollcapturewithcallback)<br/>       | Asynchronously captures a biometric sample and adds it to a template.<br/>                                                                                                                                                         |
| [**WinBioEnrollCommit**](/windows/desktop/api/Winbio/nf-winbio-winbioenrollcommit)<br/>                                 | Finalizes a pending biometric template and saves it to the database associated with the biometric unit used for enrollment. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>      |
| [**WinBioEnrollDiscard**](/windows/desktop/api/Winbio/nf-winbio-winbioenrolldiscard)<br/>                               | Ends the enrollment sequence and discards a pending biometric template. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                          |
| [**WinBioEnrollSelect**](/windows/desktop/api/winbio/nf-winbio-winbioenrollselect)<br/>                                 | Specifies the individual that you want to enroll when data that represents multiple individuals is present in the sample buffer. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/> |
| [**WinBioEnumBiometricUnits**](/windows/desktop/api/Winbio/nf-winbio-winbioenumbiometricunits)<br/>                     | Enumerates all attached biometric units that match the input type.<br/>                                                                                                                                                            |
| [**WinBioEnumDatabases**](/windows/desktop/api/Winbio/nf-winbio-winbioenumdatabases)<br/>                               | Enumerates all registered databases that match a specified type.<br/>                                                                                                                                                              |
| [**WinBioEnumEnrollments**](/windows/desktop/api/Winbio/nf-winbio-winbioenumenrollments)<br/>                           | Retrieves the biometric sub-factors enrolled for a specified identity and biometric unit. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                        |
| [**WinBioEnumServiceProviders**](/windows/desktop/api/Winbio/nf-winbio-winbioenumserviceproviders)<br/>                 | Retrieves information about installed biometric service providers. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                               |
| [**WinBioFree**](/windows/desktop/api/Winbio/nf-winbio-winbiofree)<br/>                                                 | Releases memory allocated for the client application by an earlier call to a Windows Biometric Framework API function. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>           |
| [**WinBioGetCredentialState**](/windows/desktop/api/Winbio/nf-winbio-winbiogetcredentialstate)<br/>                     | Retrieves a value that specifies whether credentials have been set for the specified user. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                       |
| [**WinBioGetDomainLogonSetting**](/windows/desktop/api/Winbio/nf-winbio-winbiogetdomainlogonsetting)<br/>               | Retrieves a value that specifies whether users can log on to a domain by using biometric information.<br/>                                                                                                                         |
| [**WinBioGetEnabledSetting**](/windows/desktop/api/Winbio/nf-winbio-winbiogetenabledsetting)<br/>                       | Retrieves a value that specifies whether the Windows Biometric Framework is currently enabled.<br/>                                                                                                                                |
| [**WinBioGetEnrolledFactors**](/windows/desktop/api/winbio/nf-winbio-winbiogetenrolledfactors)<br/>                     | Gets information about the biometric enrollments that the specified user has on the computer.<br/>                                                                                                                                 |
| [**WinBioGetLogonSetting**](/windows/desktop/api/Winbio/nf-winbio-winbiogetlogonsetting)<br/>                           | Retrieves a value that indicates whether users can log on by using biometric information.<br/>                                                                                                                                     |
| [**WinBioGetProperty**](/windows/desktop/api/Winbio/nf-winbio-winbiogetproperty)<br/>                                   | Retrieves a session, unit, or template property. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                                 |
| [**WinBioIdentify**](/windows/desktop/api/Winbio/nf-winbio-winbioidentify)<br/>                                         | Captures a biometric sample and determines whether it matches an existing biometric template. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                    |
| [**WinBioIdentifyWithCallback**](/windows/desktop/api/Winbio/nf-winbio-winbioidentifywithcallback)<br/>                 | Asynchronously captures a biometric sample and determines whether it matches an existing biometric template.<br/>                                                                                                                  |
| [**WinBioLocateSensor**](/windows/desktop/api/Winbio/nf-winbio-winbiolocatesensor)<br/>                                 | Retrieves the ID number of a biometric unit selected interactively by a user.<br/>                                                                                                                                                 |
| [**WinBioLocateSensorWithCallback**](/windows/desktop/api/Winbio/nf-winbio-winbiolocatesensorwithcallback)<br/>         | Asynchronously retrieves the ID number of the biometric unit selected interactively by a user.<br/>                                                                                                                                |
| [**WinBioLockUnit**](/windows/desktop/api/Winbio/nf-winbio-winbiolockunit)<br/>                                         | Locks a biometric unit for exclusive use by a single session. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                    |
| [**WinBioLogonIdentifiedUser**](/windows/desktop/api/Winbio/nf-winbio-winbiologonidentifieduser)<br/>                   | causes a fast user switch to the account associated with the last successful identification operation performed by the biometric session.<br/>                                                                                     |
| [**WinBioMonitorPresence**](/windows/desktop/api/winbio/nf-winbio-winbiomonitorpresence)<br/>                           | Turns on the face-recognition or iris-monitoring mechanism for the specified biometric unit. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                     |
| [**WinBioOpenSession**](/windows/desktop/api/Winbio/nf-winbio-winbioopensession)<br/>                                   | Connects to a biometric service provider and one or more biometric units.<br/>                                                                                                                                                     |
| [**WinBioRegisterEventMonitor**](/windows/desktop/api/Winbio/nf-winbio-winbioregistereventmonitor)<br/>                 | Registers a callback function to receive event notifications from the service provider associated with an open session.<br/>                                                                                                       |
| [**WinBioReleaseFocus**](/windows/desktop/api/Winbio/nf-winbio-winbioreleasefocus)<br/>                                 | Releases window focus.<br/>                                                                                                                                                                                                        |
| [**WinBioRemoveAllCredentials**](/windows/desktop/api/Winbio/nf-winbio-winbioremoveallcredentials)<br/>                 | Removes all credentials from the store. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                                          |
| [**WinBioRemoveAllDomainCredentials**](/windows/desktop/api/Winbio/nf-winbio-winbioremovealldomaincredentials)<br/>     | Removes all user credentials for the current domain from the store. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                              |
| [**WinBioRemoveCredential**](/windows/desktop/api/Winbio/nf-winbio-winbioremovecredential)<br/>                         | Deletes a biometric logon credential for a specified user. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                       |
| [**WinBioSetCredential**](/windows/desktop/api/Winbio/nf-winbio-winbiosetcredential)<br/>                               | Saves a biometric logon credential for the current user. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                                                                         |
| [**WinBioSetProperty**](/windows/desktop/api/winbio/nf-winbio-winbiosetproperty)<br/>                                   | Sets the value of a standard property associated with a biometric session, unit, template, or account. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                           |
| [**WinBioUnlockUnit**](/windows/desktop/api/Winbio/nf-winbio-winbiounlockunit)<br/>                                     | Releases the session lock on the specified biometric unit.<br/>                                                                                                                                                                    |
| [**WinBioUnregisterEventMonitor**](/windows/desktop/api/Winbio/nf-winbio-winbiounregistereventmonitor)<br/>             | cancels event notifications from the service provider associated with an open biometric session.<br/>                                                                                                                              |
| [**WinBioVerify**](/windows/desktop/api/Winbio/nf-winbio-winbioverify)<br/>                                             | Captures a biometric sample and determines whether the sample corresponds to the specified user identity. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                        |
| [**WinBioVerifyWithCallback**](/windows/desktop/api/Winbio/nf-winbio-winbioverifywithcallback)<br/>                     | Asynchronously captures a biometric sample and determines whether the sample corresponds to the specified user identity.<br/>                                                                                                      |
| [**WinBioWait**](/windows/desktop/api/Winbio/nf-winbio-winbiowait)<br/>                                                 | Blocks caller execution until all pending biometric operations for a session have been completed or canceled. Starting with Windows 10, build 1607, this function is available to use with a mobile image.<br/>                    |



 

## Related topics

<dl> <dt>

[Client Application Reference](client-application-reference.md)
</dt> </dl>

 

 




