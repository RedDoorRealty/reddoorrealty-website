# Red Door Realty website

Website for Red Door Realty (reddoorrealtyme.com), owned and run by Randy Caron, Realtor and Designated Broker (Maine license DB920716), Portland, Maine. Randy is the site's owner and decides what goes on it.

## How the site works

- `index.html` is the entire website: all text, styles, scripts and embedded images in one file. Edit this file for every change.
- Hosting: Netlify, connected to this GitHub repository. Every push to `main` publishes the live site within about a minute.
- `netlify.toml`: publishing settings, plus redirects from old Placester page addresses (/about/, /contact/ etc.) to sections of this page. Keep them.
- `share.jpg` (social share image) and `favicon.png` (browser tab icon).
- Forms use Netlify Forms: `home-value`, `schedule-call`, `listing-alert`. Each has a hidden `form-name` field, a hidden `subject` field for the notification email, and a `company` honeypot field. Keep these when editing forms. Lead emails are set in Netlify under Forms > Submission notifications.

## Publishing costs credits: batch changes

Each Netlify production deploy (each push to `main`) uses 15 Netlify credits. Make all the changes for a request, check them, then commit and push once. Never push after every small edit.

## Business facts used on the site

- Fee: 3.5% total commission = 1.5% listing fee + 2% offered to the buyer's agent. Compared against the typical 5% to 6% total in Maine. Buyer-agent compensation is negotiable; say so where relevant.
- Tagline: "Full Service. Fair Fee."
- Licensed since 2004. Designated Broker. University of Southern Maine, School of Business.
- Phone (207) 712-2958 · Email RandyCaronRealtor@gmail.com · 15 Northwood Dr, Portland, ME 04103.
- Serves Greater Portland, Southern Maine (York County), the Lakes Region, the Midcoast and Central Maine (Lewiston-Auburn).
- Savings calculator starts at $500,000 (about Portland's median, Redfin early 2026).
- "Search homes" links open the public Maine Listings search in a new tab: https://mainelistings.com/listings?mls_status=Active,Active+Under+Contract,Coming+Soon+/+No+Show,Pending

## Adding a sold home ("Recently sold" section, id="sold")

1. Only add homes where Red Door Realty was the LISTING broker. Verify on a public listing site (Redfin, Zillow, Compass, Coldwell Banker, Carey & Giampa listing pages). If Red Door only represented the buyer, do not add it and do not show a "seller kept" figure.
2. Card details: address and town, "Sold · Month Year", beds · baths · sq ft · MLS #, sale price. Add "$X over asking" or "Under contract in N days" only when the price history confirms it.
3. Seller kept = 2.5% of the sale price (6% minus 3.5%). The $ totals in the hero banner and above the sold cards add themselves up from the cards in the page script; no need to edit them by hand.
4. Photo: crop to 16:10, resize to 720x450, save as WebP (quality ~72), embed as a base64 data URI in the card's `<img>` with a descriptive alt text. Never copy photos from Zillow or other sites; use photos Randy supplies.
5. Keep cards newest first.

## Design rules

- Always the light (white) version; there is no dark mode on purpose.
- Brand red #cf1f26 for buttons and highlights; dark blue-green for contrast bands; green for money-saved figures. The logo is red, so do not change the brand color.
- Must work on phones: check at about 390px wide with no sideways scrolling.
- Copy follows StoryBrand: the seller is the hero, Randy is the guide. Confident and fair-priced, never "cheap" or "discount." Do not name or attack other brokerages.
- Keep claims accurate: savings are estimates, commissions are negotiable, the Maine Listings disclaimer stays in the footer.
