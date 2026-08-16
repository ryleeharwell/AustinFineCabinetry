Drop your cabinetry photos in this folder, then reference them in the HTML.

Two places currently use placeholder blocks that should become real photos:
1. The hero "split-frame" on index.html and about.html (white cabinetry + dark cabinetry)
2. The 9 tiles in the .photo-grid on gallery.html

To swap a placeholder for a real photo, replace a div like this:
  <div class="photo">Kitchen — white uppers, dark island</div>
with an actual image tag:
  <div class="photo"><img src="images/kitchen-01.jpg" alt="Kitchen with white upper cabinets and dark island" style="width:100%;height:100%;object-fit:cover;border-radius:6px;"></div>

For the hero split-frame, set the background image via inline style on the panel:
  <div class="panel-light" style="--img-light:url('images/kitchen-01.jpg');"></div>
  <div class="panel-dark" style="--img-dark:url('images/kitchen-02.jpg');"></div>

Recommended: compress photos (e.g. via squoosh.app) before uploading so the site stays fast.
