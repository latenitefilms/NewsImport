# How To Use

When you first run **News Import** from the Mac App Store you'll be presented with this:

![](/static/install.png)

Clicking **Launch Final Cut Pro** will launch Final Cut Pro and close the **News Import** application.

You can now access **News Import** from the Workflow Extension button in Final Cut Pro:

![](/static/toolbar.png)

You can also access it from the Workflow Extension menubar:

![](/static/menubar.png)

The first time you open the **News Import** Workflow Extension it will look like this:

![](/static/fresh-install.png)

To get started you need to press the **Install Metadata View** button.

You'll be presented with a window like this:

![](/static/install-metadata-view.png)

Click **Grant Permission**.

You'll be presented with this message:

![](/static/restart-finalcutpro.png)

As instructed, please restart Final Cut Pro.

You'll now be able to access three new Metadata Views in Final Cut Pro:

- News Import
- NewsML-G2
- VPMS

The News Import Metadata View contains all the values from both NewsML-G2 and VPMS.

You can access these Metadata Views at the bottom of Final Cut Pro's Info Inspector:

![](/static/metadata-views.png)

Because News Import is a sandbox application, you need to grant it access to the drive or folder that contains your footage.

Click the **Add Media Location** button to add a new Media Location.

Select the drive or folder that contains your footage, then click **Grant Permission**.

![](/static/grant-permission.png)

For example, I've granted News Import access to my system drive:

![](/static/granted-system-drive.png)

You can now drag an **Event** which contains footage to the **Drop Event Here** area.

**IMPORTANT:** Make sure the `.newsml.xml` and/or `.vpms.xml` files are in the same folder as the media file and have matching names.

For example, you should have three files all next to each other:

- `video_001.mxf`
- `video_001.newsml.xml`
- `video_001.vpms.xml`

You should check that you have **Leave files in place** selected in the Final Cut Pro preferences, otherwise the media files will be inside the Library bundle.

After dragging in an **Event**, the **Drag to your Final Cut Pro Library** button will now be blue:

![](/static/ready-to-drag.png)

You can now drag this **Event** back into your Final Cut Pro **Library** (in the **Browser**).

This will create a new **Event**, however, you can delete this Event straight away, as the Metadata will be automatically applied to the original source clips.

All the metadata from the sidecar files will now be accessible from the **Info Inspector**.

---

## Support Metadata Fields

We currently support the following **NewsML-G2** Metadata Fields:

- `org.iptc.newsML-G2.providerName`
- `org.iptc.newsML-G2.firstCreated`
- `org.iptc.newsML-G2.fileName`
- `org.iptc.newsML-G2.contentCreated`
- `org.iptc.newsML-G2.locatedName`
- `org.iptc.newsML-G2.creatorName`
- `org.iptc.newsML-G2.contributorName`
- `org.iptc.newsML-G2.genreName`
- `org.iptc.newsML-G2.subjectName`
- `org.iptc.newsML-G2.headline`
- `org.iptc.newsML-G2.description`

We currently support the following **VPMS** Metadata Fields:

- `org.vpms.standardJob.som`
- `org.vpms.standardJob.eom`
- `org.vpms.standardJob.acquisitionDate`
- `org.vpms.standardJob.tcSOM`
- `org.vpms.standardJob.tcEOM`
- `org.vpms.standardJob.tcSOMOfInterest`
- `org.vpms.standardJob.tcEOMOfInterest`
- `org.vpms.standardJob.dateOfExpiry`
- `org.vpms.standardJob.sourceDatabaseRef`
- `org.vpms.cutList.programName`
- `org.vpms.cutList.broadcastShortcut`
- `org.vpms.cutList.name`
- `org.vpms.cutList.description`
- `org.vpms.cutList.owner`
- `org.vpms.cutList.onAirDate`
- `org.vpms.cutList.onAirTime`
- `org.vpms.cutList.id`
- `org.vpms.cutList.jobTitlePrefix`
- `org.vpms.shotList.default.shotDescription`
- `org.vpms.shotList.default.shotLongDescription`
- `org.vpms.shotList.default.shotMemo1`
- `org.vpms.shotList.default.shotMeno2`
- `org.vpms.shotList.default.tcEOM`
- `org.vpms.shotList.default.tcSOM`
- `org.vpms.shotList.cutlist.shotDescription`
- `org.vpms.shotList.cutlist.shotLongDescription`
- `org.vpms.shotList.cutlist.shotMemo1`
- `org.vpms.shotList.cutlist.shotMeno2`
- `org.vpms.shotList.cutlist.tcEOM`
- `org.vpms.shotList.cutlist.tcSOM`
- `org.vpms.shotList.cuts.shotDescription`
- `org.vpms.shotList.cuts.shotLongDescription`
- `org.vpms.shotList.cuts.shotMemo1`
- `org.vpms.shotList.cuts.shotMeno2`
- `org.vpms.shotList.cuts.tcEOM`
- `org.vpms.shotList.cuts.tcSOM`
- `org.vpms.shotList.nle.shotDescription`
- `org.vpms.shotList.nle.shotLongDescription`
- `org.vpms.shotList.nle.shotMemo1`
- `org.vpms.shotList.nle.shotMeno2`
- `org.vpms.shotList.nle.tcEOM`
- `org.vpms.shotList.nle.tcSOM`

If there's a metadata field missing that you require, or if there's a different News sidecar file that we don't currently support, [please let us know](https://github.com/latenitefilms/NewsImport/issues).