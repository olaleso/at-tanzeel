# At-Tanzeel school portal concept

An independent NuraSpecs Solutions demonstration prepared for At-Tanzeel Schools, Ikorodu, Lagos. All learner, financial and operational records are fictional. This is not an official school service.

## Deploy from GitHub to Cloudflare Pages

Connect this repository in Cloudflare: Workers & Pages > Create application > Pages > Connect to Git.

| Setting | Value |
| --- | --- |
| Production branch | `main` |
| Framework preset | `None` |
| Build command | Leave blank |
| Build output directory | `public` |
| Root directory | Leave at repository root |
| Environment variables | None |

Select Save and Deploy. Cloudflare will deploy changes pushed to the production branch automatically. Use the actual URL returned by Cloudflare; a name suggested in this documentation is not a verified live address.

The site includes the proposal at `/proposal.pdf`. The `public` directory is the entire deployable site; no package installation is needed for hosting.

## Demo credentials

Password for all roles: `NuraDemo!2026`

- Administrator: `admin@demo.nuraspecs.com`
- Teacher: `teacher@demo.nuraspecs.com`
- Bursar: `bursar@demo.nuraspecs.com`
- Hostel warden: `hostel@demo.nuraspecs.com`
- Parent: `parent@demo.nuraspecs.com`
- Student: `student@demo.nuraspecs.com`

These are public demo identifiers, not functioning mailboxes or secure authentication credentials.

## Features

Role-specific navigation, student search and creation, admissions stages, dated attendance registers, result calculations and publication, printable reports, simulated partial payments and receipts, CSV exports, room allocations, leave approval, Hifz progress, timetables, local notices and an illustrative activity trail.

## Important boundaries

- Client-side role simulation only; production needs server-enforced authentication and authorisation.
- Data persists only in this browser using `ns-demo-v1`; no shared database.
- Payment outcomes are simulated; no live gateway or real money movement.
- No email/SMS delivery, real pupil data or medical records.
- Parent/student result previews may show unpublished sample results; production publication must be enforced server-side.
- Room eligibility needs manual confirmation in the demo; production must enforce school rules.
- Google Fonts is optional; system fonts provide a fallback.
- Use Settings & audit as administrator to restore sample data.

## Check locally

Open `public/index.html` in a browser or serve `public` using a local static server.

For the DOM-based logic checks:

```sh
npm ci
npm test
```

These checks do not replace visual browser testing. Before outreach, verify the live desktop/mobile layout, each demo role, result printing, payment simulations and the proposal download. See `docs/verification.txt` for prior verification scope.

## Company

NuraSpecs Solutions — https://nuraspecs.com/
info@nuraspecs.com · +234 803 845 5341

## References

- School: https://attanzeelschools.com/
- Facilities: https://attanzeelschools.com/our-facility/
- Cloudflare Git integration: https://developers.cloudflare.com/pages/get-started/git-integration/

The school website already links a Check Results service. Its capabilities were not assessed; this concept proposes discovery and potential integration or improvement.
