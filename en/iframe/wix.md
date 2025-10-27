# Wix Integration

Follow [this](https://youtu.be/AjSbpcc2uSE) step by step video, or read the steps below:

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

![Custom code Page](/assets/wix/custom_code_page.png)

![Custom code Element](/assets/wix/custom_code_element.png)

9. Add to a new Custom code element in the body start section, paste the code you copied on step 1 and then hit apply.

![Add Code](/assets/wix/add_code.png)

10. Save and publish your site when you are ready.
