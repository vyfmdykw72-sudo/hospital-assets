THE F WARD — INTERACTIVE PROTOTYPE 01

FILES
index.html                  New prototype, replaces the old splash-screen index
pannellum.js / pannellum.css  Your original local Pannellum 2.5.6 files, unchanged
scary_hospital_hallway.jpg   Your uploaded test panorama, unchanged

HOW TO TEST
1. Keep all four files in the same folder.
2. Upload this folder to a NEW GitHub repository, or put it in a separate /prototype-01/ folder in your existing GitHub Pages repository. Do not overwrite your working homepage yet.
3. Open the hosted index.html URL. Use GitHub Pages or a local HTTP server, not file://.
4. Click Enter Hospital, drag to look around, and click the glowing markers.
5. Click Patient Records to see a three-slide sample carousel; use Previous/Next or arrow keys. Close to return to the hallway with the blur removed.
6. Click Exit Hospital to return to the temporary exterior.

IMPORTANT
- The exterior is intentionally a styled placeholder, NOT a generated hospital photo.
- Marker coordinates are APPROXIMATE. The panorama does not yet depict the final hallway layout. Adjust the pitch/yaw values in the HOTSPOTS array near the bottom of index.html to place markers precisely.
- To find pitch/yaw, temporarily add hotSpotDebug:true in the pannellum.viewer configuration, open browser developer tools (Console), and click a target location in the panorama; Pannellum logs the pitch and yaw. Remove hotSpotDebug afterward.
- The hallway exit hotspot is just a test marker. The final exit will be aligned with the entrance double doors in the final hallway panorama.
- Carousel entries are HTML placeholders, not finished Photoshop files. Future versions can replace them with image paths.
- Ambient audio is deliberately omitted from this first test to keep it simple and avoid autoplay issues.
- A single panorama cannot show true movement between camera locations; that requires additional panoramic renders.
