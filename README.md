# Interactive Quote Calculator

This is a dynamic, client-ready quote calculator designed to showcase a wide range of service offerings and allow potential clients to estimate costs in real time. It supports custom features, bundled discounts, expandable service categories, and exportable results — perfect for embedding in websites or sending in emails.

---

## 🔧 Features

* 🧠 **Expandable Service Categories** — Organized by domain (AI, Hosting, Education, etc.)
* ✅ **Selectable Features** — Clients choose what they need
* 📊 **Real-Time Quote Summary** — Instantly calculates totals
* 💸 **Bundle Discounts** — Applies automatic discounts when certain combinations are selected
* 🛈 **Tooltips** — Short explanations for each feature
* 📥 **Download as PDF** — Clients can export their selections and quote
* ✨ **Scalable & Maintainable** — Easily add/remove categories and features via a JSON-like structure

---

## 🚀 Use Cases

* Embeddable on portfolio or service websites
* Attach in proposal emails as a calculator or PDF
* Lead generation or quote confirmation forms
* Freelancer/agency pricing breakdowns

---

## 🗂️ Project Structure

```
quote-calculator/
├── index.html       # Main calculator logic, UI, and styling
├── README.md        # Project overview and usage
```

> No external dependencies. This is a self-contained HTML/CSS/JS app.

---

## 📌 How to Use

### 🔗 Embed in Website

```html
<iframe 
  src="https://yourdomain.com/quote-calculator.html" 
  width="100%" 
  height="600" 
  style="border:none; border-radius:12px"
  title="Quote Calculator"
  loading="lazy">
</iframe>
```

### 📄 Export Quote

Click **“Download PDF”** to get a `.txt` version of the quote. This can be saved, printed, or attached in emails.

---

## 🧠 How to Add a New Service or Feature

Open `index.html`, and locate the `services` array in the script:

```js
const services = [
  {
    category: \"🧠 AI & Web App Development\",
    features: [
      { label: \"Custom AI Tools ($500+)\", value: 500, tooltip: \"GPT tools, blog editors, educational AI integrations\" },
      ...
    ]
  },
  ...
];
```

Simply add a new `category` object or append to the `features` array. No HTML changes needed.

---

## 💡 Future Ideas

* Email quote to client (with `mailto:` or backend handler)
* Connect to Firebase/Supabase to store quote history
* Optional user login or saved preferences
* Add currency selector (USD, EUR, etc.)

---

## 📬 Contact

Need a custom version or help integrating it into your platform?
* **Email:** `hello@example.com`
* **GitHub:** [YourUsername](https://github.com/YourUsername)
* **Portfolio:** [yourdomain.com](https://yourdomain.com)
