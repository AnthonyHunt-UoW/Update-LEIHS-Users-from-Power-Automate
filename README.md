# Update-LEIHS-Users-from-Power-Automate

The flow setting can be configured in the first action of the flow. The consist of:

ServerURL - The URL of the LEIHS Server without "https://"
APIToken - The API Token of an LEIHS user with read/write permissions to users.
LEIHSAdmins - This is an array of LEIHS Users from AD who will always be configured as LEIHS admins. This option is both a security risk and a security measure. Use wisely.
LEIHSServerAdmins - This is an array of LEIHS Users from AD who will always be configured as LEIHS server admins. This option is both a security risk and a security measure. Use wisely.
Organization - This is the email domain from AD.
ProfileImageURL - This is the URL part of for where you LEIHS profile images are stored. By default the image name is pulled from "ExtensionAttribute1" but can be changed in the main flow.
ProfilImageExtension - The extension for your profile images.
MissingFromADOrganization - When an account in LEIHS is missing from AD it will be moved to this organization. This helps identify stale accounts.
ExcludeFromDeletion - An array of account in LEIHS to exclude from moving to "MissingFromADOrganization". **** Currently not implimented ***
EmailResultsAddress - The email address to send the report of additions, updates, deletions (flagged) and errors to.

