# invert-display
Quickly change display characteristics to help deal with differing external lighting conditions.

This simple script leverages *xcalib* to provide four potentially useful display settings:

  * **inverted:** Minimizes total light output when combined with a display that has no dark-colored background elements.  This is intended for use at night when you want to preserve your eyes' dark adaptation, e.g., you have a laptop mounted in your car while driving at night.  It is typically used with a dimmed backlight.
  
  * **dimmed-inverted:**  For the case where the backlight can't be dimmed enough, which can be the case when you are located far from city lights.
  
  * **high-gamma:**  Helps deal with incident skylight or sunlight, or can increase contrast when dealing with an inherently low-contrast display.
  
  * **normal:**  To return your display to its factory settings.  This is likely the only setting with which you will want to view pictures.
  
Invert-display makes use of *xcalib* to cycle through its four settings.  It is intended to be triggered by the click of a panel button.  Four clicks will return it to its current setting.

Graphramps uses *graph* from the *GNU Plotutils* package as well as *xcalib* to show the ramps of your current display.  It is rather crude and may need to be adjusted to match the size of your ramps.
