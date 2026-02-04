# Disposition of Comments for the WebExtensions Working Group Charter

This document is the disposition of comments received during the review
of the [WebExtensions Working Group draft charter](https://w3c.github.io/charter-drafts/2025/webextensions-wg.html).

Comments were received through:

- [w3c/strategy#146](https://github.com/w3c/strategy/issues/146) — Strategy funnel issue (horizontal reviews, TAG review)
- [w3c/charter-drafts#690](https://github.com/w3c/charter-drafts/issues/690) — TAG request to update the Coordination section
- [w3c/charter-drafts#711](https://github.com/w3c/charter-drafts/pull/711) — Charter revision PR addressing all feedback

## Executive Summary

All comments received during the review of the WebExtensions Working
Group charter have been addressed. No formal objections were raised.
There are no unresolved issues blocking the charter from moving forward.

Of the 20 comments received:

- **14 were accepted** and resulted in charter changes, including the
  addition of new scope entries (user agent extensibility, network
  request modification), a Threat Model document in Other Deliverables,
  vendor autonomy language, explicit out-of-scope treatment of browser
  UI specifics, and trimming of the coordination section to groups with
  clear dependencies.
- **4 were noted** without requiring charter changes — the
  Internationalization WG and APA WG had no concerns, the Privacy WG
  had no blocking issues, and the “CR Forever” approach was
  explained to the commenter’s satisfaction.
- **1 was deferred** (independent implementation language) to a broader
  charter-template-level discussion, per guidance from a W3C team
  member.
- **1 was marked Won’t Fix** (packaging format and signing) —
  browser vendors agreed at TPAC that this should remain out of scope
  for the initial charter.

The charter was approved by reviewers from Google (rdcronin), Mozilla
(Rob--W), and the W3C team contact (sideshowbarker).

## Horizontal Reviews

### 1. Internationalization WG — Noted

> No comment or request from i18n.

— himorin, [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-2947668653)

No action needed.

### 2. APA WG — Noted

> No comment or request from APA.

— ruoxiran, [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-2949087704)

No action needed.

### 3. Security IG — Accepted

> From the Security IG, we believe that standardization on the Web
> Extensions side is a particularly important element for the Threat
> Model for the Web. Therefore, we would like to ask you to consider
> adding the Threat Model for the Web, particularly for the part
> concerning Web Extensions.

— simoneonofri, [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-2949428870)

**Response:** Threat Modeling CG added to the Coordination section.
“Threat Model document” added to Other Deliverables.

### 4. Privacy WG (PING) — Noted

> No particular privacy concerns or blockers regarding the charter.
> However, we note that this is going to be very privacy-relevant work
> (adding surface area to the whole user agent itself, not just from a
> site), and will be challenging given the limitations of existing
> deployments. I recognize that ’app store’ stuff is out of scope,
> but some things about reputation/integrity/audits/evaluations is going
> to be pretty important for a good cross-browser privacy and security
> plan.

— npdoty, [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-3297048789)

**Response:** No charter change requested. The group welcomes future
engagement with the Privacy WG on these topics.

## TAG Review

### 5. Threat Modeling document — Accepted

> Incorporate a “Threat Modeling” document under the Other
> Deliverables section to help implementers and developers understand
> potential attack surfaces and mitigations.

— csarven (TAG), [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-3257447876)

**Response:** “Threat Model document” added to Other Deliverables in
[PR #711](https://github.com/w3c/charter-drafts/pull/711).

### 6. Authentication / credential handling in Scope — Accepted

> Incorporate “authentication” under the Scope section to cover
> extension-specific credential handling, background access, and
> interactions with auth flows.

— csarven (TAG), [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-3257447876)

**Response:** Rather than an authentication-specific section, two new
scope entries were added: “User agent extensibility” (covering all
browser features extensions may access) and “Network request
modification” (covering implications on authentication, identity,
navigation, and session management). This broader approach was
[endorsed](https://github.com/w3c/strategy/issues/146#issuecomment-3378316920)
by the team contact.

### 7. Update Coordination section — Accepted

> To ensure adequate coordination with other groups and organisations,
> the charter should include or clarify relevant coordination points.

— csarven (TAG), [charter-drafts#690](https://github.com/w3c/charter-drafts/issues/690)

**Response:** Initially all suggested groups were added. After discussion
at TPAC and in the PR, the list was
[trimmed](https://github.com/w3c/charter-drafts/pull/711#discussion_r1933279696)
to groups with clear or strong dependencies. See also comments 14 and 19.

### 8. Incubation / MV3 lessons — Noted

> The charter could clarify whether sufficient incubation has occurred
> to navigate prior experience and developer feedback, such as lessons
> from Manifest V3.

— csarven (TAG), [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-3257447876)

**Response:** TAG
[subsequently clarified](https://github.com/w3c/strategy/issues/146#issuecomment-3417093218)
that this was discretionary. Left to the group’s judgment; no charter
change made.

### 9. Packaging format and signing — Won’t Fix

> Packaging format and methods for signing extensions, currently marked
> out of scope, are very important areas. A common format could support
> decentralization and reduce reliance on extension stores.

— csarven (TAG), [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1889485437)

**Response:** Discussed at TPAC. No browser vendor currently
participating is interested in pursuing this for the initial charter.
The group will focus on the common API surface and reducing
implementation inconsistencies.
[Resolved](https://github.com/w3c/charter-drafts/pull/711#discussion_r1889485437)
as Won’t Fix for the initial charter; may be revisited in future
rechartering.

### 10. Independent implementation language — Deferred

> Independent implementations must be developed by separate parties and
> cannot reuse or derive code from another qualifying implementation
> relevant to this specification.

— csarven (TAG), [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1889529077)

**Response:** Per
[jyasskin’s suggestion](https://github.com/w3c/charter-drafts/pull/711#discussion_r1889529077),
deferred to a broader discussion about the charter template itself,
rather than modifying this specific charter.

## Other Strategy Issue Feedback

### 11. Recommendation track — Noted

> Curious why there is no intention to take the specifications to
> Recommendation?

— Chris Lilley (svgeesus), [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-2710937575)

**Response:** Explained that the “CR Forever” (living standard)
approach is the best fit given that the web extensions platform is
constantly evolving, and that transitioning from CR to Recommendation
later is easier than the reverse.
[Full response](https://github.com/w3c/strategy/issues/146#issuecomment-2711226413).

### 12. Naming: “web extensions” vs “browser extensions” — Accepted

> Why is this called “web extensions” when it is about *browser*
> extensions?

— Martin Thomson (martinthomson), [strategy#146 comment](https://github.com/w3c/strategy/issues/146#issuecomment-2711014539)

**Response:** Explained
[historical naming context](https://github.com/w3c/strategy/issues/146#issuecomment-2711226413).
Naming was later standardized to CamelCase “WebExtensions”
throughout the charter (see comment 17).

## PR Review Feedback

### 13. Editorial copyediting — Accepted

Seven editorial suggestions improving wording, grammar, and clarity
across the Scope section (user agent extensibility, resource files,
WebDriver integration, extension/web interactions, network request
modification).

— sideshowbarker, [PR #711 review](https://github.com/w3c/charter-drafts/pull/711#pullrequestreview-3333339939)

**Response:** All suggestions accepted and incorporated.

### 14. Remove FedCM from Coordination section — Accepted

> FedCM should be removed from the charter coordination section. The
> WECG has had no discussion about FedCM, only Chrome implements it,
> Mozilla’s position is neutral, and WebKit’s position is
> unpublished.

— Rob--W, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1885979479)

**Response:** Discussed at TPAC.
[Consensus](https://github.com/w3c/charter-drafts/pull/711#discussion_r1885979479)
was that FedCM is not integral enough to warrant listing. Removed from
the charter.

### 15. Vendor autonomy language — Accepted

> The CG charter includes an “Autonomy” section acknowledging that
> browsers will provide significantly more than what the spec covers,
> and that vendor-specific experimentation is expected. Similar language
> should be in the WG charter.

— rdcronin, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1890121069)

**Response:** Language about vendor autonomy added in
[commit 4847de2e](https://github.com/w3c/charter-drafts/pull/711/commits/4847de2e198979b5f51b74c610b073980a8f0469).
[Confirmed](https://github.com/w3c/charter-drafts/pull/711#discussion_r1923879754)
by rdcronin.

### 16. Mission statement / browser UI — Accepted

> The opening description should explicitly mention that extensions can
> add to and extend features of the browser interface.

— carlosjeurissen, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1897479006)

**Response:** Mission statement revised in
[commit 9af31b97](https://github.com/w3c/charter-drafts/pull/711/commits/9af31b9769a3ccfc4fb0a8c1b1e0e00a2dc05e23)
to read: “Users can extend their browsers with extensions: small
applications that run within a browser that modify its behavior, change
web page content, and add or enhance interface features.” Additional
editorial suggestions also incorporated.

### 17. “WebExtensions” vs “Web Extensions” naming consistency — Accepted

> Inconsistency between “Web Extensions” and “WebExtensions”
> throughout the document. Should not be both “Web Extensions Working
> Group” and “WebExtensions WG.”

— rdcronin, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1926781325)

**Response:** Standardized to CamelCase “WebExtensions” throughout
in [commit 012ec12c](https://github.com/w3c/charter-drafts/pull/711/commits/012ec12c).

### 18. Browser UI out of scope — Accepted

> Browser UI should be explicitly called out as out of scope, including
> specific UI related to permission requests and installation, which is
> left to the user agent.

— rdcronin, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1926790423)

**Response:** Added “User interface specifics” to the Out of Scope
section in
[commit e0155740](https://github.com/w3c/charter-drafts/pull/711/commits/e0155740),
clarifying that UI specifics are out of scope while UX discussions (e.g.,
permission management user journeys) remain in scope.

### 19. Trim coordination groups list — Accepted

> It is strange to list groups the WG might only occasionally interact
> with. Since extensions touch the entire web platform, the group will
> likely interact with most W3C groups. Suggest keeping only groups with
> clear dependencies.

— rdcronin, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1926800280)

**Response:** Coordination section trimmed to groups with clear or strong
dependencies in
[commit 282bcdcd](https://github.com/w3c/charter-drafts/pull/711/commits/282bcdcd0b1332553ddedec364042d4d457825bf).
Groups with weak or no known dependency (ECMA TC39, Web Authentication
WG, Web Applications Security WG, WHATWG, Web Applications WG, IETF)
were removed.

### 20. Conformance testing exception for packaging — Accepted

Out of Scope section revised to allow packaging discussion as it relates
to conformance testing.

— dotproto, [PR #711 comment](https://github.com/w3c/charter-drafts/pull/711#discussion_r1938055985)

**Response:** Resolved in
[commit 22ef9825](https://github.com/w3c/charter-drafts/pull/711/commits/22ef9825).

## Approvals

The following reviewers approved the charter revision PR:

- **sideshowbarker** (W3C team contact) — [approved](https://github.com/w3c/charter-drafts/pull/711#pullrequestreview-3333339939) 2025-10-13
- **rdcronin** (Google) — [approved](https://github.com/w3c/charter-drafts/pull/711#pullrequestreview-3485178194) 2025-12-19, “LG % comments”
- **Rob--W** (Mozilla) — [approved](https://github.com/w3c/charter-drafts/pull/711#pullrequestreview-3497975255) 2025-12-24, “Looks good to me (on behalf of Mozilla)”
