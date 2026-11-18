# Privacy Policy: Apex Hub Connector

**Last updated: November 18, 2026**

Apex Hub Connector ("the extension", formerly CBH NextGen Connector) is a
browser extension that helps a medical practice's billing staff do their
billing work in NextGen Office and CollaborateMD using the practice's Apex Hub
account (Apex Hub was formerly called Clinic Billing Helper). This policy
explains what the extension reads, what it sends, and what it stores. NextGen
Office and CollaborateMD are third-party products; the extension is an
independent tool and is not affiliated with either.

## Who this is for

The extension is an internal tool for staff of the practice that operates Apex
Hub. It does nothing without an Apex Hub account and a personal API key issued
from that account. The practice's Apex Hub administrator decides which
features each person has.

## Websites the extension works on

- **NextGen Office** (nextgenoffice.cloud and healthfusionclaims.com)
- **CollaborateMD** (app.collaboratemd.com), added in version 1.29
- **The practice's own Apex Hub server**

It does not run on, read or collect anything from any other website.

## What the extension reads

On the page you have open, and only to do the task you asked for:

- **A NextGen claim:** diagnosis and procedure codes, modifiers, units and
  charges, date of service, providers, location, insurance payer names, the
  claim's status and identifiers, and the fields the extension fills in.
- **The visit behind a claim** (for people with the note checks turned on):
  blood pressure, test results, medications and diagnoses recorded for that
  visit, the visit's appointment type and reason, and the patient's prior
  authorizations and insurance ID and group number.
- **NextGen remittances (ERAs) and reports**, to decode a remittance, send it
  to Apex Hub, or export a report you asked for.
- **A CollaborateMD claim** (for people with surgery-center injection billing
  turned on): the claim's patient, payer, member ID, group number,
  authorization and charge lines.
- **A patient's name and date of birth** from the NextGen claim, only to pick
  the same patient in CollaborateMD (see below).

## What the extension sends, and to whom

Everything the extension sends goes to **the practice's own Apex Hub server
only**, over HTTPS, authenticated with your personal API key. Nothing is sent
to the extension's developer or to any other third party, and nothing is sold.

- **Claim checks:** the claim's codes, modifiers, units, charges, date of
  service, providers, location and payer names, so Apex Hub can validate them
  and return the practice's rules and prices. For a self-pay claim, the
  patient's NextGen member ID is sent so Apex Hub can look up a discount.
- **Remittances (ERAs):** payment and denial data. Patient names, member IDs,
  account numbers and addresses are removed in the browser before an ERA is
  sent.
- **Usage counts:** that a check ran or a change was undone, keyed to the
  claim's number, so the practice can measure the tool. For people with claim
  snapshots turned on, the claim's codes and status as well.
- **The assistant:** what you type into it.
- **A superbill photo** (only when you choose to take or pick one): the photo
  is sent to Apex Hub to be read and is not stored by the extension. Apex Hub
  returns the codes marked on the sheet.
- **Problem reports** you choose to send.

**A patient's name and date of birth are never sent to Apex Hub by the
extension.** For surgery-center injection billing they are passed inside your
browser from the NextGen tab to the CollaborateMD tab, to find the same
patient there, and are held only in the browser's session memory, which is
cleared when the browser closes.

## What the extension writes

The extension fills in fields on the NextGen or CollaborateMD claim you have
open, when you ask it to. It does not save, submit or delete a claim: you
review and save.

## What the extension stores in your browser

- Your personal Apex Hub API key, on this device only, and an optional
  server-address override
- Settings (theme, pinned panel) and the list of features turned on for you
- The most recent check result per tab, so the panel can show it again
- Progress counts for ERA sync (counts and dates, no patient data)
- In session memory only, cleared when the browser closes: the open assistant
  conversation, and the surgery-center case you are entering (codes, the
  patient's name and date of birth, insurance ID)

Report files you export are saved to your computer's Downloads folder, as you
asked; they are not sent anywhere by the extension.

## API key usage records

When your API key is used, Apex Hub records standard security metadata for
that key: the time it was last used, the IP address of the request, and the
browser or device type. API keys expire 90 days after they are created and can
be revoked at any time from Apex Hub.

## Data the extension does not collect

The extension does not use analytics or advertising trackers, does not collect
your browsing history, and does not read any page outside the websites listed
above.

## Data security

All communication with Apex Hub is over HTTPS. API keys are stored on the
server only as a cryptographic hash and are sent only to the practice's Apex
Hub server. Patient information handled by Apex Hub is covered by the
practice's own HIPAA obligations and agreements.

## Changes to this policy

This policy may be updated from time to time. Material changes are reflected
here with a new "Last updated" date. Version 1.29 added CollaborateMD, the
surgery-center injection card and the superbill photo.

## Contact

Questions about this policy can be directed to **obieze.apex@gmail.com**.
