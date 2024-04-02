# printclient-releases-qa
Contains releases for SimpleRfid print client

UpgradeCode {CCC8EE69-837E-4321-B420-16A446C67A81}

Steps to deploy ZPL print Client's version:

1. Increase Assembly vresion and File version of SimpleRfid.ZplPrintClient project (these options will be in Properties -> Assembly Information window).
2. Increase SimpleRfid.NewPrintClient.Installer's Version (in Properties window). After increasing Version's number you'll see window which should ask you to change Product code. Press "Yes". (!IMPORTANT! SimpleRfid.ZplPrintClient versions numbers and SimpleRfid.NewPrintClient.Installer version number should be the same).
3. Change Upgrade code in SimpleRfid.ZplPrintClient.Installer project to Upgrade code from this documentation (↑ above this steps).
4. Change Manufacturer, Description and ProductName in SimpleRfid.ZplPrintClient.Installer project (just remove "Dev" part).
5. Build SimpleRfid.NewPrintClient project in Prod or Release mode.
6. Build SimpleRfid.NewPrintClient.Installer project in Prod or Release mode.
7. Go to SimpleRfid.NewPrintClient.Installer's folder, then go into "Release" folder, where you'll see simplerfid-printclient.msi file.
8. Create new release with same number as your project's versions in this repository. And add simplerfid-printclient.msi as attached file.
