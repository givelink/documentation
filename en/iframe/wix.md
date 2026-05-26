# Wix Integration

## Option A – Button

Follow the steps below:

1. Copy the html code by <strong>selecting</strong> the non profit that you want to promote from our [Widget Copy Page](https://givelink.app/charities/widget-gen)

   ![Copy Code](/assets/widget-gen.png)

2. Go to your Wix edit panel.
3. Navigate to `Website & mobile app > Website`, press edit site on top right

4. Select Add Element on the top left, then Button

![Add Button](/assets/wix/wix_add_button.png)

5. Place the button on the page. Feel free to customize colors & font according to your site. Make sure the Call-To-Action is <strong>"Give in-kind"</strong>, <strong>"View our Needs"</strong> or something else similar.

6. From the top bar, enable Dev mode, then select the button you just created and add as id: `givelink-button`

![Dev Mode](/assets/wix/dev_mode.png)

7. Add the following code to the page code:

```javascript
$w.onReady(function () {
  $w("#givelink-button").customClassList.add("givelink-button");
});
```

![Velo Code](/assets/wix/velo_code.png)

8. Click on add element and search for Custom code

![Custom code Element](/assets/wix/custom_code_element.png)

9. Add to a new Custom code element in the body start section, paste the code you copied on step 1 and then hit apply.

![Custom code Page](/assets/wix/custom_code_page.png)

![Add Code](/assets/wix/add_code.png)

10. Save and publish your site when you are ready.

---

## Option B – Inline Widget

The widget is displayed directly on the page — no button click needed. Visitors see it immediately when they arrive.

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. In the Wix editor, click **Add Element → Embed → Embed HTML**
3. Paste the inline embed code and resize the element to fit your layout
4. Save and publish

> 💡 **Tip:** The inline embed code (Option B) is different from the popup script (Option A). Make sure to select the correct tab in the Widget Generator.
