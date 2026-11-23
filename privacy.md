---
title: Privacy Policy
updated: 2026-11-23
---

## Summary

- Logue is built on the AT Protocol. What you publish (logues, posts, follows, your profile) is stored in **your own account** on your Personal Data Server (PDS) and is **public to everyone** on the network, not only on Logue, unless you publish it in a non-public space (section 5).
- We keep an index of that public data so Logue can show it quickly. Privately, we keep only what we need to sign you in (your email address and your login session) and to send the email subscriptions you ask for, which you can also use without an account.
- We do not track you. We measure how Logue is used only on our own servers, without analytics cookies or scripts in your browser, and only in aggregate. If we show ads, they will be based on what you are reading, not on a profile of you. We do not sell your data.
- If you are signed in, we suggest logues on the Explore page based on what you publicly follow and like. You can turn this off at any time.

## 1. Data controller

Logue (logue.is) is operated by **Lefelys**, registered with the Dutch Chamber of Commerce (KVK) under number 42216103, in the Netherlands. We are the data controller for the personal data described in this policy.

This policy covers the Logue service at logue.is. Other instances running Logue's open-source code are run by their own operators, who are responsible for the data they process.

Contact us about privacy at [logue@lefelys.com](mailto:logue@lefelys.com). We have not appointed a Data Protection Officer.

## 2. Data on the AT Protocol

Logue does not own your account. You sign in with an existing Atmosphere account (for example Bluesky, Blacksky, Eurosky, or a self-hosted server). Your account provider runs your PDS and has its own privacy policy.

When you publish on Logue, we write records to your PDS using the open `is.logue.*` and `site.standard.*` formats. Unless you publish into a non-public space (section 5), those records, and any images you upload, are **public**. Anyone, including other apps, search engines, and archives, can read and copy them, and we cannot control what others do with them. Do not publish anything you want to keep private.

When you publish a post, you can choose to also share it to Bluesky. For each post you share, we create a Bluesky post (`app.bsky.feed.post`) in your account linking to your post on Logue. That Bluesky post is public and appears on Bluesky and in other apps that show Bluesky posts. When you delete the original post on Logue, we delete the Bluesky post we created as well.

Deleting a record on Logue deletes it from your PDS, and well-behaved apps will remove it too. We cannot guarantee that copies others made before the deletion are removed.

## 3. Personal data we process

### Registered users

- **Account identity**: your DID, handle, and the profile you set up on Logue (display name, avatar, bio, pronouns, website). On your first sign-in we copy your Bluesky profile as a starting point. Needed to run your account (performance of contract).
- **Email address**: read from your account provider when you sign in, or entered by you if your provider does not share one. We use it to contact you about your account or important changes, such as updates to this policy, and to deliver email subscriptions you turn on. You can also add up to 10 more addresses for email subscriptions, each confirmed with a code. We never use your addresses for marketing without asking and never share them. Kept privately in our database (performance of contract and legitimate interest).
- **Login session**: the OAuth tokens your account provider issues to Logue so we can publish on your behalf. Deleted when you log out (performance of contract).
- **Your public content**: logues, posts, images, follows, and co-logger relationships, as described in section 4.
- **Your non-public content**: content in spaces you own or belong to, and their member lists, as described in section 5 (performance of contract).
- **Recommendations**: to suggest logues on the Explore page, we use your public follows, likes, reposts, and similar public interactions on Logue and other AT Protocol apps, together with what people with similar follows read. We do not label you with interests or sensitive traits (such as health, religion, politics, or sexuality), and we never use non-public content to recommend anything to other people. You can turn personalised recommendations off in your settings; Explore then shows popular and new logues instead, and we delete the recommendation data we keep about you (legitimate interest in showing you relevant logues).

### Email subscribers

You can subscribe to a logue by email whether or not you have an account. These rules apply either way:

- **What we store**: your email address, which logues it is subscribed to, and when you confirmed it. This is kept privately, never in a public account. Publishers see only how many people subscribed, never who or their email addresses (performance of contract).
- **Confirming your address**: before we send anything else, we email you a 6-digit code to confirm the address is yours. The code expires after 10 minutes, and we store only a one-way hash of it. An address that is never confirmed receives nothing but the codes requested for it (performance of contract).
- **Bot check**: when you open the email subscription dialog, it runs Cloudflare Turnstile, so bots cannot use the form to send codes to other people's addresses. Turnstile loads a Cloudflare script in your browser that checks technical signals from your browser and device, such as how it renders and responds, to tell people from bots. Usually it runs unseen; sometimes it asks you to tick a box. It runs only in this dialog, and Cloudflare does not use it to track you across sites or for advertising (legitimate interest in preventing abuse of the form).
- **Abuse limits**: to limit how many codes can be requested or entered, we count requests per email address and per IP address for up to an hour. The counters are stored under a one-way hash of the address, not the address itself, and our logs of these requests contain neither your email address nor your IP address (legitimate interest in preventing abuse).
- **The emails**: when a logue you subscribed to publishes a public post, we email it to you. Every email has links to unsubscribe from that logue or from all logues, which work without signing in, and supports your email app's one-click unsubscribe button. Unsubscribing deletes the subscription. Our emails contain no tracking pixels or tracked links: images are loaded like on any web page, from our servers, Bluesky's image CDN, or, for an embedded video, the video's service (such as YouTube), at the same address for every reader, so we cannot tell who opened an email.
- **If you have an account**: you can also subscribe and unsubscribe in the logue's subscribe menu. If you later confirm, from your account, an address you subscribed with while signed out, those subscriptions join your account so you can manage them there.

