# OverDrive
** This stanza needs manual review at [https://www.oclc.org/support/services/ezproxy/documentation/db/overdrive.en.html](https://www.oclc.org/support/services/ezproxy/documentation/db/overdrive.en.html) **

## Some of OCLC's notes for this stanza

EZproxy is not used to proxy access to OverDrive. When you create links to OverDrive, you will create direct links to OverDrive with no reference to EZproxy. Instead of proxying access, EZproxy is linked with OverDrive to handle user authentication when a user performs an action that requires an OverDrive account such as checking out an item.

When a user authenticates for OverDrive access, EZproxy creates a "persistent identifier" for the user. The persistent identifier is an arbitrary series of letters and digits that is uniquely assigned to the user. Each time the same user accesses OverDrive, the same persistent identifier will be used for the user. However, the value of the persistent identifier gives no personally identifiable information about the user, so the persistent identifier does not provide any information for the identity of the user. In an instance of abuse, OverDrive can provide your library with the persistent identifier and you can use the EZproxy administration page to cross-reference back to the original user if necessary.

The persistent identifiers are stored in the file ezproxy.tkn. If this file is lost, all correlation between your users and their persistent identifiers is lost, disrupting all accounts. To avoid disruption of service caused by server crash, you are encouraged to insure that this file is backed up on a regular basis.

To maintain persistent identifiers, EZproxy requires unique user login information, and most EZproxy user authentication methods provide such information. AutoLoginIP and referring URL are incompatible since they do not provide unique user information. Sites that use CGI authentication should insure that they are providing "loguser" information to associate distinct user information. If you have any questions regarding this requirement, contact OCLC support.

OverDrive does not use a traditional database definition. It requires a single, special entry in config.txt  that looks like this:

OverDrive will provide you with the values to insert after -URL= and -Secret=. -ILSName and -LibraryID are optional; if they are required, OverDrive will provide you with these values; otherwise, you should omit these. You will replace sitename with a short code that describes you institution; a common value is the unique part of your domain name (e.g. for yourlib.org, a typical value might be yourlib).

To form the URL to provide to OverDrive, take your base EZproxy URL (e.g. http://ezproxy.yourlib.org:2048), add "/OverDrive/" and add the sitename, such as:

Note: the port number above is optional. If you are using standard port 80, then the port number can be omitted.
 

Once you provide this URL to OverDrive, they can configure everything on their servers to complete the integration.

If needed, it is possible to have more than one OverDriveSite directive. OverDriveSite also interacts with Group, allowing different configurations to be associated with different groups to meet the needs of a consortium. If you need help constructing such a configuration, contact OCLC support.
