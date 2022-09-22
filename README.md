# cat-adoption

<strong>Problems in the Process</strong> </br>
1. Rounded corner bug: @login.html
- The corners got cut off when rounded class was applied to both input fields. 
- What we did: inspect the login.html and css file
- The problem: The bg-color rule that was applied universally
- Solution: Instead of applying it by the universal rule, we changed it to </br>
html, body, main, header {
    background: #d4ecc7;}
- Advice: Use the universal rule sparingly.
</br>
</br>
2. Image don't fill up the who top of product card: @catprofile.html
- There were spaces both left and right of the image.
- What we did: Inspect the card, try applying margin/ padding, try unapplying Bootstrap rules.
- The problem: .row gutter was 1.5 by default
- Solution: Apply class g-0 to the rows (Bootstrap 5)
