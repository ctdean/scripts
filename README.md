# Scripts

Collection of personal scripts.  That are unsupported and
undocumented.

- Chris Dean <ctdean@sokitomi.com>

## s3-download-urls

- Desription: Print the temporary urls to download from an s3 bucket.
  These urls can be used to download an s3 object even if the object
  is marked as private.  The url expires after N seconds after
  created.

- Install:
  - Install ruby
  - `gem install aws-sdk`

- Usage:
  - To create a single url:  `s3-download-urls s3://standard-releases/jars/workflow/workflow-standalone.jar`
  - To print a curl download command line: `s3-download-urls --curl s3://standard-releases/jars/workflow/workflow-standalone.jar`
  - To print curl download lines for an entire tree: `s3-download-urls -r --curl s3://standard-releases/releases/foe`
