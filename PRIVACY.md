# Privacy Policy — ChainLearn

**Last updated:** 17 May 2026
**Effective date:** 17 May 2026

This Privacy Policy describes how ChainLearn ("we", "us", "the app") collects, uses, stores, and shares your personal information when you use the ChainLearn mobile application on iOS and Android. It also explains your rights regarding your data.

ChainLearn is operated by **Kaan Cankaya**, located in Melbourne, Victoria, Australia. For any questions about this policy or to exercise your data rights, contact: **kaancnkya@gmail.com**

---

## 1. Information We Collect

### 1.1 Information you provide directly

- **Email address** — required to create an account. We use it to authenticate you (via magic link or password), to recover access, and to send account-related notifications. We do not send marketing emails unless you explicitly opt in.
- **Words you add to your chain** — every word you choose to learn becomes part of your personal vocabulary chain. This is the core data of the product.
- **Spaced repetition review responses** — your "Forgot / Hard / Good / Easy" ratings on review cards, used to schedule future reviews and to mark words as mastered.
- **Settings preferences** — theme, UI language, audio playback settings, notification preferences.

### 1.2 Information collected automatically

- **Anonymous user ID** — when you first open the app, we create an anonymous Supabase user account so your data can sync across sessions before you sign up. This ID is replaced (via identity linking, not deletion) when you provide your email.
- **Device and OS version** — for crash diagnostics only.
- **Crash reports** — via Sentry. Includes stack traces and device metadata. Does not include the contents of your chain.
- **IP address** — logged by our hosting provider (Supabase) for security and abuse prevention. Retained for 30 days.

### 1.3 Information from third-party sign-in providers

If you sign in with **Apple** or **Google**:

- **Apple Sign In** — we receive a stable identifier and, optionally (only if you grant), your name and email. Apple's "Hide My Email" relay address is accepted. We do not receive your Apple ID password or any other Apple account data.
- **Google Sign In** — we receive your name, email, and Google profile ID. We do not receive your Google password or access to your Google account.

### 1.4 Information related to in-app purchases

- **Subscription status** — managed by RevenueCat. We store: subscription tier, period start/end, product ID. We do not store credit card numbers or payment information — those are handled exclusively by Apple and Google.

### 1.5 Camera and microphone

- **Camera access (Book Scan)** — when you use the Book Scan feature to capture a book page, the photo is sent to our LLM proxy server, where text is extracted by an OCR model. **The photo is not stored** on our servers after the extraction completes (transient processing only). The extracted text is returned to your device and is not stored on our servers.
- **Microphone access (Pronunciation)** — used only for in-app pronunciation practice. Audio is **processed locally on your device** and is not transmitted to our servers.

We request these permissions only when you initiate the relevant feature.

---

## 2. How We Use Your Information

We use your information for the following purposes:

1. **Provide the service** — sync your chain across devices, schedule reviews, generate example sentences for new words.
2. **Authenticate you** — verify it's you when you sign in.
3. **Process payments** — through Apple App Store, Google Play Store, and RevenueCat. We do not see your payment details.
4. **Improve reliability** — fix crashes and performance issues using Sentry diagnostic data.
5. **Communicate** — send essential transactional emails (magic link, password reset, subscription receipts). We do not send marketing emails without opt-in.

We do **not**:
- Sell your personal information to anyone.
- Use your chain content to train AI models.
- Track you across other apps or websites.
- Show advertisements in the app.

---

## 3. Third-Party Services We Use

| Service | Role | Data shared |
|---------|------|-------------|
| **Supabase** (Australia / EU region) | Hosting, database, authentication | Account email, chain data, IP, subscription status |
| **Anthropic** (US) | Sentence and definition generation (via Claude) | Words, sentences, and OCR images (transient) |
| **OpenAI** (US) | Text-to-speech audio generation | Text strings to be spoken aloud |
| **YouTube Data API** (Google, US) | Example video lookup for words | Word being searched (no user identifier) |
| **RevenueCat** (US) | Subscription management | Anonymous user ID, subscription product ID, period |
| **Apple App Store** (US) | Payments and Sign in with Apple | Per Apple's privacy policy |
| **Google Play Store / Google Sign In** (US) | Payments and Google Sign In | Per Google's privacy policy |
| **Sentry** (US) | Crash reporting | Stack traces, device model, OS version |

We have data processing agreements with each of these services where applicable.

---

## 4. Data Storage and Security

- Your data is stored on **Supabase infrastructure**, primarily in **Australia or the EU** region (depending on your account region). We do not store data on devices outside these regions.
- All data in transit is encrypted via **TLS 1.2+**.
- All data at rest is encrypted using Supabase's standard encryption.
- Server access is restricted to authorized personnel via SSH key authentication.
- We use Supabase Row Level Security (RLS) so that database queries can only access your own rows.
- Anthropic and OpenAI API keys are stored server-side only — never bundled in the app binary.

---

## 5. Data Retention

- **Account data** — kept for as long as your account is active.
- **Anonymous account data** — kept for **180 days** of inactivity. After that, anonymous accounts that never linked to an email are garbage-collected.
- **Crash reports (Sentry)** — kept for 90 days.
- **Server logs (IP, request timing)** — kept for 30 days.
- **OCR images** — not retained; processed in-memory and discarded immediately.
- **Microphone audio** — not retained; not transmitted to our servers.

If you delete your account, all data is permanently deleted within **30 days** (the buffer accounts for backup rotation).

---

## 6. Your Rights

You have the following rights regarding your personal data:

- **Access** — you can request a copy of all personal data we hold about you.
- **Correction** — you can correct inaccurate data via the Settings screen or by contacting us.
- **Deletion** — you can delete your account in-app (Settings → Account → Delete Account). All data is removed within 30 days. You can also email us to request deletion.
- **Portability** — you can request your chain data in machine-readable JSON format.
- **Objection** — you can object to specific processing activities.
- **Withdraw consent** — you can withdraw consent for optional processing at any time.
- **Lodge a complaint** — you may lodge a complaint with the **Office of the Australian Information Commissioner (OAIC)** at oaic.gov.au, or with your local data protection authority in the EEA.

To exercise any of these rights, email: **kaancnkya@gmail.com**. We respond within 30 days.

---

## 7. Children's Privacy

ChainLearn is **not directed at children under 13**. We do not knowingly collect personal information from children under 13. If you become aware that a child has provided us with personal information, contact us and we will delete it.

Users between 13 and 18 should review this policy with a parent or guardian.

---

## 8. International Data Transfers

By using the app, you understand that your data may be transferred to and processed in countries outside your country of residence — specifically, in the United States (Anthropic, OpenAI, YouTube, RevenueCat, Sentry) and the European Union (Supabase, depending on region).

These transfers are made under **Standard Contractual Clauses** (for EU/EEA users) or equivalent legal frameworks. The U.S. providers we use have committed to GDPR-equivalent data protection terms.

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will:

1. Update the "Last updated" date at the top of this policy.
2. Notify you in-app for material changes (changes that affect what data we collect or how we use it).
3. Require your consent for changes that materially expand our processing of your data.

The current version is always available at the URL of this document.

---

## 10. Contact

For any privacy-related question or request:

**Kaan Cankaya**
Email: kaancnkya@gmail.com
Location: Melbourne, Victoria, Australia

For data protection authority complaints:
- Australia: Office of the Australian Information Commissioner — oaic.gov.au
- European Union: your local DPA (find yours at edpb.europa.eu)
