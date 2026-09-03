# RQ1 release manifest

`latest.json` names the most recently published version of the RQ1 TSB
processing platform. An installation reads it to tell its administrator that a
newer build exists.

It carries a version number, a date, and one line of text. Nothing else lives
here on purpose: an installation should be able to learn that an update exists
without being given credentials for a private repository, and a public file is
the smallest way to do that. It holds no code, no release notes, no links into
private repositories, and no customer information.

Updates are never downloaded or installed from here. The application only
reports what this file says; installing a build is a deliberate action taken on
the machine, because a database migration cannot be undone automatically.
