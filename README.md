# Privacy Policy — CBH NextGen Connector

**Last updated: June 26, 2026**

CBH NextGen Connector ("the extension") is a browser extension that helps medical
billing staff complete claims in NextGen Office using their Clinic Billing Helper
(CBH) account. This policy explains what the extension accesses, what it sends,
and what it stores. NextGen Office is a third-party product; this extension is an
independent tool and is not affiliated with NextGen.

## Who this is for

The extension is an internal tool for staff of the practice that operates Clinic
Billing Helper. It does nothing without a Clinic Billing Helper account and a
personal API key issued from that account.

## What the extension accesses

When you open a claim in NextGen Office and run the extension, it reads only
specific fields from the open claim:

- ICD-10 diagnosis codes
- Servicing provider, location, and the names of the primary and secondary
  insurance payers
- Date of service
- The provider role fields it fills in (referring, rendering, supervising,
  pay-to, and billing) and the fee schedule

The extension does **not** read the patient's name or other patient-identifying
information from the claim page.

## What the extension sends, and to whom

To do its job, the extension sends the following to **your Clinic Billing Helper
instance only** — never to any other third party:

- The diagnosis codes and date of service, to validate the ICD-10 codes
- The servicing provider, location, and insurance payer names, to determine the
  correct providers and fee schedule

These requests are authenticated with your personal API key. The information sent
does not include the patient's name or other direct patient identifiers.

## What the extension stores

The extension stores the following in your browser, using the browser's extension
storage:

- Your personal Clinic Billing Helper API key, and an optional server-URL
  override, so you do not have to re-enter them each session
- A short-lived cache of your most recent claim scan and auto-fill result, per
  browser tab, so the popup can re-display it if you close and reopen it

This data stays in your browser. It is not sold or shared with any third party,
and it contains no patient-identifying information.

## API key usage records

When your API key is used, the Clinic Billing Helper service records standard
security metadata for that key: the time it was last used, the IP address of the
request, and the browser/device type. This is used to secure and manage API keys.
API keys expire 90 days after they are created and can be revoked at any time from
Clinic Billing Helper.

## Data the extension does not collect

The extension does not use analytics or tracking, does not collect your browsing
history, and does not access any websites other than NextGen Office
(healthfusionclaims.com) and your Clinic Billing Helper instance.

## Data security

All communication with Clinic Billing Helper occurs over HTTPS. API keys are
stored on the server only as a cryptographic hash (never in plain text) and are
transmitted only to your Clinic Billing Helper instance.

## Changes to this policy

This policy may be updated from time to time. Material changes will be reflected
here with a new "Last updated" date.

## Contact

Questions about this policy can be directed to **obieze.apex@gmail.com**.
