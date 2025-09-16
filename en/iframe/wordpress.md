# WordPress Integration

1. Copy the html code that it is provided in the [Charity Interface](https://ci.givelink.app).

![Copy Code](/assets/ci-1.png)
![Copy Code](/assets/ci-2.png)

2. Go to your WordPress admin panel and log in.
3. Navigate to the page or post where you want to add the donation button.

4. Add a new code block by clicking the "+" button and selecting "Code" from the block options.
   ![Add Code Block](/assets/wp/wp-code-insert.png)

5. Paste inside the code block the script provided by the step 1.
   (this will be not be shown to the users)

6. Add a new button block by clicking the "+" button and selecting "Buttons" from the block options.
   ![Add Button Block](/assets/wp/wp-button-insert.png)

7. Click on the button to edit its text and change it to something like "Donate Now".

8. With the button selected, on the right side, click on advanced and add on Additional css class(es) the following: `givelink-button`.
   ![Add CSS Class](/assets/wp/wp-button-classname.png)
