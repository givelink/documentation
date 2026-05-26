# 🌟 Real-World Examples

See how nonprofits are using Givelink to accept in-kind donations on their websites.

---

## Nonprofits Using Givelink

| Organization | Website | Integration Type |
|---|---|---|
| Pilgrim Terrace | [pilgrimterrace.org/donate](https://pilgrimterrace.org/donate) | Option A – Button |
| Swords to Plowshares | [swords-to-plowshares.org](https://www.swords-to-plowshares.org/) | Option A – Button |
| The KSP | [theksp.org/donate-goods](https://www.theksp.org/donate-goods) | Option A – Button |
| BOSS | [bosshelp.org/donate-goods](https://bosshelp.org/donate-goods/) | Option B – Inline Widget |
| Rock SF | [rocksf.org/donate](https://rocksf.org/donate/) | Link to Givelink Profile |
| Heart to Art Collective | [hearttoartcollective.org](https://sites.google.com/view/hearttoartcollective/get-involved#h.tfcoiq7bsef0) | Link to Givelink Profile |

> **Rock SF** and **Heart to Art Collective** use the simplest approach: a plain hyperlink on their website pointing directly to their Givelink profile page — no embed code required.

---

## Option A – Button

A button is placed on your page. When clicked, it opens the Givelink donation widget in a popup overlay. This is the most common and easiest integration.

**Nonprofits using this option:** Pilgrim Terrace · Swords to Plowshares · The KSP

### WordPress

1. Copy your embed code from the [Widget Generator](https://givelink.app/charities/widget-gen)
2. In your WordPress editor, add a **Custom HTML** block and paste the embed code
3. Add a **Buttons** block and set its Additional CSS Class to `givelink-button`
4. Customize button text and colors to match your site
5. Save and publish

📖 [Full WordPress Guide →](wordpress.md)

---

### Squarespace

1. Copy your embed code from the [Widget Generator](https://givelink.app/charities/widget-gen)
2. Add a **Button** block to your page
3. Set the button link to `#givelink-button` (remove "Open in new tab")
4. Go to **Custom Code → Code Injection** and paste the embed code in the **Footer** section
5. Save and publish

📖 [Full Squarespace Guide →](squarespace.md)

---

### Wix

1. Copy your embed code from the [Widget Generator](https://givelink.app/charities/widget-gen)
2. Add a **Button** element to your page and customize it
3. Enable **Dev Mode**, select the button, and set its ID to `givelink-button`
4. Add this code to the **Page Code**:
   ```javascript
   $w.onReady(function () {
     $w("#givelink-button").customClassList.add("givelink-button");
   });
   ```
5. Add a **Custom Code** element (body start) and paste your embed code
6. Save and publish

📖 [Full Wix Guide →](wix.md)

---

### Custom Website (HTML/JavaScript)

1. Copy your embed code from the [Widget Generator](https://givelink.app/charities/widget-gen)
2. Paste it anywhere in your HTML (e.g., before `</body>`)
3. Add a button with the `givelink-button` class:
   ```html
   <button class="givelink-button">View Our Needs</button>
   ```
4. Deploy your changes

📖 [Full Native JavaScript Guide →](native.md)

---

## Option B – Inline Widget

The widget is embedded directly on the page — no button click needed. Visitors see the donation widget immediately when they visit the page.

**Nonprofits using this option:** BOSS

### WordPress

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. In your WordPress editor, add a **Custom HTML** block
3. Paste the inline embed code into the block
4. Save and publish

---

### Squarespace

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. Edit your page and add a **Code** block where you want the widget to appear
3. Paste the inline embed code into the block
4. Save and publish

---

### Wix

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. In the Wix editor, click **Add Element → Embed → Embed HTML**
3. Paste the inline embed code and resize the element to fit your layout
4. Save and publish

---

### Custom Website (HTML)

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. Paste it directly into your HTML where you want the widget to appear:
   ```html
   <!-- Paste your Givelink inline embed code here -->
   ```
3. Deploy your changes

---

> 💡 **Tip:** The inline embed code (Option B) is different from the popup script (Option A). Make sure to select the correct tab in the Widget Generator.

---

📖 **[Back to Integration Hub →](landing.md)**
