## iCloud3 Version 2.2.0 - Release Candidate Change Log

#### Release Candidate 4 (5/31/2020)

* The Event Log will only show the state/zone/interval/travel time/distance line when the values change. This reduces the size of the Event Log and improves it's readability.

* Cleaned up the Event Log code and made several visual changes.

* Errors encountered when sending a message to a device are now caught. The error and message are displayed in the HA log and on the Event Log.

* Increased the number of records that will be displayed in the Event Log.

* When the account needed to be authenticated in the Web Services Program (pyicloud-ic3.py), an 'Error 450' error message was displayed in the HA Log. This has been changed to an Info message that describes that the authentication is needed.

* The battery level from the iOS App is now displayed when using the Find-my-Friends tracking method or when the battery level is not available when using the Family Sharing tracking method.
* Cleaned up and tuned some more code.

#### Release Candidate 3 (5/27/2020)

* Fixed an issue where the iOS App location request time was not set available, creating an error when restarting ic3 multiple of times on the Event Log screen.

* iCloud3 was using legacy HA DeviceScanner code that was made available for people running HA versions before 0.95. iCloud3 will now use the current code rather than legacy code.

* Changed the "Error 450" error message generated by pyicloud_ic3.py when the iCloud account needed to be authenticated from an 'error' message to an 'info' message. It now just indicates a reauthentication is needed, which is then done by iCloud3.

#### Release Candidate 2 (5/26/2020)

* Fixed the error generated if running older versions of HA that do not have the zone.reload service call.

* Revamped the Trusted Device selection and code entry forms to fix some issues where the Trusted Devices were not displayed.

* Did some home house keeping and added a few error trapping routines.