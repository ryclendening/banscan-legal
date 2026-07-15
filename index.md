# Privacy Policy for BanScan

**Effective Date: July 15, 2026**

BanScan helps users screen product ingredient labels against banned-substance lists. This policy explains what information BanScan processes, how optional AI-assisted label reading works, and the choices available to users.

## Information We Process

BanScan may process the following information when you use the app:

- Photos or images you choose to capture or upload
- Text and ingredient information extracted from product labels
- Text you highlight or submit for re-scanning
- Product barcodes you choose to look up
- Ingredient search inputs you submit in the app
- Limited technical and operational information needed to complete requests, diagnose errors, and maintain app functionality

BanScan does not require you to create an account.

## How We Use Information

BanScan uses this information to:

- Extract and normalize ingredient text from product labels
- Retrieve available product ingredient information from a barcode
- Check ingredients against banned-substance lists
- Display potential matches and supporting substance details
- Diagnose failures and maintain and improve app functionality

BanScan is a screening aid and does not make authoritative compliance, medical, eligibility, or safety decisions.

## On-Device and AI-Assisted Label Reading

BanScan offers on-device label reading and optional AI-assisted label reading.

If you select **Use On-Device Only**, the selected label image is processed on your device using Apple-provided image and text-recognition technologies. The image is not sent to BanScan's AWS proxy or Google Gemini for ingredient extraction.

If you select **Allow AI Analysis**, BanScan sends the selected label image over an encrypted HTTPS connection to a BanScan-operated proxy hosted using Amazon Web Services (AWS), including API Gateway and AWS Lambda. The proxy forwards the image and task instructions to the Google Gemini API so that Gemini can locate the ingredient region or extract ingredient information. The submitted image may include label text and nearby package or background details.

Gemini returns a detected ingredient region or extracted ingredient information to the proxy, which returns the result to the app. BanScan then normalizes the resulting ingredients and checks them against its banned-substance database.

Your AI-analysis choice is stored in the app. You can change it in **AI Privacy Settings**.

## Barcode Product Lookup

When you choose to look up a scanned or manually entered barcode, BanScan sends the barcode value to the Open Food Facts API. BanScan uses the returned product identity and ingredient data to perform the same ingredient normalization and banned-substance screening used for label scans.

BanScan does not upload your label photo to Open Food Facts as part of barcode lookup.

## Third-Party Services

BanScan uses the following service providers:

- **Amazon Web Services (AWS):** Hosts the API Gateway and Lambda proxy used for optional AI-assisted label analysis. See the [AWS Privacy Notice](https://aws.amazon.com/privacy/).
- **Google Gemini API:** Processes label images and returns ingredient-region or ingredient information when AI analysis is allowed. Google's handling of submitted content depends on the applicable Gemini service terms and account configuration. See the [Gemini API Additional Terms](https://ai.google.dev/gemini-api/terms) and [Google Privacy Policy](https://policies.google.com/privacy).
- **Open Food Facts:** Receives barcode values when you request a product lookup and returns community-provided product information. See the [Open Food Facts API documentation](https://openfoodfacts.github.io/documentation/docs/Product-Opener/api/).

These providers may process request metadata and submitted content according to their applicable terms, privacy notices, and service configurations.

## Data Sharing

BanScan does not sell user data. BanScan does not use label images, ingredient text, barcode values, or scan data for advertising or cross-app tracking.

BanScan shares information with the service providers described above only as needed to provide the feature you requested, maintain service security, diagnose failures, or comply with applicable legal obligations.

## Data Retention

BanScan does not intentionally maintain user scan history or store submitted label images in a BanScan user account or persistent scan-history database.

The AWS proxy processes AI-analysis requests and may generate limited operational logs, such as request status, timing, and error information. BanScan does not intentionally include label images or extracted ingredient text in those operational logs.

Third-party providers may retain submitted content or request metadata according to their own policies, terms, service configuration, and legal obligations. Images in your photo library remain subject to your device and photo-library settings.

## User Choices

You can:

- Use on-device label reading instead of AI-assisted analysis
- Change your AI-analysis choice in AI Privacy Settings
- Decline camera or photo-library access
- Use direct database search without submitting a label image
- Avoid barcode lookup and photograph the physical ingredient label instead

Disabling a permission or declining AI analysis may limit the related feature but does not prevent use of the app's available on-device and direct-search features.

## Security

BanScan uses encrypted HTTPS connections when communicating with its proxy and external APIs. No method of electronic transmission or processing is completely secure, but BanScan uses reasonable measures intended to protect submitted information.

## Changes to This Policy

BanScan may update this policy as the app and its service providers change. The effective date above indicates when this policy was last revised.

## Contact

For privacy questions, contact:

Ryan Clendening  
ryclendening@gmail.com
