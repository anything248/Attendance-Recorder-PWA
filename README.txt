Office Attendance Tracker V0.1 — Offline-first PWA

START:
- For immediate desktop testing, double-click index.html (works as a local web page).
- For mobile PWA installation and offline service worker: host these files together at an HTTPS URL (e.g. GitHub Pages or another approved static host). Open URL in Android Chrome or iOS Safari, then Add to Home Screen. Opening index.html as file:// is NOT a PWA installation.
- Each user has their own device-local records (browser localStorage). Export JSON backups periodically: clearing app/browser data may erase records.

WORKFLOW:
Calendar: tap a past or current eligible day to mark/unmark attendance.
Quarter: view cumulative quarters, surplus visualization, monthly detail.
Year: see every recorded date sorted by fiscal quarter.
Settings: percentage, country/region, benchmark basis, fiscal year; personal holiday and workday overrides.
Export HTML: standalone, browser-openable, read-only attendance snapshot, with month selector/calendar; no connection to your phone.
Export CSV: detailed calendar records for Excel.
Backup JSON: full device state; importing overwrites phone local state after confirmation.

RULES:
Default benchmark: CEIL(percentage * Mon-Fri calendar days), public holidays INCLUDED.
Available days: eligible days on/after local today; weekends excluded except official make-up workdays; public holidays excluded.
Monthly independent; quarter actual cumulative and surplus doesn't cross quarters; yearly raw actual crosses quarters.
Yellow when buffer=0 or 1; Red if impossible; Met if target already achieved. Any incomplete holiday calendar is a limitation of the risk indicator.

KNOWN LIMITATIONS:
- Built for FY Nov 2026 through Oct 2027 by default. SG holidays for this FY are bundled from MOM.
- China 2027 national scheduled holidays and make-up workdays are bundled. Nanning's Guangxi-specific holidays are NOT bundled; add confirmed local dates as overrides.
- Malaysia 2027 federal/state calendar is preliminary and substitute holidays may require verification. Confirm dates with local HR/official schedules before relying on risk alerts.
- No cloud sync, no automatic notifications, no audit log, no encryption. Browser storage can be cleared by OS/browser. Keep backups.
- A local file runs but service workers / install mode require HTTPS or localhost. Some corporate browsers may restrict local HTML scripts.
- User-selected dates on holidays and weekends are blocked; exceptional days can be enabled through settings overrides. Policy changes are applied retroactively in this prototype.

DATA PRIVACY: no network data transfer in app itself, unless you follow the clickable source links. Hosting service may still log initial page downloads; user attendance stays local. Exporting/sharing reports is an explicit user action.

Verification sources: Singapore MOM https://www.mom.gov.sg/employment-practices/public-holidays ; Malaysia BKPP https://www.kabinet.gov.my/hari-kelepasan-am/ ; China https://www.gov.cn/zhengce/content/202611/content_7085101.htm
