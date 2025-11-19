# Image Setup Instructions

To complete the website setup, you need to copy the images to the correct locations:

## Partner Logos

**Source:** The horizontal partner logo strip (Image #1)
**Destination:** `C:\WebDev\WillSparkMedia\.playwright-mcp\current-website-full.png`

This image is already referenced in the HTML. No action needed if it's already there.

## Portfolio/Success Stories Images

Copy the following images to the `images` folder:

1. **Image #2** (Building/Corporate photo) → `images/portfolio-1.jpg`
2. **Image #3** (Laptop with analytics) → `images/portfolio-2.jpg`
3. **Image #4** (Portfolio yellow tiles) → `images/portfolio-3.jpg`

### Step-by-Step:

1. Create the `images` folder if it doesn't exist:
   ```bash
   mkdir C:\WebDev\WillSparkMedia\images
   ```

2. Copy your images:
   - Rename Image #2 to `portfolio-1.jpg` and place it in the `images` folder
   - Rename Image #3 to `portfolio-2.jpg` and place it in the `images` folder
   - Rename Image #4 to `portfolio-3.jpg` and place it in the `images` folder

### Alternative: Use the actual image paths

If you want to keep the original file locations, you can update the HTML image paths in `index.html`:

```html
<!-- Replace these paths with your actual image paths -->
<img src="path/to/your/image-2.jpg" alt="Business Growth Analytics" class="portfolio-img">
<img src="path/to/your/image-3.jpg" alt="Data Analytics Dashboard" class="portfolio-img">
<img src="path/to/your/image-4.jpg" alt="Portfolio Strategy" class="portfolio-img">
```

## Image Optimization Tips

For best performance:
- Use WebP format when possible
- Keep file sizes under 500KB
- Recommended dimensions: 800x600px for portfolio images
- Use tools like TinyPNG or ImageOptim to compress images

## Result

Once the images are in place, your website will show:
- Partner logos in a horizontal strip (responsive)
- Real portfolio images with smooth hover zoom effects
- Professional category badges overlaying the images