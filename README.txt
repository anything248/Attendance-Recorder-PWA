Office Attendance PWA v0.2

Upload all 5 files to the repository root.

Changes:
- Country: Singapore, Malaysia (Selangor/Kuala Lumpur), China national, Poland national.
- Language in Settings: English / 简体中文. Interface switches upon Save settings.
- Poland FY27 statutory holiday dates bundled. Weekend statutory days may require employer-defined substitute day. Add holiday override for actual substitute day.
- Existing local attendance preserved: same localStorage key office-attendance-v01.
- Export JSON backup before changing settings/updating.
- To force offline app refresh, close installed app and reopen online after GitHub Pages redeploy; service-worker cache upgraded to v02.

WARNING: Country calendars and employer-specific replacement holidays must be checked before relying on risk alarms.

Sources:
- Poland: EU EURES https://eures.europa.eu/eures-services/chat-eures-advisers/public-holidays-calendar_en
- Polish Labour Inspectorate https://www.pip.gov.pl/
- Singapore: MOM https://www.mom.gov.sg/employment-practices/public-holidays