### Authors of public content on the network

- Logue reads the public AT Protocol network through a relay service (the “firehose”) and indexes public records in the Logue and Standard.site formats, together with the author's DID, handle, and Logue profile. This lets Logue show publications written in other compatible apps (legitimate interest in running an open, interoperable reader). If you are listed as a co-logger, we store your DID and handle with that logue.
- We also index public interactions made in other AT Protocol apps, such as likes, reposts, replies, and follows (for example Bluesky's `app.bsky.*` records), when they involve content or people on Logue. We use them to show counts and conversations and, in aggregate, to recommend logues (legitimate interest). When an interaction is deleted on the network, we delete it too.

### All visitors

- **Technical logs**: like any website, our servers receive your IP address, browser type, and the pages you request. We use logs only to keep Logue secure and fix problems, and keep them for a short period (legitimate interest).
- **Usage statistics**: aggregate counts of how Logue is used, as described in section 7 (legitimate interest).
- **Link previews**: when someone adds a link to a post, our bot [LogueLinkPreviewBot](https://logue.is/bot) fetches the public page to build a preview. Previews are cached and not linked to you.

Apart from the optional recommendations described above, we do not profile you. We do not use your data for automated decisions with legal or similarly significant effects, and we do not use your content to train generative AI models or let others do so.

## 4. Indexing of public content

To display public content fast, we keep an indexed copy in our own database and caches. This includes your logues, posts, profile, the logues you follow, and your public interactions such as likes.

The original image files stay on your PDS. To load them quickly, we fetch them from your PDS when someone views them and keep cached copies on our image servers and content delivery network (CDN). Cached copies expire on their own, and we remove them when the image is deleted. Images from non-public spaces are cached separately and served only to people allowed to see them.

When you delete a logue or post, it disappears from Logue straight away. We may keep a hidden internal copy so our index stays consistent. You can ask us to erase these copies at any time.

We may also hide content from Logue to enforce our [Terms of Service](https://logue.is/terms). Hiding content on Logue does not delete it from your PDS.

## 5. Non-public content (spaces)

Some content on Logue, such as members-only logues and private follows, is stored in AT Protocol **spaces**: content that only the members of a space can read.

- **Who decides access.** Every space has an owner, usually the account that created it, who decides which accounts and apps can read it. Content in a space stays on each author's PDS, separate from public records.
- **Access control, not encryption.** Spaces limit who can read content; they do not encrypt it. Members, the apps a space allows, and the PDS that stores it can read it. Do not use spaces for highly sensitive information.
- **What Logue keeps.** To show you a space, Logue keeps a copy of its content and member list on our servers, and shows it only to members. We access it ourselves only to run Logue, to handle a report about it, or when the law requires.
- **Never for ads, analytics, or others' recommendations.** Non-public content is never used to choose ads, shared with advertisers, used to recommend anything to people outside the space, or used in analytics beyond simple totals.
- **Members can share.** Anyone who can read a space can copy what they see. Removing a member stops their future access but cannot take back what they already saw.
- **Removing content.** When content is deleted from a space, when the space is deleted, or when Logue loses access to it, we delete our copy.

## 6. Cookies and local storage

- **session**: one encrypted, first-party cookie that keeps you signed in. It contains only your DID and expires after 14 days or when you log out. It is strictly necessary, so it does not need your consent.
- **theme**: your light or dark mode choice, stored in your browser's local storage. It never leaves your device.
- **Security cookies**: Cloudflare, which protects Logue against attacks and abuse, may set short-lived cookies such as `__cf_bm` or `cf_clearance` to tell people apart from bots. They are strictly necessary and are not used for tracking.

We do not use analytics, advertising, or tracking cookies. Apart from the above, and the Cloudflare bot check that runs only when you subscribe by email (section 3), nothing is stored on or read from your device.

## 7. Analytics

We want to know whether Logue is useful, for example how many people read a logue or which pages break, without watching any one person. So our analytics follow these rules:

- **Server-side only.** We count the requests your browser already makes to our servers. There are no analytics scripts, pixels, cookies, local storage, or fingerprinting in your browser, so nothing is stored on or read from your device.
- **Self-hosted.** We use an open-source analytics tool that we run on our own servers. No analytics company receives data about your visit.
- **Only what we need.** For each page view we record the page, the referring website (domain only) and any campaign tags in the link, your country, and your browser and operating system name and version. The country comes from Cloudflare; the browser and system are read from your browser's User-Agent header, which is not stored.
- **No IP addresses.** Your IP address is never sent to or stored by our analytics. So that one visit is not counted as many, our server turns your IP address and browser into a one-way hash using a secret that is replaced every day. The hash is used only to group page views into a single visit, is deleted 8 hours after your last page view, and cannot be reversed or linked from one day to the next.
- **Totals only.** We do not store individual page views. What we keep are hourly and daily totals, such as how many visits a page had or how many came from a country, which say nothing about any one person. Analytics are never tied to your account. We may show totals, such as how many times a post was viewed, to its author or publicly.
- **Kept in-house.** Apart from basic traffic statistics that Cloudflare produces for us from the traffic it delivers, analytics stay on our servers and are never shared with or sold to third parties.
- **Respecting your signal.** If your browser sends Global Privacy Control or Do Not Track, we do not count your visit at all. Because our analytics cannot tell who you are, this is also the way to opt out: we have no records of your visits to find or delete.

## 8. Advertising

Logue does not show ads today. If we introduce ads or sponsored content, the same principles apply:

- **Contextual only.** Ads are chosen based on the page, logue, or topic you are viewing, never on your identity, the logues you follow, your browsing history, or any other profile of you.
- **No tracking.** Ads are served without cookies, tracking pixels, or third-party tracking scripts.
- **Not in non-public spaces.** Ads are never chosen based on non-public content.
- **Nothing shared with advertisers.** Ads are matched on our own servers. Advertisers receive only aggregate numbers, such as how many times an ad was shown or clicked, and never learn who saw an ad or receive your personal data.
- **Clearly labelled.** Ads and sponsored content are marked as such, together with who paid for them.

We will update this policy before ads start.

## 9. Recipients and international transfers

We do not sell or rent personal data. Some data reaches the following parties so Logue can work:

- **Your account provider (PDS)**: receives what you publish and the images you upload, and handles sign-in.
- **Bluesky Social PBC** (USA): some images may be served through Bluesky's image CDN; handle suggestions while typing a mention query Bluesky's public API; some link previews are fetched through Bluesky's preview service.
- **Cloudflare, Inc.** (USA): all traffic to Logue passes through Cloudflare, which delivers the site and images from servers near you and protects it against attacks. It therefore processes your IP address and request details on our behalf, and provides us with aggregate traffic statistics. When you subscribe by email, it also runs the bot check described in section 3.
- **Hetzner Online GmbH** (Germany): hosts the servers, databases, and image caches that store the data described above.
- **Our email delivery provider**: sends the emails described above, and receives your email address and the content of each email for that purpose only.
- **Embedded content**: when a post embeds content from YouTube (privacy-enhanced mode), X, Instagram, Reddit, Bluesky, or Bandcamp, your browser loads it directly from that service when you view the post. That service receives your IP address and may set its own cookies under its own privacy policy.
- **Authorities**: when we are legally required to.

Some of these services are outside the European Economic Area. Where that applies, transfers rely on the safeguards in the GDPR, such as the EU-US Data Privacy Framework or Standard Contractual Clauses.

## 10. Data retention

- Profile, email address, and indexed content: while your account is active on Logue, or until you ask us to delete it.
- Non-public content: while it exists in its space and Logue has access to it.
- Cached images: until the cache expires or the image is deleted.
- Recommendation data: while personalised recommendations are on; deleted when you turn them off. Interactions removed from the network are deleted from our index.
- Email subscriptions: until you unsubscribe, after which we delete them.
- Email verification codes: 10 minutes, stored only as a one-way hash. Abuse limit counters: up to an hour.
- Login session: until you log out or the session expires.
- Technical logs: only as long as needed for security and debugging.
- Analytics: visit hashes until 8 hours after your last page view, with the daily secret deleted every day; anonymous totals indefinitely.
- Link previews: cached and refreshed periodically.

## 11. Your rights

Under the GDPR you have the right to access, correct, delete, restrict, and port your personal data, and to object to processing based on legitimate interest. You can stop personalised recommendations yourself in your settings. To use these rights, email [logue@lefelys.com](mailto:logue@lefelys.com) from the address on your account, or, if you subscribed by email without an account, from the subscribed address. We reply within one month.

Content in your PDS is yours to edit or delete directly, in Logue or any compatible app. To remove your Logue account and our copy of your data, email us. Your Atmosphere account and data in other apps are not affected. If you keep publishing in Logue's formats, our index will pick it up again, because it is public.

You can complain to the Dutch Data Protection Authority ([Autoriteit Persoonsgegevens](https://autoriteitpersoonsgegevens.nl)) or the authority in your own EU country.

## 12. Children

Logue is not intended for anyone under 16. If you believe a child has given us personal data, contact us and we will delete it.

## 13. Security

Connections to Logue are encrypted (HTTPS), the session cookie is encrypted, and we never see your account password, because sign-in happens with your account provider. No system is perfectly secure; if a breach affects your data, we will notify you and the authorities as the law requires.

## 14. Changes to this policy

We will post updates on this page and change the date above. If a change is significant, we will give notice on Logue or by email before it takes effect. Every change is also announced in [Logue Legal](https://logue.is/~logue-legal-updates), which you can follow or subscribe to by email.
